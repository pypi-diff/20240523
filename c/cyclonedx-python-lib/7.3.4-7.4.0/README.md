# Comparing `tmp/cyclonedx_python_lib-7.3.4.tar.gz` & `tmp/cyclonedx_python_lib-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyclonedx_python_lib-7.3.4.tar", max compression
+gzip compressed data, was "cyclonedx_python_lib-7.4.0.tar", max compression
```

## Comparing `cyclonedx_python_lib-7.3.4.tar` & `cyclonedx_python_lib-7.4.0.tar`

### file list

```diff
@@ -1,1148 +1,1148 @@
--rw-r--r--   0        0        0   276000 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/LICENSE
--rw-r--r--   0        0        0      147 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/NOTICE
--rw-r--r--   0        0        0     4571 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/README.md
--rw-r--r--   0        0        0      850 2024-05-06 13:40:55.852499 cyclonedx_python_lib-7.3.4/cyclonedx/__init__.py
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/_internal/__init__.py
--rw-r--r--   0        0        0     3148 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/_internal/compare.py
--rw-r--r--   0        0        0     1164 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/_internal/hash.py
--rw-r--r--   0        0        0      847 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/_internal/time.py
--rw-r--r--   0        0        0      993 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/exception/__init__.py
--rw-r--r--   0        0        0     1536 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/exception/factory.py
--rw-r--r--   0        0        0     3685 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/exception/model.py
--rw-r--r--   0        0        0     1136 2024-05-06 13:40:25.268526 cyclonedx_python_lib-7.3.4/cyclonedx/exception/output.py
--rw-r--r--   0        0        0     1730 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/exception/serialization.py
--rw-r--r--   0        0        0      680 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/factory/__init__.py
--rw-r--r--   0        0        0     4191 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/factory/license.py
--rw-r--r--   0        0        0    43540 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/__init__.py
--rw-r--r--   0        0        0    26098 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/bom.py
--rw-r--r--   0        0        0     2179 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/bom_ref.py
--rw-r--r--   0        0        0    59251 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/component.py
--rw-r--r--   0        0        0    11793 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/contact.py
--rw-r--r--   0        0        0    48270 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/crypto.py
--rw-r--r--   0        0        0     3766 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/dependency.py
--rw-r--r--   0        0        0     3568 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/impact_analysis.py
--rw-r--r--   0        0        0     7024 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/issue.py
--rw-r--r--   0        0        0    13070 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/license.py
--rw-r--r--   0        0        0     8623 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/release_note.py
--rw-r--r--   0        0        0    12798 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/service.py
--rw-r--r--   0        0        0    43655 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/model/vulnerability.py
--rw-r--r--   0        0        0     5872 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/output/__init__.py
--rw-r--r--   0        0        0     4270 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/output/json.py
--rw-r--r--   0        0        0     4285 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/output/xml.py
--rw-r--r--   0        0        0      153 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/py.typed
--rw-r--r--   0        0        0     3018 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/__init__.py
--rw-r--r--   0        0        0     2114 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/README.md
--rw-r--r--   0        0        0     2493 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/__init__.py
--rw-r--r--   0        0        0    13604 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
--rw-r--r--   0        0        0    39716 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
--rw-r--r--   0        0        0    37110 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    36226 2024-05-06 13:40:25.272526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    76383 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
--rw-r--r--   0        0        0    40324 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    39348 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    88794 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
--rw-r--r--   0        0        0    72300 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   133792 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
--rw-r--r--   0        0        0   164689 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   311805 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
--rw-r--r--   0        0        0   252643 2024-05-06 13:40:25.276526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   492947 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
--rw-r--r--   0        0        0     8058 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
--rw-r--r--   0        0        0    14269 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
--rw-r--r--   0        0        0   165694 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
--rw-r--r--   0        0        0     2573 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/schema/schema.py
--rw-r--r--   0        0        0     6576 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/serialization/__init__.py
--rw-r--r--   0        0        0     2503 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/spdx.py
--rw-r--r--   0        0        0     3701 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/validation/__init__.py
--rw-r--r--   0        0        0     4817 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/validation/json.py
--rw-r--r--   0        0        0      853 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/validation/model.py
--rw-r--r--   0        0        0     3672 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/cyclonedx/validation/xml.py
--rw-r--r--   0        0        0      634 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/Makefile
--rw-r--r--   0        0        0     1524 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/architecture.rst
--rw-r--r--   0        0        0      686 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/changelog.rst
--rw-r--r--   0        0        0     2657 2024-05-06 13:40:55.852499 cyclonedx_python_lib-7.3.4/docs/conf.py
--rw-r--r--   0        0        0       34 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/contributing.rst
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/examples.rst
--rw-r--r--   0        0        0     1857 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/index.rst
--rw-r--r--   0        0        0     1499 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/install.rst
--rw-r--r--   0        0        0      800 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/make.bat
--rw-r--r--   0        0        0     3275 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/modelling.rst
--rw-r--r--   0        0        0     2269 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/outputting.rst
--rw-r--r--   0        0        0       81 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/requirements.txt
--rw-r--r--   0        0        0     8093 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/schema-support.rst
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/docs/support.rst
--rw-r--r--   0        0        0      176 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/examples/README.md
--rw-r--r--   0        0        0     8164 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/examples/complex_deserialize.py
--rw-r--r--   0        0        0     4081 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/examples/complex_serialize.py
--rw-r--r--   0        0        0     4249 2024-05-06 13:40:55.852499 cyclonedx_python_lib-7.3.4/pyproject.toml
--rw-r--r--   0        0        0     6967 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/__init__.py
--rw-r--r--   0        0        0      704 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/__init__.py
--rw-r--r--   0        0        0    44385 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/models.py
--rw-r--r--   0        0        0       16 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/README.md
--rw-r--r--   0        0        0     1213 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1358 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0     1309 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
--rw-r--r--   0        0        0      567 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.4/empty_supplier.json
--rw-r--r--   0        0        0     2461 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/xml/1.4/bom_setuptools.xml
--rw-r--r--   0        0        0    98508 2024-05-06 13:40:25.280526 cyclonedx_python_lib-7.3.4/tests/_data/own/xml/1.4/webgoat-6.1.xml
--rw-r--r--   0        0        0     3723 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
--rw-r--r--   0        0        0     1195 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
--rw-r--r--   0        0        0      559 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
--rw-r--r--   0        0        0      313 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
--rw-r--r--   0        0        0      830 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
--rw-r--r--   0        0        0      801 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
--rw-r--r--   0        0        0      793 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
--rw-r--r--   0        0        0      769 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
--rw-r--r--   0        0        0     1303 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
--rw-r--r--   0        0        0    16515 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
--rw-r--r--   0        0        0    16513 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
--rw-r--r--   0        0        0     1328 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
--rw-r--r--   0        0        0     1366 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
--rw-r--r--   0        0        0      302 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
--rw-r--r--   0        0        0    21038 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
--rw-r--r--   0        0        0      348 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
--rw-r--r--   0        0        0    21026 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
--rw-r--r--   0        0        0     1217 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
--rw-r--r--   0        0        0      704 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
--rw-r--r--   0        0        0      965 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
--rw-r--r--   0        0        0      186 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
--rw-r--r--   0        0        0    22339 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
--rw-r--r--   0        0        0     1210 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
--rw-r--r--   0        0        0     1214 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
--rw-r--r--   0        0        0     1226 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
--rw-r--r--   0        0        0      317 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
--rw-r--r--   0        0        0    21121 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
--rw-r--r--   0        0        0    10048 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
--rw-r--r--   0        0        0      165 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
--rw-r--r--   0        0        0      560 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
--rw-r--r--   0        0        0      385 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
--rw-r--r--   0        0        0      433 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
--rw-r--r--   0        0        0      249 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
--rw-r--r--   0        0        0      314 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
--rw-r--r--   0        0        0      667 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
--rw-r--r--   0        0        0      809 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
--rw-r--r--   0        0        0      247 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
--rw-r--r--   0        0        0      856 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
--rw-r--r--   0        0        0      831 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
--rw-r--r--   0        0        0      827 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
--rw-r--r--   0        0        0      802 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
--rw-r--r--   0        0        0      819 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
--rw-r--r--   0        0        0      794 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
--rw-r--r--   0        0        0      795 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
--rw-r--r--   0        0        0      770 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
--rw-r--r--   0        0        0      706 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
--rw-r--r--   0        0        0     1184 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
--rw-r--r--   0        0        0     1554 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
--rw-r--r--   0        0        0      515 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
--rw-r--r--   0        0        0     1304 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
--rw-r--r--   0        0        0    15788 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
--rw-r--r--   0        0        0    16516 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
--rw-r--r--   0        0        0      428 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
--rw-r--r--   0        0        0    16514 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
--rw-r--r--   0        0        0     1367 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
--rw-r--r--   0        0        0      209 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      244 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      303 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
--rw-r--r--   0        0        0     1185 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
--rw-r--r--   0        0        0     1555 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
--rw-r--r--   0        0        0      275 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
--rw-r--r--   0        0        0      349 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
--rw-r--r--   0        0        0      148 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
--rw-r--r--   0        0        0    21027 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
--rw-r--r--   0        0        0      416 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
--rw-r--r--   0        0        0      363 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
--rw-r--r--   0        0        0      361 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
--rw-r--r--   0        0        0      548 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
--rw-r--r--   0        0        0    20390 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
--rw-r--r--   0        0        0    24278 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
--rw-r--r--   0        0        0     2163 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
--rw-r--r--   0        0        0     1897 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
--rw-r--r--   0        0        0     1342 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
--rw-r--r--   0        0        0     1346 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
--rw-r--r--   0        0        0      892 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
--rw-r--r--   0        0        0     1223 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
--rw-r--r--   0        0        0      693 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
--rw-r--r--   0        0        0      824 2024-05-06 13:40:25.284526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
--rw-r--r--   0        0        0      161 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
--rw-r--r--   0        0        0      187 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
--rw-r--r--   0        0        0    22340 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
--rw-r--r--   0        0        0     1211 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
--rw-r--r--   0        0        0     1215 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
--rw-r--r--   0        0        0      440 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
--rw-r--r--   0        0        0     1227 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
--rw-r--r--   0        0        0      333 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
--rw-r--r--   0        0        0      417 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
--rw-r--r--   0        0        0      468 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
--rw-r--r--   0        0        0      224 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
--rw-r--r--   0        0        0      254 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
--rw-r--r--   0        0        0      605 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
--rw-r--r--   0        0        0      253 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
--rw-r--r--   0        0        0      318 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
--rw-r--r--   0        0        0     2465 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
--rw-r--r--   0        0        0     3337 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
--rw-r--r--   0        0        0    21122 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
--rw-r--r--   0        0        0     2308 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json
--rw-r--r--   0        0        0     2693 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
--rw-r--r--   0        0        0      419 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
--rw-r--r--   0        0        0      495 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
--rw-r--r--   0        0        0    11181 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
--rw-r--r--   0        0        0      165 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
--rw-r--r--   0        0        0      560 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
--rw-r--r--   0        0        0      385 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
--rw-r--r--   0        0        0      433 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
--rw-r--r--   0        0        0      249 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
--rw-r--r--   0        0        0      314 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
--rw-r--r--   0        0        0      667 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
--rw-r--r--   0        0        0      809 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
--rw-r--r--   0        0        0      197 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
--rw-r--r--   0        0        0      247 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
--rw-r--r--   0        0        0      856 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
--rw-r--r--   0        0        0      831 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
--rw-r--r--   0        0        0      827 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
--rw-r--r--   0        0        0      802 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
--rw-r--r--   0        0        0      819 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
--rw-r--r--   0        0        0      794 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
--rw-r--r--   0        0        0      795 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
--rw-r--r--   0        0        0      770 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
--rw-r--r--   0        0        0      706 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
--rw-r--r--   0        0        0     1184 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
--rw-r--r--   0        0        0     1554 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
--rw-r--r--   0        0        0      515 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
--rw-r--r--   0        0        0     1304 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
--rw-r--r--   0        0        0    15788 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
--rw-r--r--   0        0        0    16516 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
--rw-r--r--   0        0        0      428 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
--rw-r--r--   0        0        0    16514 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
--rw-r--r--   0        0        0     1367 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
--rw-r--r--   0        0        0      277 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
--rw-r--r--   0        0        0      319 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      209 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      244 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      228 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
--rw-r--r--   0        0        0      303 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
--rw-r--r--   0        0        0     1185 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
--rw-r--r--   0        0        0     1555 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
--rw-r--r--   0        0        0      275 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
--rw-r--r--   0        0        0      349 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
--rw-r--r--   0        0        0      148 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
--rw-r--r--   0        0        0    21027 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
--rw-r--r--   0        0        0      416 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
--rw-r--r--   0        0        0      548 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
--rw-r--r--   0        0        0    20390 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
--rw-r--r--   0        0        0    24278 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
--rw-r--r--   0        0        0     2163 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
--rw-r--r--   0        0        0     1897 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
--rw-r--r--   0        0        0     1342 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
--rw-r--r--   0        0        0     1346 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
--rw-r--r--   0        0        0      892 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
--rw-r--r--   0        0        0     1223 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
--rw-r--r--   0        0        0     1497 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
--rw-r--r--   0        0        0     1983 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
--rw-r--r--   0        0        0      693 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
--rw-r--r--   0        0        0      824 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
--rw-r--r--   0        0        0      161 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
--rw-r--r--   0        0        0      187 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
--rw-r--r--   0        0        0     1384 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
--rw-r--r--   0        0        0     1596 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
--rw-r--r--   0        0        0    22340 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
--rw-r--r--   0        0        0     1117 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
--rw-r--r--   0        0        0     1324 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.288526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
--rw-r--r--   0        0        0     1211 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
--rw-r--r--   0        0        0     1215 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
--rw-r--r--   0        0        0      440 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
--rw-r--r--   0        0        0     1227 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
--rw-r--r--   0        0        0      333 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
--rw-r--r--   0        0        0      279 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
--rw-r--r--   0        0        0      321 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
--rw-r--r--   0        0        0      417 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
--rw-r--r--   0        0        0      468 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
--rw-r--r--   0        0        0      224 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
--rw-r--r--   0        0        0      254 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
--rw-r--r--   0        0        0      605 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
--rw-r--r--   0        0        0      253 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
--rw-r--r--   0        0        0      318 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
--rw-r--r--   0        0        0     2465 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
--rw-r--r--   0        0        0     3337 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
--rw-r--r--   0        0        0      983 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
--rw-r--r--   0        0        0     1213 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
--rw-r--r--   0        0        0    21122 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
--rw-r--r--   0        0        0     2308 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json
--rw-r--r--   0        0        0     2693 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
--rw-r--r--   0        0        0      419 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
--rw-r--r--   0        0        0      495 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
--rw-r--r--   0        0        0    11181 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
--rw-r--r--   0        0        0      165 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
--rw-r--r--   0        0        0      560 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
--rw-r--r--   0        0        0      385 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
--rw-r--r--   0        0        0      433 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
--rw-r--r--   0        0        0      249 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
--rw-r--r--   0        0        0      314 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
--rw-r--r--   0        0        0      667 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
--rw-r--r--   0        0        0      809 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
--rw-r--r--   0        0        0      197 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
--rw-r--r--   0        0        0      247 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
--rw-r--r--   0        0        0      856 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
--rw-r--r--   0        0        0      831 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
--rw-r--r--   0        0        0      827 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
--rw-r--r--   0        0        0      802 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
--rw-r--r--   0        0        0      819 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
--rw-r--r--   0        0        0      794 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
--rw-r--r--   0        0        0      795 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
--rw-r--r--   0        0        0      770 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
--rw-r--r--   0        0        0      706 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
--rw-r--r--   0        0        0     1184 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
--rw-r--r--   0        0        0     1554 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
--rw-r--r--   0        0        0      515 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
--rw-r--r--   0        0        0     1304 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
--rw-r--r--   0        0        0    15788 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
--rw-r--r--   0        0        0    16516 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
--rw-r--r--   0        0        0      428 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
--rw-r--r--   0        0        0    16514 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
--rw-r--r--   0        0        0     1367 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
--rw-r--r--   0        0        0      277 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
--rw-r--r--   0        0        0      319 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      209 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      244 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      228 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
--rw-r--r--   0        0        0      303 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
--rw-r--r--   0        0        0     1185 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
--rw-r--r--   0        0        0     1555 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
--rw-r--r--   0        0        0      275 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
--rw-r--r--   0        0        0      349 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
--rw-r--r--   0        0        0      148 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
--rw-r--r--   0        0        0    21027 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
--rw-r--r--   0        0        0      416 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
--rw-r--r--   0        0        0      548 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
--rw-r--r--   0        0        0    20390 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
--rw-r--r--   0        0        0    24278 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
--rw-r--r--   0        0        0     2163 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
--rw-r--r--   0        0        0     1897 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
--rw-r--r--   0        0        0     1342 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
--rw-r--r--   0        0        0     1346 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
--rw-r--r--   0        0        0      892 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
--rw-r--r--   0        0        0     1223 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
--rw-r--r--   0        0        0     1497 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
--rw-r--r--   0        0        0     1983 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
--rw-r--r--   0        0        0      693 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
--rw-r--r--   0        0        0      824 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
--rw-r--r--   0        0        0      161 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
--rw-r--r--   0        0        0      187 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
--rw-r--r--   0        0        0     1384 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
--rw-r--r--   0        0        0     1596 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
--rw-r--r--   0        0        0    22340 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
--rw-r--r--   0        0        0     1117 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
--rw-r--r--   0        0        0     1324 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
--rw-r--r--   0        0        0     1211 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
--rw-r--r--   0        0        0     1215 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
--rw-r--r--   0        0        0      440 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
--rw-r--r--   0        0        0     1227 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
--rw-r--r--   0        0        0      333 2024-05-06 13:40:25.292526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
--rw-r--r--   0        0        0      279 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
--rw-r--r--   0        0        0      321 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
--rw-r--r--   0        0        0      438 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
--rw-r--r--   0        0        0      417 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
--rw-r--r--   0        0        0      468 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
--rw-r--r--   0        0        0      224 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
--rw-r--r--   0        0        0      254 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
--rw-r--r--   0        0        0      605 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
--rw-r--r--   0        0        0      227 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
--rw-r--r--   0        0        0      281 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
--rw-r--r--   0        0        0     2465 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
--rw-r--r--   0        0        0     3337 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
--rw-r--r--   0        0        0      983 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
--rw-r--r--   0        0        0     1213 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
--rw-r--r--   0        0        0    21122 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
--rw-r--r--   0        0        0     5338 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
--rw-r--r--   0        0        0     6828 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
--rw-r--r--   0        0        0     2312 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json
--rw-r--r--   0        0        0     2693 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
--rw-r--r--   0        0        0      419 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
--rw-r--r--   0        0        0      495 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
--rw-r--r--   0        0        0     9733 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
--rw-r--r--   0        0        0     4274 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
--rw-r--r--   0        0        0     5987 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
--rw-r--r--   0        0        0    11181 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
--rw-r--r--   0        0        0      165 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
--rw-r--r--   0        0        0      508 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
--rw-r--r--   0        0        0      866 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
--rw-r--r--   0        0        0      385 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
--rw-r--r--   0        0        0      433 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
--rw-r--r--   0        0        0      249 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
--rw-r--r--   0        0        0      314 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
--rw-r--r--   0        0        0      746 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
--rw-r--r--   0        0        0     1086 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
--rw-r--r--   0        0        0      197 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
--rw-r--r--   0        0        0      247 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
--rw-r--r--   0        0        0      856 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
--rw-r--r--   0        0        0      831 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
--rw-r--r--   0        0        0      827 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
--rw-r--r--   0        0        0      802 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
--rw-r--r--   0        0        0      819 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
--rw-r--r--   0        0        0      794 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
--rw-r--r--   0        0        0      795 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
--rw-r--r--   0        0        0      770 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
--rw-r--r--   0        0        0      706 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
--rw-r--r--   0        0        0     1184 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
--rw-r--r--   0        0        0     1554 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
--rw-r--r--   0        0        0      515 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
--rw-r--r--   0        0        0     1304 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
--rw-r--r--   0        0        0    15788 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
--rw-r--r--   0        0        0    16516 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
--rw-r--r--   0        0        0      428 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
--rw-r--r--   0        0        0    16514 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
--rw-r--r--   0        0        0     1367 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
--rw-r--r--   0        0        0      277 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
--rw-r--r--   0        0        0      319 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      209 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      244 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0      228 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
--rw-r--r--   0        0        0      303 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
--rw-r--r--   0        0        0     1185 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
--rw-r--r--   0        0        0     1555 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
--rw-r--r--   0        0        0      275 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
--rw-r--r--   0        0        0      349 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
--rw-r--r--   0        0        0      148 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
--rw-r--r--   0        0        0    21027 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
--rw-r--r--   0        0        0      416 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
--rw-r--r--   0        0        0     2527 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
--rw-r--r--   0        0        0     3596 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
--rw-r--r--   0        0        0      548 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
--rw-r--r--   0        0        0    20390 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
--rw-r--r--   0        0        0    24278 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
--rw-r--r--   0        0        0     2163 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
--rw-r--r--   0        0        0     1897 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
--rw-r--r--   0        0        0     1342 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
--rw-r--r--   0        0        0     1346 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
--rw-r--r--   0        0        0      892 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
--rw-r--r--   0        0        0     1223 2024-05-06 13:40:25.296526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
--rw-r--r--   0        0        0     1810 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
--rw-r--r--   0        0        0     2449 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
--rw-r--r--   0        0        0      693 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
--rw-r--r--   0        0        0      824 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
--rw-r--r--   0        0        0      161 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
--rw-r--r--   0        0        0      187 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
--rw-r--r--   0        0        0     3189 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
--rw-r--r--   0        0        0     4519 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
--rw-r--r--   0        0        0    22340 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
--rw-r--r--   0        0        0     1117 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
--rw-r--r--   0        0        0     1324 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
--rw-r--r--   0        0        0     7703 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
--rw-r--r--   0        0        0    11757 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
--rw-r--r--   0        0        0      473 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
--rw-r--r--   0        0        0     1270 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
--rw-r--r--   0        0        0      467 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
--rw-r--r--   0        0        0     1236 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
--rw-r--r--   0        0        0     1539 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
--rw-r--r--   0        0        0     2197 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
--rw-r--r--   0        0        0      477 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
--rw-r--r--   0        0        0     1248 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
--rw-r--r--   0        0        0    98548 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
--rw-r--r--   0        0        0   100112 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
--rw-r--r--   0        0        0      333 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
--rw-r--r--   0        0        0      279 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
--rw-r--r--   0        0        0      321 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
--rw-r--r--   0        0        0      436 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
--rw-r--r--   0        0        0      624 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
--rw-r--r--   0        0        0      507 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
--rw-r--r--   0        0        0      537 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
--rw-r--r--   0        0        0      482 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
--rw-r--r--   0        0        0      509 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
--rw-r--r--   0        0        0      224 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
--rw-r--r--   0        0        0      254 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
--rw-r--r--   0        0        0     1162 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
--rw-r--r--   0        0        0     1471 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
--rw-r--r--   0        0        0      605 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
--rw-r--r--   0        0        0      227 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
--rw-r--r--   0        0        0      281 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
--rw-r--r--   0        0        0     2465 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
--rw-r--r--   0        0        0     3337 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
--rw-r--r--   0        0        0     1520 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
--rw-r--r--   0        0        0     1660 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
--rw-r--r--   0        0        0    21122 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
--rw-r--r--   0        0        0     5338 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
--rw-r--r--   0        0        0     6828 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
--rw-r--r--   0        0        0     9412 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
--rw-r--r--   0        0        0    12249 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
--rw-r--r--   0        0        0     2312 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json
--rw-r--r--   0        0        0     2693 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
--rw-r--r--   0        0        0      419 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
--rw-r--r--   0        0        0      495 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
--rw-r--r--   0        0        0     9733 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
--rw-r--r--   0        0        0    17746 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
--rw-r--r--   0        0        0    19794 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
--rw-r--r--   0        0        0    11181 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
--rw-r--r--   0        0        0      165 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
--rw-r--r--   0        0        0      508 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
--rw-r--r--   0        0        0      866 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
--rw-r--r--   0        0        0      385 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
--rw-r--r--   0        0        0      433 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
--rw-r--r--   0        0        0      249 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
--rw-r--r--   0        0        0      314 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
--rw-r--r--   0        0        0      746 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
--rw-r--r--   0        0        0     1086 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
--rw-r--r--   0        0        0      197 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
--rw-r--r--   0        0        0      247 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
--rw-r--r--   0        0        0      856 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
--rw-r--r--   0        0        0      831 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
--rw-r--r--   0        0        0      827 2024-05-06 13:40:25.300526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
--rw-r--r--   0        0        0      802 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
--rw-r--r--   0        0        0      819 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
--rw-r--r--   0        0        0      794 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
--rw-r--r--   0        0        0      795 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
--rw-r--r--   0        0        0      770 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
--rw-r--r--   0        0        0      731 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
--rw-r--r--   0        0        0      706 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
--rw-r--r--   0        0        0     1184 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
--rw-r--r--   0        0        0     1554 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
--rw-r--r--   0        0        0      515 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
--rw-r--r--   0        0        0     1304 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
--rw-r--r--   0        0        0    15788 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
--rw-r--r--   0        0        0    16516 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
--rw-r--r--   0        0        0      428 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
--rw-r--r--   0        0        0    16514 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
--rw-r--r--   0        0        0     1329 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
--rw-r--r--   0        0        0      360 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
--rw-r--r--   0        0        0      466 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
--rw-r--r--   0        0        0     1367 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
--rw-r--r--   0        0        0      277 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
--rw-r--r--   0        0        0      319 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      209 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      244 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0      228 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
--rw-r--r--   0        0        0      303 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
--rw-r--r--   0        0        0    21039 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
--rw-r--r--   0        0        0     1185 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
--rw-r--r--   0        0        0     1555 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
--rw-r--r--   0        0        0     1290 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
--rw-r--r--   0        0        0     1504 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
--rw-r--r--   0        0        0      275 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
--rw-r--r--   0        0        0      349 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
--rw-r--r--   0        0        0      148 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
--rw-r--r--   0        0        0    21027 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
--rw-r--r--   0        0        0      416 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
--rw-r--r--   0        0        0     2527 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
--rw-r--r--   0        0        0     3596 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
--rw-r--r--   0        0        0      548 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
--rw-r--r--   0        0        0     5654 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
--rw-r--r--   0        0        0     7084 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
--rw-r--r--   0        0        0     6538 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
--rw-r--r--   0        0        0    24921 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
--rw-r--r--   0        0        0     2163 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
--rw-r--r--   0        0        0     1897 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
--rw-r--r--   0        0        0      750 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
--rw-r--r--   0        0        0      865 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
--rw-r--r--   0        0        0      394 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
--rw-r--r--   0        0        0      705 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
--rw-r--r--   0        0        0      492 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
--rw-r--r--   0        0        0     1342 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
--rw-r--r--   0        0        0     1346 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
--rw-r--r--   0        0        0      892 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
--rw-r--r--   0        0        0     1223 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
--rw-r--r--   0        0        0     1810 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
--rw-r--r--   0        0        0     2449 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
--rw-r--r--   0        0        0     2978 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
--rw-r--r--   0        0        0     4629 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
--rw-r--r--   0        0        0     1459 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
--rw-r--r--   0        0        0     2217 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
--rw-r--r--   0        0        0      693 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
--rw-r--r--   0        0        0      824 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
--rw-r--r--   0        0        0      161 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
--rw-r--r--   0        0        0      187 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
--rw-r--r--   0        0        0     4432 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
--rw-r--r--   0        0        0     6383 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
--rw-r--r--   0        0        0    22340 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
--rw-r--r--   0        0        0     1117 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
--rw-r--r--   0        0        0     1324 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
--rw-r--r--   0        0        0     7703 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
--rw-r--r--   0        0        0    11757 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
--rw-r--r--   0        0        0      514 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
--rw-r--r--   0        0        0     1297 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
--rw-r--r--   0        0        0      510 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
--rw-r--r--   0        0        0     1263 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
--rw-r--r--   0        0        0     1539 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
--rw-r--r--   0        0        0     2197 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
--rw-r--r--   0        0        0      477 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
--rw-r--r--   0        0        0     1248 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
--rw-r--r--   0        0        0    98548 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
--rw-r--r--   0        0        0   100112 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
--rw-r--r--   0        0        0     1835 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
--rw-r--r--   0        0        0     2811 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
--rw-r--r--   0        0        0      333 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
--rw-r--r--   0        0        0      430 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
--rw-r--r--   0        0        0      432 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
--rw-r--r--   0        0        0      456 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
--rw-r--r--   0        0        0      436 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
--rw-r--r--   0        0        0      624 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
--rw-r--r--   0        0        0      521 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
--rw-r--r--   0        0        0      551 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
--rw-r--r--   0        0        0      508 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
--rw-r--r--   0        0        0      539 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
--rw-r--r--   0        0        0      482 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
--rw-r--r--   0        0        0      509 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
--rw-r--r--   0        0        0      224 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
--rw-r--r--   0        0        0      254 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
--rw-r--r--   0        0        0     1162 2024-05-06 13:40:25.304526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
--rw-r--r--   0        0        0     1471 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
--rw-r--r--   0        0        0      605 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
--rw-r--r--   0        0        0      227 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
--rw-r--r--   0        0        0      281 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
--rw-r--r--   0        0        0     2465 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
--rw-r--r--   0        0        0     3337 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
--rw-r--r--   0        0        0     1894 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
--rw-r--r--   0        0        0     1872 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
--rw-r--r--   0        0        0    21122 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
--rw-r--r--   0        0        0     5338 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
--rw-r--r--   0        0        0     6828 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
--rw-r--r--   0        0        0     9412 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
--rw-r--r--   0        0        0    12249 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
--rw-r--r--   0        0        0     2312 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-1.6.json
--rw-r--r--   0        0        0     2693 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
--rw-r--r--   0        0        0      419 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
--rw-r--r--   0        0        0      495 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
--rw-r--r--   0        0        0     9733 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
--rw-r--r--   0        0        0     1902 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
--rw-r--r--   0        0        0     2747 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
--rw-r--r--   0        0        0      491 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
--rw-r--r--   0        0        0      870 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
--rw-r--r--   0        0        0    17746 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
--rw-r--r--   0        0        0    19794 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
--rw-r--r--   0        0        0    11181 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
--rw-r--r--   0        0        0      157 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/README.md
--rwxr-xr-x   0        0        0      745 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/fetch.sh
--rw-r--r--   0        0        0      391 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/README.md
--rw-r--r--   0        0        0      579 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
--rw-r--r--   0        0        0      649 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
--rw-r--r--   0        0        0     1050 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
--rw-r--r--   0        0        0     1055 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
--rw-r--r--   0        0        0     1050 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
--rw-r--r--   0        0        0     1055 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
--rw-r--r--   0        0        0     2128 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
--rw-r--r--   0        0        0     2211 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
--rw-r--r--   0        0        0     2264 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
--rw-r--r--   0        0        0     2326 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
--rw-r--r--   0        0        0     2264 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
--rw-r--r--   0        0        0     2326 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
--rw-r--r--   0        0        0      806 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
--rw-r--r--   0        0        0      949 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
--rw-r--r--   0        0        0     1835 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
--rw-r--r--   0        0        0     1806 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
--rw-r--r--   0        0        0     1835 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
--rw-r--r--   0        0        0     1806 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
--rw-r--r--   0        0        0     2808 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
--rw-r--r--   0        0        0     2877 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
--rw-r--r--   0        0        0     3596 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
--rw-r--r--   0        0        0     3640 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
--rw-r--r--   0        0        0     3788 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
--rw-r--r--   0        0        0     3831 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
--rw-r--r--   0        0        0      944 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
--rw-r--r--   0        0        0      865 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
--rw-r--r--   0        0        0      944 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
--rw-r--r--   0        0        0      865 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
--rw-r--r--   0        0        0     2085 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
--rw-r--r--   0        0        0     2072 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
--rw-r--r--   0        0        0     2221 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
--rw-r--r--   0        0        0     2187 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
--rw-r--r--   0        0        0     2221 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
--rw-r--r--   0        0        0     2187 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
--rw-r--r--   0        0        0      496 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
--rw-r--r--   0        0        0      893 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin
--rw-r--r--   0        0        0      812 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
--rw-r--r--   0        0        0      893 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin
--rw-r--r--   0        0        0      812 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
--rw-r--r--   0        0        0     2013 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin
--rw-r--r--   0        0        0     2002 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
--rw-r--r--   0        0        0     2149 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin
--rw-r--r--   0        0        0     2117 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
--rw-r--r--   0        0        0     2149 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.6.json.bin
--rw-r--r--   0        0        0     2117 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
--rw-r--r--   0        0        0     4485 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
--rw-r--r--   0        0        0     4434 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
--rw-r--r--   0        0        0     4801 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
--rw-r--r--   0        0        0     4434 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
--rw-r--r--   0        0        0     4801 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
--rw-r--r--   0        0        0     5562 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
--rw-r--r--   0        0        0     5999 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
--rw-r--r--   0        0        0     5947 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
--rw-r--r--   0        0        0     6363 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
--rw-r--r--   0        0        0     5991 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
--rw-r--r--   0        0        0     6407 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
--rw-r--r--   0        0        0      749 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
--rw-r--r--   0        0        0      793 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
--rw-r--r--   0        0        0     1894 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
--rw-r--r--   0        0        0     1461 2024-05-06 13:40:25.308526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
--rw-r--r--   0        0        0     1894 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
--rw-r--r--   0        0        0     1461 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
--rw-r--r--   0        0        0     3014 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
--rw-r--r--   0        0        0     2651 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
--rw-r--r--   0        0        0     3150 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
--rw-r--r--   0        0        0     2766 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
--rw-r--r--   0        0        0     3150 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
--rw-r--r--   0        0        0     2766 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
--rw-r--r--   0        0        0     2092 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
--rw-r--r--   0        0        0     2289 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
--rw-r--r--   0        0        0     2228 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
--rw-r--r--   0        0        0     2404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
--rw-r--r--   0        0        0     2228 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
--rw-r--r--   0        0        0     2404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
--rw-r--r--   0        0        0     3282 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
--rw-r--r--   0        0        0     3686 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
--rw-r--r--   0        0        0     3418 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
--rw-r--r--   0        0        0     3801 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
--rw-r--r--   0        0        0     3418 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
--rw-r--r--   0        0        0     3801 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
--rw-r--r--   0        0        0     1827 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
--rw-r--r--   0        0        0     2023 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
--rw-r--r--   0        0        0     1963 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
--rw-r--r--   0        0        0     2138 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
--rw-r--r--   0        0        0     1963 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
--rw-r--r--   0        0        0     2138 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
--rw-r--r--   0        0        0     2577 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
--rw-r--r--   0        0        0     2822 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
--rw-r--r--   0        0        0     2713 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
--rw-r--r--   0        0        0     2937 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
--rw-r--r--   0        0        0     2713 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
--rw-r--r--   0        0        0     2937 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
--rw-r--r--   0        0        0     1081 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
--rw-r--r--   0        0        0     1083 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
--rw-r--r--   0        0        0     1081 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
--rw-r--r--   0        0        0     1083 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2201 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
--rw-r--r--   0        0        0     2273 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2337 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
--rw-r--r--   0        0        0     2388 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2337 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
--rw-r--r--   0        0        0     2388 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
--rw-r--r--   0        0        0      308 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
--rw-r--r--   0        0        0      886 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
--rw-r--r--   0        0        0      821 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
--rw-r--r--   0        0        0      886 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
--rw-r--r--   0        0        0      821 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
--rw-r--r--   0        0        0     2006 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
--rw-r--r--   0        0        0     2011 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
--rw-r--r--   0        0        0     2142 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
--rw-r--r--   0        0        0     2126 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
--rw-r--r--   0        0        0     2142 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
--rw-r--r--   0        0        0     2126 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
--rw-r--r--   0        0        0     2014 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
--rw-r--r--   0        0        0     2243 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
--rw-r--r--   0        0        0     2150 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
--rw-r--r--   0        0        0     2358 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
--rw-r--r--   0        0        0     2150 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
--rw-r--r--   0        0        0     2358 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
--rw-r--r--   0        0        0      413 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
--rw-r--r--   0        0        0      404 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
--rw-r--r--   0        0        0     2025 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
--rw-r--r--   0        0        0     2268 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
--rw-r--r--   0        0        0     2161 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
--rw-r--r--   0        0        0     2383 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
--rw-r--r--   0        0        0     2161 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
--rw-r--r--   0        0        0     2383 2024-05-06 13:40:25.312526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
--rw-r--r--   0        0        0      596 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
--rw-r--r--   0        0        0      695 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
--rw-r--r--   0        0        0     1561 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
--rw-r--r--   0        0        0     1597 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
--rw-r--r--   0        0        0     1561 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
--rw-r--r--   0        0        0     1597 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
--rw-r--r--   0        0        0     2702 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
--rw-r--r--   0        0        0     2804 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
--rw-r--r--   0        0        0     2838 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
--rw-r--r--   0        0        0     2919 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
--rw-r--r--   0        0        0     2838 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
--rw-r--r--   0        0        0     2919 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
--rw-r--r--   0        0        0      662 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
--rw-r--r--   0        0        0      678 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
--rw-r--r--   0        0        0     1385 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
--rw-r--r--   0        0        0     1402 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
--rw-r--r--   0        0        0     1385 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
--rw-r--r--   0        0        0     1402 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
--rw-r--r--   0        0        0     2526 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
--rw-r--r--   0        0        0     2609 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
--rw-r--r--   0        0        0     2662 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
--rw-r--r--   0        0        0     2724 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
--rw-r--r--   0        0        0     2662 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
--rw-r--r--   0        0        0     2724 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
--rw-r--r--   0        0        0      246 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
--rw-r--r--   0        0        0      847 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
--rw-r--r--   0        0        0     1085 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
--rw-r--r--   0        0        0     1163 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
--rw-r--r--   0        0        0     1085 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
--rw-r--r--   0        0        0     1163 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
--rw-r--r--   0        0        0     2205 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
--rw-r--r--   0        0        0     2353 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
--rw-r--r--   0        0        0     2341 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
--rw-r--r--   0        0        0     2468 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
--rw-r--r--   0        0        0     2341 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
--rw-r--r--   0        0        0     2468 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
--rw-r--r--   0        0        0      581 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.0.xml.bin
--rw-r--r--   0        0        0      612 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.1.xml.bin
--rw-r--r--   0        0        0      939 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.json.bin
--rw-r--r--   0        0        0      962 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.xml.bin
--rw-r--r--   0        0        0      939 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.json.bin
--rw-r--r--   0        0        0      962 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.xml.bin
--rw-r--r--   0        0        0     2080 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.json.bin
--rw-r--r--   0        0        0     2169 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.xml.bin
--rw-r--r--   0        0        0     2216 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.json.bin
--rw-r--r--   0        0        0     2284 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.xml.bin
--rw-r--r--   0        0        0     2216 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.json.bin
--rw-r--r--   0        0        0     2284 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
--rw-r--r--   0        0        0     8540 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
--rw-r--r--   0        0        0     8315 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
--rw-r--r--   0        0        0    10266 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
--rw-r--r--   0        0        0     9628 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
--rw-r--r--   0        0        0    13173 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
--rw-r--r--   0        0        0    12575 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
--rw-r--r--   0        0        0    13309 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
--rw-r--r--   0        0        0    12690 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
--rw-r--r--   0        0        0    14474 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
--rw-r--r--   0        0        0    14004 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0     2739 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
--rw-r--r--   0        0        0     3108 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
--rw-r--r--   0        0        0     2449 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
--rw-r--r--   0        0        0     2636 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
--rw-r--r--   0        0        0     3086 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
--rw-r--r--   0        0        0     3518 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
--rw-r--r--   0        0        0     2634 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
--rw-r--r--   0        0        0     2831 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
--rw-r--r--   0        0        0     2164 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
--rw-r--r--   0        0        0     2217 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
--rw-r--r--   0        0        0     2164 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
--rw-r--r--   0        0        0     2217 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
--rw-r--r--   0        0        0     1199 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
--rw-r--r--   0        0        0     4993 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
--rw-r--r--   0        0        0     7631 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
--rw-r--r--   0        0        0     7396 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
--rw-r--r--   0        0        0     8830 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
--rw-r--r--   0        0        0     8293 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
--rw-r--r--   0        0        0    11737 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
--rw-r--r--   0        0        0    11240 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
--rw-r--r--   0        0        0    11873 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
--rw-r--r--   0        0        0    11355 2024-05-06 13:40:25.316526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
--rw-r--r--   0        0        0    12042 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
--rw-r--r--   0        0        0    11556 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
--rw-r--r--   0        0        0      307 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
--rw-r--r--   0        0        0      477 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
--rw-r--r--   0        0        0      860 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
--rw-r--r--   0        0        0      859 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
--rw-r--r--   0        0        0      860 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
--rw-r--r--   0        0        0      859 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
--rw-r--r--   0        0        0     1980 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
--rw-r--r--   0        0        0     2049 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
--rw-r--r--   0        0        0     2116 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
--rw-r--r--   0        0        0     2164 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
--rw-r--r--   0        0        0     2116 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
--rw-r--r--   0        0        0     2164 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
--rw-r--r--   0        0        0      395 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
--rw-r--r--   0        0        0      572 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
--rw-r--r--   0        0        0      952 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
--rw-r--r--   0        0        0      961 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
--rw-r--r--   0        0        0      952 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
--rw-r--r--   0        0        0      961 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
--rw-r--r--   0        0        0     2093 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
--rw-r--r--   0        0        0     2168 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
--rw-r--r--   0        0        0     2229 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
--rw-r--r--   0        0        0     2283 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
--rw-r--r--   0        0        0     2229 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
--rw-r--r--   0        0        0     2283 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
--rw-r--r--   0        0        0     3848 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
--rw-r--r--   0        0        0     3888 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
--rw-r--r--   0        0        0     3984 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
--rw-r--r--   0        0        0     4003 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
--rw-r--r--   0        0        0     3984 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
--rw-r--r--   0        0        0     4003 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
--rw-r--r--   0        0        0     2028 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
--rw-r--r--   0        0        0     2102 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
--rw-r--r--   0        0        0     2164 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
--rw-r--r--   0        0        0     2217 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
--rw-r--r--   0        0        0     3918 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
--rw-r--r--   0        0        0     4052 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
--rw-r--r--   0        0        0      329 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
--rw-r--r--   0        0        0      506 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
--rw-r--r--   0        0        0      887 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
--rw-r--r--   0        0        0      895 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
--rw-r--r--   0        0        0     5189 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
--rw-r--r--   0        0        0     5704 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
--rw-r--r--   0        0        0     5325 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
--rw-r--r--   0        0        0     5819 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
--rw-r--r--   0        0        0     5518 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
--rw-r--r--   0        0        0     6044 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
--rw-r--r--   0        0        0     1056 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
--rw-r--r--   0        0        0     1071 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
--rw-r--r--   0        0        0     1243 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
--rw-r--r--   0        0        0     1214 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
--rw-r--r--   0        0        0     2384 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
--rw-r--r--   0        0        0     2421 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
--rw-r--r--   0        0        0     2520 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
--rw-r--r--   0        0        0     2536 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
--rw-r--r--   0        0        0     2520 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
--rw-r--r--   0        0        0     2536 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
--rw-r--r--   0        0        0     2950 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
--rw-r--r--   0        0        0     3403 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
--rw-r--r--   0        0        0      655 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
--rw-r--r--   0        0        0      980 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
--rw-r--r--   0        0        0     1582 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
--rw-r--r--   0        0        0     1579 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
--rw-r--r--   0        0        0     1769 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
--rw-r--r--   0        0        0     1722 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
--rw-r--r--   0        0        0     2889 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
--rw-r--r--   0        0        0     2912 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
--rw-r--r--   0        0        0     3025 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
--rw-r--r--   0        0        0     3027 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
--rw-r--r--   0        0        0     3025 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
--rw-r--r--   0        0        0     3027 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
--rw-r--r--   0        0        0      654 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
--rw-r--r--   0        0        0     1045 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
--rw-r--r--   0        0        0     1562 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
--rw-r--r--   0        0        0     1749 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
--rw-r--r--   0        0        0     2890 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
--rw-r--r--   0        0        0     3026 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
--rw-r--r--   0        0        0     3042 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
--rw-r--r--   0        0        0     3026 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
--rw-r--r--   0        0        0     3042 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
--rw-r--r--   0        0        0      431 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
--rw-r--r--   0        0        0      629 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
--rw-r--r--   0        0        0      666 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
--rw-r--r--   0        0        0      792 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
--rw-r--r--   0        0        0      797 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
--rw-r--r--   0        0        0     1933 2024-05-06 13:40:25.320526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
--rw-r--r--   0        0        0     2004 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
--rw-r--r--   0        0        0     2069 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
--rw-r--r--   0        0        0     2119 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
--rw-r--r--   0        0        0     2069 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
--rw-r--r--   0        0        0     2119 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
--rw-r--r--   0        0        0      516 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
--rw-r--r--   0        0        0     1123 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     3019 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
--rw-r--r--   0        0        0     2676 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     3119 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
--rw-r--r--   0        0        0     2767 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     4176 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
--rw-r--r--   0        0        0     3906 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     4312 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
--rw-r--r--   0        0        0     4021 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     4482 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
--rw-r--r--   0        0        0     4131 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      448 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
--rw-r--r--   0        0        0      723 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
--rw-r--r--   0        0        0     1575 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
--rw-r--r--   0        0        0     1577 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
--rw-r--r--   0        0        0     1762 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
--rw-r--r--   0        0        0     1720 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
--rw-r--r--   0        0        0     2903 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
--rw-r--r--   0        0        0     2927 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
--rw-r--r--   0        0        0     3039 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
--rw-r--r--   0        0        0     3042 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
--rw-r--r--   0        0        0     3039 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
--rw-r--r--   0        0        0     3042 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
--rw-r--r--   0        0        0      245 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
--rw-r--r--   0        0        0      459 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
--rw-r--r--   0        0        0     1475 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
--rw-r--r--   0        0        0     1382 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
--rw-r--r--   0        0        0     1649 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
--rw-r--r--   0        0        0     1533 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
--rw-r--r--   0        0        0     2748 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
--rw-r--r--   0        0        0     2706 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
--rw-r--r--   0        0        0     2884 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
--rw-r--r--   0        0        0     2821 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
--rw-r--r--   0        0        0     2884 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
--rw-r--r--   0        0        0     2821 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
--rw-r--r--   0        0        0     3900 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
--rw-r--r--   0        0        0     4021 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
--rw-r--r--   0        0        0     4263 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
--rw-r--r--   0        0        0     4295 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
--rw-r--r--   0        0        0     7224 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
--rw-r--r--   0        0        0     7288 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
--rw-r--r--   0        0        0     7360 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
--rw-r--r--   0        0        0     7403 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
--rw-r--r--   0        0        0     7915 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
--rw-r--r--   0        0        0     8054 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
--rw-r--r--   0        0        0     2106 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
--rw-r--r--   0        0        0     2196 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
--rw-r--r--   0        0        0     2469 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
--rw-r--r--   0        0        0     2470 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
--rw-r--r--   0        0        0     5430 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
--rw-r--r--   0        0        0     5463 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
--rw-r--r--   0        0        0     5566 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
--rw-r--r--   0        0        0     5578 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
--rw-r--r--   0        0        0     5735 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
--rw-r--r--   0        0        0     5779 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
--rw-r--r--   0        0        0      108 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
--rw-r--r--   0        0        0      169 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
--rw-r--r--   0        0        0     1030 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
--rw-r--r--   0        0        0     1040 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
--rw-r--r--   0        0        0     1030 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
--rw-r--r--   0        0        0     1040 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
--rw-r--r--   0        0        0     2171 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
--rw-r--r--   0        0        0     2247 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
--rw-r--r--   0        0        0     2307 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
--rw-r--r--   0        0        0     2362 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
--rw-r--r--   0        0        0     2307 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
--rw-r--r--   0        0        0     2362 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
--rw-r--r--   0        0        0     2957 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_component.py
--rw-r--r--   0        0        0     3727 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_deserialize_json.py
--rw-r--r--   0        0        0     1764 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_deserialize_xml.py
--rw-r--r--   0        0        0    19038 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_enums.py
--rw-r--r--   0        0        0     5728 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_factory_license.py
--rw-r--r--   0        0        0    22602 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model.py
--rw-r--r--   0        0        0    13254 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_bom.py
--rw-r--r--   0        0        0     2782 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_bom_ref.py
--rw-r--r--   0        0        0    18544 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_component.py
--rw-r--r--   0        0        0     1793 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_dependency.py
--rw-r--r--   0        0        0     4064 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_issue.py
--rw-r--r--   0        0        0     4295 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_license.py
--rw-r--r--   0        0        0     2758 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_release_note.py
--rw-r--r--   0        0        0     3390 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_service.py
--rw-r--r--   0        0        0    14370 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_model_vulnerability.py
--rw-r--r--   0        0        0     3154 2024-05-06 13:40:25.324526 cyclonedx_python_lib-7.3.4/tests/test_output.py
--rw-r--r--   0        0        0     4587 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_output_json.py
--rw-r--r--   0        0        0     4029 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_output_xml.py
--rw-r--r--   0        0        0     1307 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_real_world_examples.py
--rw-r--r--   0        0        0     2509 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_schema_SchemaVersion.py
--rw-r--r--   0        0        0     1248 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_schema__res.py
--rw-r--r--   0        0        0     2873 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_spdx.py
--rw-r--r--   0        0        0     1977 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_validation.py
--rw-r--r--   0        0        0     4939 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_validation_json.py
--rw-r--r--   0        0        0     3414 2024-05-06 13:40:25.328526 cyclonedx_python_lib-7.3.4/tests/test_validation_xml.py
--rw-r--r--   0        0        0     6663 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.3.4/PKG-INFO
+-rw-r--r--   0        0        0   276291 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/LICENSE
+-rw-r--r--   0        0        0      147 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/NOTICE
+-rw-r--r--   0        0        0     4574 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/README.md
+-rw-r--r--   0        0        0      850 2024-05-23 05:42:46.196781 cyclonedx_python_lib-7.4.0/cyclonedx/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/_internal/__init__.py
+-rw-r--r--   0        0        0     3148 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/_internal/compare.py
+-rw-r--r--   0        0        0     1164 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/_internal/hash.py
+-rw-r--r--   0        0        0      847 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/_internal/time.py
+-rw-r--r--   0        0        0      993 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/exception/__init__.py
+-rw-r--r--   0        0        0     1536 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/exception/factory.py
+-rw-r--r--   0        0        0     3685 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/exception/model.py
+-rw-r--r--   0        0        0     1136 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/exception/output.py
+-rw-r--r--   0        0        0     1730 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/exception/serialization.py
+-rw-r--r--   0        0        0      680 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/factory/__init__.py
+-rw-r--r--   0        0        0     4191 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/factory/license.py
+-rw-r--r--   0        0        0    43540 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/model/__init__.py
+-rw-r--r--   0        0        0    26098 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/model/bom.py
+-rw-r--r--   0        0        0     2179 2024-05-23 05:42:26.404826 cyclonedx_python_lib-7.4.0/cyclonedx/model/bom_ref.py
+-rw-r--r--   0        0        0    59251 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/component.py
+-rw-r--r--   0        0        0    11793 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/contact.py
+-rw-r--r--   0        0        0    48270 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/crypto.py
+-rw-r--r--   0        0        0     3766 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/dependency.py
+-rw-r--r--   0        0        0     3568 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/impact_analysis.py
+-rw-r--r--   0        0        0     7024 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/issue.py
+-rw-r--r--   0        0        0    13070 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/license.py
+-rw-r--r--   0        0        0     8623 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/release_note.py
+-rw-r--r--   0        0        0    12798 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/service.py
+-rw-r--r--   0        0        0    43655 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/model/vulnerability.py
+-rw-r--r--   0        0        0     5872 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/output/__init__.py
+-rw-r--r--   0        0        0     4270 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/output/json.py
+-rw-r--r--   0        0        0     4285 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/output/xml.py
+-rw-r--r--   0        0        0      153 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/py.typed
+-rw-r--r--   0        0        0     3018 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/__init__.py
+-rw-r--r--   0        0        0     2114 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/README.md
+-rw-r--r--   0        0        0     2493 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/__init__.py
+-rw-r--r--   0        0        0    13604 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    39716 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    37110 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    36226 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    76383 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    40324 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    39348 2024-05-23 05:42:26.408826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    88794 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd
+-rw-r--r--   0        0        0    72300 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   133792 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   164689 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   311805 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd
+-rw-r--r--   0        0        0   252643 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   492947 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     8058 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0    14830 2024-05-23 05:42:26.412826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json
+-rw-r--r--   0        0        0   171640 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd
+-rw-r--r--   0        0        0     2573 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/schema/schema.py
+-rw-r--r--   0        0        0     6576 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/serialization/__init__.py
+-rw-r--r--   0        0        0     2503 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/spdx.py
+-rw-r--r--   0        0        0     3701 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/validation/__init__.py
+-rw-r--r--   0        0        0     4817 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/validation/json.py
+-rw-r--r--   0        0        0      853 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/validation/model.py
+-rw-r--r--   0        0        0     3672 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/cyclonedx/validation/xml.py
+-rw-r--r--   0        0        0      634 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/Makefile
+-rw-r--r--   0        0        0     1524 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/architecture.rst
+-rw-r--r--   0        0        0      686 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/changelog.rst
+-rw-r--r--   0        0        0     2657 2024-05-23 05:42:46.196781 cyclonedx_python_lib-7.4.0/docs/conf.py
+-rw-r--r--   0        0        0       34 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/contributing.rst
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/examples.rst
+-rw-r--r--   0        0        0     1857 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/index.rst
+-rw-r--r--   0        0        0     1499 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/install.rst
+-rw-r--r--   0        0        0      800 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/make.bat
+-rw-r--r--   0        0        0     3275 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/modelling.rst
+-rw-r--r--   0        0        0     2269 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/outputting.rst
+-rw-r--r--   0        0        0       81 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/requirements.txt
+-rw-r--r--   0        0        0     8093 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/schema-support.rst
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/docs/support.rst
+-rw-r--r--   0        0        0      176 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/examples/README.md
+-rw-r--r--   0        0        0     8164 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/examples/complex_deserialize.py
+-rw-r--r--   0        0        0     4081 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/examples/complex_serialize.py
+-rw-r--r--   0        0        0     4249 2024-05-23 05:42:46.196781 cyclonedx_python_lib-7.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6967 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/__init__.py
+-rw-r--r--   0        0        0    44385 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/models.py
+-rw-r--r--   0        0        0       16 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/README.md
+-rw-r--r--   0        0        0     1213 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1358 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0     1309 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json
+-rw-r--r--   0        0        0      567 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.4/empty_supplier.json
+-rw-r--r--   0        0        0     2461 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/xml/1.4/bom_setuptools.xml
+-rw-r--r--   0        0        0    98508 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/own/xml/1.4/webgoat-6.1.xml
+-rw-r--r--   0        0        0     3723 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml
+-rw-r--r--   0        0        0     1195 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml
+-rw-r--r--   0        0        0      559 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      313 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-component-type-1.1.xml
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-empty-component-1.1.xml
+-rw-r--r--   0        0        0      830 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml
+-rw-r--r--   0        0        0      801 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml
+-rw-r--r--   0        0        0      793 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml
+-rw-r--r--   0        0        0      769 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml
+-rw-r--r--   0        0        0     1303 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml
+-rw-r--r--   0        0        0    16515 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml
+-rw-r--r--   0        0        0    16513 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1328 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml
+-rw-r--r--   0        0        0     1366 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml
+-rw-r--r--   0        0        0      302 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-missing-component-type-1.1.xml
+-rw-r--r--   0        0        0    21038 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml
+-rw-r--r--   0        0        0      348 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-scope-1.1.xml
+-rw-r--r--   0        0        0    21026 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml
+-rw-r--r--   0        0        0     1217 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml
+-rw-r--r--   0        0        0      704 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml
+-rw-r--r--   0        0        0      965 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml
+-rw-r--r--   0        0        0      186 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-empty-components-1.1.xml
+-rw-r--r--   0        0        0    22339 2024-05-23 05:42:26.416826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml
+-rw-r--r--   0        0        0     1210 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml
+-rw-r--r--   0        0        0     1214 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml
+-rw-r--r--   0        0        0     1226 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml
+-rw-r--r--   0        0        0      317 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-minimal-viable-1.1.xml
+-rw-r--r--   0        0        0    21121 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml
+-rw-r--r--   0        0        0    10048 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml
+-rw-r--r--   0        0        0      165 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-bomformat-1.2.json
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.json
+-rw-r--r--   0        0        0      560 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      385 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.json
+-rw-r--r--   0        0        0      433 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-swid-1.2.xml
+-rw-r--r--   0        0        0      249 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.json
+-rw-r--r--   0        0        0      314 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-type-1.2.xml
+-rw-r--r--   0        0        0      667 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json
+-rw-r--r--   0        0        0      809 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml
+-rw-r--r--   0        0        0      247 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-empty-component-1.2.xml
+-rw-r--r--   0        0        0      856 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json
+-rw-r--r--   0        0        0      831 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml
+-rw-r--r--   0        0        0      827 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json
+-rw-r--r--   0        0        0      802 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml
+-rw-r--r--   0        0        0      819 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json
+-rw-r--r--   0        0        0      794 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml
+-rw-r--r--   0        0        0      795 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json
+-rw-r--r--   0        0        0      770 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json
+-rw-r--r--   0        0        0      706 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml
+-rw-r--r--   0        0        0     1184 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json
+-rw-r--r--   0        0        0     1554 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml
+-rw-r--r--   0        0        0      515 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json
+-rw-r--r--   0        0        0     1304 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml
+-rw-r--r--   0        0        0    15788 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json
+-rw-r--r--   0        0        0    16516 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml
+-rw-r--r--   0        0        0      428 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.json
+-rw-r--r--   0        0        0    16514 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml
+-rw-r--r--   0        0        0     1367 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml
+-rw-r--r--   0        0        0      209 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      244 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      303 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-missing-component-type-1.2.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml
+-rw-r--r--   0        0        0     1185 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json
+-rw-r--r--   0        0        0     1555 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml
+-rw-r--r--   0        0        0      275 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.json
+-rw-r--r--   0        0        0      349 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-scope-1.2.xml
+-rw-r--r--   0        0        0      148 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.json
+-rw-r--r--   0        0        0    21027 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.json
+-rw-r--r--   0        0        0      416 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-service-data-1.2.xml
+-rw-r--r--   0        0        0      363 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/skip_invalid-empty-component-1.2.json
+-rw-r--r--   0        0        0      361 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/skip_invalid-missing-component-type-1.2.json
+-rw-r--r--   0        0        0      548 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml
+-rw-r--r--   0        0        0    20390 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json
+-rw-r--r--   0        0        0    24278 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml
+-rw-r--r--   0        0        0     2163 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json
+-rw-r--r--   0        0        0     1897 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.json
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-1.2.xml
+-rw-r--r--   0        0        0     1342 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json
+-rw-r--r--   0        0        0     1346 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml
+-rw-r--r--   0        0        0      892 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json
+-rw-r--r--   0        0        0     1223 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml
+-rw-r--r--   0        0        0      693 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json
+-rw-r--r--   0        0        0      824 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml
+-rw-r--r--   0        0        0      161 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.json
+-rw-r--r--   0        0        0      187 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-empty-components-1.2.xml
+-rw-r--r--   0        0        0    22340 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.json
+-rw-r--r--   0        0        0     1211 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.json
+-rw-r--r--   0        0        0     1215 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml
+-rw-r--r--   0        0        0      440 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.json
+-rw-r--r--   0        0        0     1227 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml
+-rw-r--r--   0        0        0      333 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.json
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-author-1.2.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-manufacture-1.2.xml
+-rw-r--r--   0        0        0      417 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.json
+-rw-r--r--   0        0        0      468 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-supplier-1.2.xml
+-rw-r--r--   0        0        0      224 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.json
+-rw-r--r--   0        0        0      254 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-timestamp-1.2.xml
+-rw-r--r--   0        0        0      605 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml
+-rw-r--r--   0        0        0      253 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.json
+-rw-r--r--   0        0        0      318 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-minimal-viable-1.2.xml
+-rw-r--r--   0        0        0     2465 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json
+-rw-r--r--   0        0        0     3337 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml
+-rw-r--r--   0        0        0    21122 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml
+-rw-r--r--   0        0        0     2308 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json
+-rw-r--r--   0        0        0     2693 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml
+-rw-r--r--   0        0        0      419 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.json
+-rw-r--r--   0        0        0      495 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-empty-objects-1.2.xml
+-rw-r--r--   0        0        0    11181 2024-05-23 05:42:26.420826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml
+-rw-r--r--   0        0        0      165 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-bomformat-1.3.json
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.json
+-rw-r--r--   0        0        0      560 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      385 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.json
+-rw-r--r--   0        0        0      433 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-swid-1.3.xml
+-rw-r--r--   0        0        0      249 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.json
+-rw-r--r--   0        0        0      314 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-type-1.3.xml
+-rw-r--r--   0        0        0      667 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json
+-rw-r--r--   0        0        0      809 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml
+-rw-r--r--   0        0        0      197 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.json
+-rw-r--r--   0        0        0      247 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-empty-component-1.3.xml
+-rw-r--r--   0        0        0      856 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json
+-rw-r--r--   0        0        0      831 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml
+-rw-r--r--   0        0        0      827 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json
+-rw-r--r--   0        0        0      802 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml
+-rw-r--r--   0        0        0      819 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json
+-rw-r--r--   0        0        0      794 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml
+-rw-r--r--   0        0        0      795 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json
+-rw-r--r--   0        0        0      770 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json
+-rw-r--r--   0        0        0      706 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml
+-rw-r--r--   0        0        0     1184 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json
+-rw-r--r--   0        0        0     1554 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml
+-rw-r--r--   0        0        0      515 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json
+-rw-r--r--   0        0        0     1304 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml
+-rw-r--r--   0        0        0    15788 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json
+-rw-r--r--   0        0        0    16516 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml
+-rw-r--r--   0        0        0      428 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.json
+-rw-r--r--   0        0        0    16514 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml
+-rw-r--r--   0        0        0     1367 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml
+-rw-r--r--   0        0        0      277 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      319 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      209 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      244 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      228 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.json
+-rw-r--r--   0        0        0      303 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-missing-component-type-1.3.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml
+-rw-r--r--   0        0        0     1185 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json
+-rw-r--r--   0        0        0     1555 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml
+-rw-r--r--   0        0        0      275 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.json
+-rw-r--r--   0        0        0      349 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-scope-1.3.xml
+-rw-r--r--   0        0        0      148 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.json
+-rw-r--r--   0        0        0    21027 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.json
+-rw-r--r--   0        0        0      416 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-service-data-1.3.xml
+-rw-r--r--   0        0        0      548 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml
+-rw-r--r--   0        0        0    20390 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json
+-rw-r--r--   0        0        0    24278 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml
+-rw-r--r--   0        0        0     2163 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json
+-rw-r--r--   0        0        0     1897 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.json
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-1.3.xml
+-rw-r--r--   0        0        0     1342 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json
+-rw-r--r--   0        0        0     1346 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml
+-rw-r--r--   0        0        0      892 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json
+-rw-r--r--   0        0        0     1223 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml
+-rw-r--r--   0        0        0     1497 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json
+-rw-r--r--   0        0        0     1983 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml
+-rw-r--r--   0        0        0      693 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json
+-rw-r--r--   0        0        0      824 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml
+-rw-r--r--   0        0        0      161 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.json
+-rw-r--r--   0        0        0      187 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-empty-components-1.3.xml
+-rw-r--r--   0        0        0     1384 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json
+-rw-r--r--   0        0        0     1596 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml
+-rw-r--r--   0        0        0    22340 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml
+-rw-r--r--   0        0        0     1117 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json
+-rw-r--r--   0        0        0     1324 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.json
+-rw-r--r--   0        0        0     1211 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.json
+-rw-r--r--   0        0        0     1215 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml
+-rw-r--r--   0        0        0      440 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.json
+-rw-r--r--   0        0        0     1227 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml
+-rw-r--r--   0        0        0      333 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.json
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-author-1.3.xml
+-rw-r--r--   0        0        0      279 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.json
+-rw-r--r--   0        0        0      321 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-license-1.3.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-manufacture-1.3.xml
+-rw-r--r--   0        0        0      417 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.json
+-rw-r--r--   0        0        0      468 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-supplier-1.3.xml
+-rw-r--r--   0        0        0      224 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.json
+-rw-r--r--   0        0        0      254 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-timestamp-1.3.xml
+-rw-r--r--   0        0        0      605 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml
+-rw-r--r--   0        0        0      253 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.json
+-rw-r--r--   0        0        0      318 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-minimal-viable-1.3.xml
+-rw-r--r--   0        0        0     2465 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json
+-rw-r--r--   0        0        0     3337 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml
+-rw-r--r--   0        0        0      983 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json
+-rw-r--r--   0        0        0     1213 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml
+-rw-r--r--   0        0        0    21122 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml
+-rw-r--r--   0        0        0     2308 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json
+-rw-r--r--   0        0        0     2693 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml
+-rw-r--r--   0        0        0      419 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.json
+-rw-r--r--   0        0        0      495 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-empty-objects-1.3.xml
+-rw-r--r--   0        0        0    11181 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml
+-rw-r--r--   0        0        0      165 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-bomformat-1.4.json
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.json
+-rw-r--r--   0        0        0      560 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      385 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.json
+-rw-r--r--   0        0        0      433 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-swid-1.4.xml
+-rw-r--r--   0        0        0      249 2024-05-23 05:42:26.424826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.json
+-rw-r--r--   0        0        0      314 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-type-1.4.xml
+-rw-r--r--   0        0        0      667 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json
+-rw-r--r--   0        0        0      809 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml
+-rw-r--r--   0        0        0      197 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.json
+-rw-r--r--   0        0        0      247 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-empty-component-1.4.xml
+-rw-r--r--   0        0        0      856 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json
+-rw-r--r--   0        0        0      831 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml
+-rw-r--r--   0        0        0      827 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json
+-rw-r--r--   0        0        0      802 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml
+-rw-r--r--   0        0        0      819 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json
+-rw-r--r--   0        0        0      794 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml
+-rw-r--r--   0        0        0      795 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json
+-rw-r--r--   0        0        0      770 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json
+-rw-r--r--   0        0        0      706 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml
+-rw-r--r--   0        0        0     1184 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json
+-rw-r--r--   0        0        0     1554 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml
+-rw-r--r--   0        0        0      515 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json
+-rw-r--r--   0        0        0     1304 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml
+-rw-r--r--   0        0        0    15788 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json
+-rw-r--r--   0        0        0    16516 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml
+-rw-r--r--   0        0        0      428 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.json
+-rw-r--r--   0        0        0    16514 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml
+-rw-r--r--   0        0        0     1367 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml
+-rw-r--r--   0        0        0      277 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      319 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      209 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      244 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      228 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.json
+-rw-r--r--   0        0        0      303 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-missing-component-type-1.4.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml
+-rw-r--r--   0        0        0     1185 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json
+-rw-r--r--   0        0        0     1555 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml
+-rw-r--r--   0        0        0      275 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.json
+-rw-r--r--   0        0        0      349 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-scope-1.4.xml
+-rw-r--r--   0        0        0      148 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.json
+-rw-r--r--   0        0        0    21027 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.json
+-rw-r--r--   0        0        0      416 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-service-data-1.4.xml
+-rw-r--r--   0        0        0      548 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml
+-rw-r--r--   0        0        0    20390 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json
+-rw-r--r--   0        0        0    24278 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml
+-rw-r--r--   0        0        0     2163 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json
+-rw-r--r--   0        0        0     1897 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.json
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-1.4.xml
+-rw-r--r--   0        0        0     1342 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json
+-rw-r--r--   0        0        0     1346 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml
+-rw-r--r--   0        0        0      892 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json
+-rw-r--r--   0        0        0     1223 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml
+-rw-r--r--   0        0        0     1497 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json
+-rw-r--r--   0        0        0     1983 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml
+-rw-r--r--   0        0        0      693 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json
+-rw-r--r--   0        0        0      824 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml
+-rw-r--r--   0        0        0      161 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.json
+-rw-r--r--   0        0        0      187 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-empty-components-1.4.xml
+-rw-r--r--   0        0        0     1384 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json
+-rw-r--r--   0        0        0     1596 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml
+-rw-r--r--   0        0        0    22340 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml
+-rw-r--r--   0        0        0     1117 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json
+-rw-r--r--   0        0        0     1324 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.json
+-rw-r--r--   0        0        0     1211 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.json
+-rw-r--r--   0        0        0     1215 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml
+-rw-r--r--   0        0        0      440 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.json
+-rw-r--r--   0        0        0     1227 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml
+-rw-r--r--   0        0        0      333 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.json
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-author-1.4.xml
+-rw-r--r--   0        0        0      279 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.json
+-rw-r--r--   0        0        0      321 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-license-1.4.xml
+-rw-r--r--   0        0        0      438 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-manufacture-1.4.xml
+-rw-r--r--   0        0        0      417 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.json
+-rw-r--r--   0        0        0      468 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-supplier-1.4.xml
+-rw-r--r--   0        0        0      224 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.json
+-rw-r--r--   0        0        0      254 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-timestamp-1.4.xml
+-rw-r--r--   0        0        0      605 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml
+-rw-r--r--   0        0        0      227 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.json
+-rw-r--r--   0        0        0      281 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-minimal-viable-1.4.xml
+-rw-r--r--   0        0        0     2465 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json
+-rw-r--r--   0        0        0     3337 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml
+-rw-r--r--   0        0        0      983 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json
+-rw-r--r--   0        0        0     1213 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml
+-rw-r--r--   0        0        0    21122 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml
+-rw-r--r--   0        0        0     5338 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json
+-rw-r--r--   0        0        0     6828 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml
+-rw-r--r--   0        0        0     2312 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json
+-rw-r--r--   0        0        0     2693 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml
+-rw-r--r--   0        0        0      419 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.json
+-rw-r--r--   0        0        0      495 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-empty-objects-1.4.xml
+-rw-r--r--   0        0        0     9733 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json
+-rw-r--r--   0        0        0     4274 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json
+-rw-r--r--   0        0        0     5987 2024-05-23 05:42:26.428826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml
+-rw-r--r--   0        0        0    11181 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml
+-rw-r--r--   0        0        0      165 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-bomformat-1.5.json
+-rw-r--r--   0        0        0      508 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.json
+-rw-r--r--   0        0        0      866 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      385 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.json
+-rw-r--r--   0        0        0      433 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-swid-1.5.xml
+-rw-r--r--   0        0        0      249 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.json
+-rw-r--r--   0        0        0      314 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-type-1.5.xml
+-rw-r--r--   0        0        0      746 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json
+-rw-r--r--   0        0        0     1086 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml
+-rw-r--r--   0        0        0      197 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.json
+-rw-r--r--   0        0        0      247 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-empty-component-1.5.xml
+-rw-r--r--   0        0        0      856 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json
+-rw-r--r--   0        0        0      831 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml
+-rw-r--r--   0        0        0      827 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json
+-rw-r--r--   0        0        0      802 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml
+-rw-r--r--   0        0        0      819 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json
+-rw-r--r--   0        0        0      794 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml
+-rw-r--r--   0        0        0      795 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json
+-rw-r--r--   0        0        0      770 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json
+-rw-r--r--   0        0        0      706 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml
+-rw-r--r--   0        0        0     1184 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json
+-rw-r--r--   0        0        0     1554 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml
+-rw-r--r--   0        0        0      515 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json
+-rw-r--r--   0        0        0     1304 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml
+-rw-r--r--   0        0        0    15788 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json
+-rw-r--r--   0        0        0    16516 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml
+-rw-r--r--   0        0        0      428 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.json
+-rw-r--r--   0        0        0    16514 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml
+-rw-r--r--   0        0        0     1367 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml
+-rw-r--r--   0        0        0      277 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      319 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      209 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      244 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0      228 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.json
+-rw-r--r--   0        0        0      303 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-missing-component-type-1.5.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml
+-rw-r--r--   0        0        0     1185 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json
+-rw-r--r--   0        0        0     1555 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml
+-rw-r--r--   0        0        0      275 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.json
+-rw-r--r--   0        0        0      349 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-scope-1.5.xml
+-rw-r--r--   0        0        0      148 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.json
+-rw-r--r--   0        0        0    21027 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.json
+-rw-r--r--   0        0        0      416 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-service-data-1.5.xml
+-rw-r--r--   0        0        0     2527 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json
+-rw-r--r--   0        0        0     3596 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml
+-rw-r--r--   0        0        0      548 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml
+-rw-r--r--   0        0        0    20390 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json
+-rw-r--r--   0        0        0    24278 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml
+-rw-r--r--   0        0        0     2163 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json
+-rw-r--r--   0        0        0     1897 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.json
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-1.5.xml
+-rw-r--r--   0        0        0     1342 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json
+-rw-r--r--   0        0        0     1346 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml
+-rw-r--r--   0        0        0      892 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json
+-rw-r--r--   0        0        0     1223 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml
+-rw-r--r--   0        0        0     1810 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json
+-rw-r--r--   0        0        0     2449 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml
+-rw-r--r--   0        0        0      693 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json
+-rw-r--r--   0        0        0      824 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml
+-rw-r--r--   0        0        0      161 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.json
+-rw-r--r--   0        0        0      187 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-empty-components-1.5.xml
+-rw-r--r--   0        0        0     3189 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json
+-rw-r--r--   0        0        0     4519 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml
+-rw-r--r--   0        0        0    22340 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml
+-rw-r--r--   0        0        0     1117 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json
+-rw-r--r--   0        0        0     1324 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml
+-rw-r--r--   0        0        0     7703 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json
+-rw-r--r--   0        0        0    11757 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml
+-rw-r--r--   0        0        0      473 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.json
+-rw-r--r--   0        0        0     1270 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml
+-rw-r--r--   0        0        0      467 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.json
+-rw-r--r--   0        0        0     1236 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml
+-rw-r--r--   0        0        0     1539 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json
+-rw-r--r--   0        0        0     2197 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml
+-rw-r--r--   0        0        0      477 2024-05-23 05:42:26.432826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.json
+-rw-r--r--   0        0        0     1248 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml
+-rw-r--r--   0        0        0    98548 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json
+-rw-r--r--   0        0        0   100112 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml
+-rw-r--r--   0        0        0      333 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.json
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-author-1.5.xml
+-rw-r--r--   0        0        0      279 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.json
+-rw-r--r--   0        0        0      321 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-license-1.5.xml
+-rw-r--r--   0        0        0      436 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.json
+-rw-r--r--   0        0        0      624 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml
+-rw-r--r--   0        0        0      507 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.json
+-rw-r--r--   0        0        0      537 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml
+-rw-r--r--   0        0        0      482 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.json
+-rw-r--r--   0        0        0      509 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-supplier-1.5.xml
+-rw-r--r--   0        0        0      224 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.json
+-rw-r--r--   0        0        0      254 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-timestamp-1.5.xml
+-rw-r--r--   0        0        0     1162 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json
+-rw-r--r--   0        0        0     1471 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml
+-rw-r--r--   0        0        0      605 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml
+-rw-r--r--   0        0        0      227 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.json
+-rw-r--r--   0        0        0      281 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-minimal-viable-1.5.xml
+-rw-r--r--   0        0        0     2465 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json
+-rw-r--r--   0        0        0     3337 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml
+-rw-r--r--   0        0        0     1520 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json
+-rw-r--r--   0        0        0     1660 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml
+-rw-r--r--   0        0        0    21122 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml
+-rw-r--r--   0        0        0     5338 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json
+-rw-r--r--   0        0        0     6828 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml
+-rw-r--r--   0        0        0     9412 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json
+-rw-r--r--   0        0        0    12249 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml
+-rw-r--r--   0        0        0     2312 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json
+-rw-r--r--   0        0        0     2693 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml
+-rw-r--r--   0        0        0      419 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.json
+-rw-r--r--   0        0        0      495 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-empty-objects-1.5.xml
+-rw-r--r--   0        0        0     9733 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json
+-rw-r--r--   0        0        0    17746 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json
+-rw-r--r--   0        0        0    19794 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml
+-rw-r--r--   0        0        0    11181 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml
+-rw-r--r--   0        0        0      165 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-bomformat-1.6.json
+-rw-r--r--   0        0        0      508 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.json
+-rw-r--r--   0        0        0      866 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      385 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.json
+-rw-r--r--   0        0        0      433 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-swid-1.6.xml
+-rw-r--r--   0        0        0      249 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.json
+-rw-r--r--   0        0        0      314 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-type-1.6.xml
+-rw-r--r--   0        0        0      746 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json
+-rw-r--r--   0        0        0     1086 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml
+-rw-r--r--   0        0        0      197 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.json
+-rw-r--r--   0        0        0      247 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-empty-component-1.6.xml
+-rw-r--r--   0        0        0      856 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json
+-rw-r--r--   0        0        0      831 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml
+-rw-r--r--   0        0        0      827 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json
+-rw-r--r--   0        0        0      802 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml
+-rw-r--r--   0        0        0      819 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json
+-rw-r--r--   0        0        0      794 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml
+-rw-r--r--   0        0        0      795 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json
+-rw-r--r--   0        0        0      770 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml
+-rw-r--r--   0        0        0      731 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json
+-rw-r--r--   0        0        0      706 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml
+-rw-r--r--   0        0        0     1184 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json
+-rw-r--r--   0        0        0     1554 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml
+-rw-r--r--   0        0        0      515 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json
+-rw-r--r--   0        0        0     1304 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml
+-rw-r--r--   0        0        0    15788 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json
+-rw-r--r--   0        0        0    16516 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml
+-rw-r--r--   0        0        0      428 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.json
+-rw-r--r--   0        0        0    16514 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1329 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml
+-rw-r--r--   0        0        0      360 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.json
+-rw-r--r--   0        0        0      466 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-missing-id-and-name-1.6.xml
+-rw-r--r--   0        0        0     1367 2024-05-23 05:42:26.436826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml
+-rw-r--r--   0        0        0      277 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      319 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      209 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      244 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0      228 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.json
+-rw-r--r--   0        0        0      303 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-missing-component-type-1.6.xml
+-rw-r--r--   0        0        0    21039 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml
+-rw-r--r--   0        0        0     1185 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json
+-rw-r--r--   0        0        0     1555 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml
+-rw-r--r--   0        0        0     1290 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json
+-rw-r--r--   0        0        0     1504 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml
+-rw-r--r--   0        0        0      275 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.json
+-rw-r--r--   0        0        0      349 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-scope-1.6.xml
+-rw-r--r--   0        0        0      148 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.json
+-rw-r--r--   0        0        0    21027 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.json
+-rw-r--r--   0        0        0      416 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-service-data-1.6.xml
+-rw-r--r--   0        0        0     2527 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json
+-rw-r--r--   0        0        0     3596 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml
+-rw-r--r--   0        0        0      548 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml
+-rw-r--r--   0        0        0     5654 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json
+-rw-r--r--   0        0        0     7084 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml
+-rw-r--r--   0        0        0     6538 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json
+-rw-r--r--   0        0        0    24921 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml
+-rw-r--r--   0        0        0     2163 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json
+-rw-r--r--   0        0        0     1897 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml
+-rw-r--r--   0        0        0      750 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json
+-rw-r--r--   0        0        0      865 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml
+-rw-r--r--   0        0        0      394 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.json
+-rw-r--r--   0        0        0      705 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.json
+-rw-r--r--   0        0        0      492 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-1.6.xml
+-rw-r--r--   0        0        0     1342 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json
+-rw-r--r--   0        0        0     1346 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml
+-rw-r--r--   0        0        0      892 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json
+-rw-r--r--   0        0        0     1223 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml
+-rw-r--r--   0        0        0     1810 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json
+-rw-r--r--   0        0        0     2449 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml
+-rw-r--r--   0        0        0     2978 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json
+-rw-r--r--   0        0        0     4629 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml
+-rw-r--r--   0        0        0     1459 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json
+-rw-r--r--   0        0        0     2217 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml
+-rw-r--r--   0        0        0      693 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json
+-rw-r--r--   0        0        0      824 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml
+-rw-r--r--   0        0        0      161 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.json
+-rw-r--r--   0        0        0      187 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-empty-components-1.6.xml
+-rw-r--r--   0        0        0     4432 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json
+-rw-r--r--   0        0        0     6383 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml
+-rw-r--r--   0        0        0    22340 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml
+-rw-r--r--   0        0        0     1117 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json
+-rw-r--r--   0        0        0     1324 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml
+-rw-r--r--   0        0        0     7703 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json
+-rw-r--r--   0        0        0    11757 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml
+-rw-r--r--   0        0        0      514 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json
+-rw-r--r--   0        0        0     1297 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml
+-rw-r--r--   0        0        0      510 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.json
+-rw-r--r--   0        0        0     1263 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml
+-rw-r--r--   0        0        0     1539 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json
+-rw-r--r--   0        0        0     2197 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml
+-rw-r--r--   0        0        0      477 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.json
+-rw-r--r--   0        0        0     1248 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml
+-rw-r--r--   0        0        0    98548 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json
+-rw-r--r--   0        0        0   100112 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml
+-rw-r--r--   0        0        0     1835 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json
+-rw-r--r--   0        0        0     2811 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml
+-rw-r--r--   0        0        0      333 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.json
+-rw-r--r--   0        0        0      430 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-author-1.6.xml
+-rw-r--r--   0        0        0      432 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.json
+-rw-r--r--   0        0        0      456 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-license-1.6.xml
+-rw-r--r--   0        0        0      436 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.json
+-rw-r--r--   0        0        0      624 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml
+-rw-r--r--   0        0        0      521 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json
+-rw-r--r--   0        0        0      551 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml
+-rw-r--r--   0        0        0      508 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.json
+-rw-r--r--   0        0        0      539 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml
+-rw-r--r--   0        0        0      482 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.json
+-rw-r--r--   0        0        0      509 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-supplier-1.6.xml
+-rw-r--r--   0        0        0      224 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.json
+-rw-r--r--   0        0        0      254 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-timestamp-1.6.xml
+-rw-r--r--   0        0        0     1162 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json
+-rw-r--r--   0        0        0     1471 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml
+-rw-r--r--   0        0        0      605 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml
+-rw-r--r--   0        0        0      227 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.json
+-rw-r--r--   0        0        0      281 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-minimal-viable-1.6.xml
+-rw-r--r--   0        0        0     2465 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json
+-rw-r--r--   0        0        0     3337 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml
+-rw-r--r--   0        0        0     1894 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json
+-rw-r--r--   0        0        0     1872 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml
+-rw-r--r--   0        0        0    21122 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml
+-rw-r--r--   0        0        0     5338 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json
+-rw-r--r--   0        0        0     6828 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml
+-rw-r--r--   0        0        0     9412 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json
+-rw-r--r--   0        0        0    12249 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml
+-rw-r--r--   0        0        0     2312 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json
+-rw-r--r--   0        0        0     2693 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml
+-rw-r--r--   0        0        0      419 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.json
+-rw-r--r--   0        0        0      495 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-empty-objects-1.6.xml
+-rw-r--r--   0        0        0     9733 2024-05-23 05:42:26.440826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json
+-rw-r--r--   0        0        0     1902 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json
+-rw-r--r--   0        0        0     2747 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml
+-rw-r--r--   0        0        0      491 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.json
+-rw-r--r--   0        0        0      870 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml
+-rw-r--r--   0        0        0    17746 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json
+-rw-r--r--   0        0        0    19794 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml
+-rw-r--r--   0        0        0    11181 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml
+-rw-r--r--   0        0        0      157 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/README.md
+-rwxr-xr-x   0        0        0      745 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/fetch.sh
+-rw-r--r--   0        0        0      391 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/README.md
+-rw-r--r--   0        0        0      579 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin
+-rw-r--r--   0        0        0      649 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin
+-rw-r--r--   0        0        0     1050 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin
+-rw-r--r--   0        0        0     1055 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin
+-rw-r--r--   0        0        0     1050 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin
+-rw-r--r--   0        0        0     1055 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin
+-rw-r--r--   0        0        0     2128 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin
+-rw-r--r--   0        0        0     2211 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin
+-rw-r--r--   0        0        0     2264 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin
+-rw-r--r--   0        0        0     2326 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin
+-rw-r--r--   0        0        0     2264 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin
+-rw-r--r--   0        0        0     2326 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin
+-rw-r--r--   0        0        0      806 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin
+-rw-r--r--   0        0        0      949 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin
+-rw-r--r--   0        0        0     1835 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin
+-rw-r--r--   0        0        0     1806 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin
+-rw-r--r--   0        0        0     1835 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin
+-rw-r--r--   0        0        0     1806 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin
+-rw-r--r--   0        0        0     2808 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin
+-rw-r--r--   0        0        0     2877 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin
+-rw-r--r--   0        0        0     3596 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin
+-rw-r--r--   0        0        0     3640 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin
+-rw-r--r--   0        0        0     3788 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin
+-rw-r--r--   0        0        0     3831 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.1.xml.bin
+-rw-r--r--   0        0        0      944 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin
+-rw-r--r--   0        0        0      865 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin
+-rw-r--r--   0        0        0      944 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin
+-rw-r--r--   0        0        0      865 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin
+-rw-r--r--   0        0        0     2085 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin
+-rw-r--r--   0        0        0     2072 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin
+-rw-r--r--   0        0        0     2221 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin
+-rw-r--r--   0        0        0     2187 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin
+-rw-r--r--   0        0        0     2221 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin
+-rw-r--r--   0        0        0     2187 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.0.xml.bin
+-rw-r--r--   0        0        0      496 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.1.xml.bin
+-rw-r--r--   0        0        0      893 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin
+-rw-r--r--   0        0        0      812 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin
+-rw-r--r--   0        0        0      893 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin
+-rw-r--r--   0        0        0      812 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin
+-rw-r--r--   0        0        0     2013 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin
+-rw-r--r--   0        0        0     2002 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin
+-rw-r--r--   0        0        0     2149 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin
+-rw-r--r--   0        0        0     2117 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin
+-rw-r--r--   0        0        0     2149 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin
+-rw-r--r--   0        0        0     2117 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.0.xml.bin
+-rw-r--r--   0        0        0     4485 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin
+-rw-r--r--   0        0        0     4434 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin
+-rw-r--r--   0        0        0     4801 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin
+-rw-r--r--   0        0        0     4434 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin
+-rw-r--r--   0        0        0     4801 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin
+-rw-r--r--   0        0        0     5562 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin
+-rw-r--r--   0        0        0     5999 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin
+-rw-r--r--   0        0        0     5947 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin
+-rw-r--r--   0        0        0     6363 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin
+-rw-r--r--   0        0        0     5991 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin
+-rw-r--r--   0        0        0     6407 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin
+-rw-r--r--   0        0        0      749 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin
+-rw-r--r--   0        0        0      793 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin
+-rw-r--r--   0        0        0     1894 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin
+-rw-r--r--   0        0        0     1461 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin
+-rw-r--r--   0        0        0     1894 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin
+-rw-r--r--   0        0        0     1461 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin
+-rw-r--r--   0        0        0     3014 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin
+-rw-r--r--   0        0        0     2651 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin
+-rw-r--r--   0        0        0     3150 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin
+-rw-r--r--   0        0        0     2766 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin
+-rw-r--r--   0        0        0     3150 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin
+-rw-r--r--   0        0        0     2766 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.3.xml.bin
+-rw-r--r--   0        0        0     2092 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin
+-rw-r--r--   0        0        0     2289 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin
+-rw-r--r--   0        0        0     2228 2024-05-23 05:42:26.444826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin
+-rw-r--r--   0        0        0     2404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin
+-rw-r--r--   0        0        0     2228 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin
+-rw-r--r--   0        0        0     2404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.3.xml.bin
+-rw-r--r--   0        0        0     3282 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin
+-rw-r--r--   0        0        0     3686 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin
+-rw-r--r--   0        0        0     3418 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin
+-rw-r--r--   0        0        0     3801 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin
+-rw-r--r--   0        0        0     3418 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin
+-rw-r--r--   0        0        0     3801 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.3.xml.bin
+-rw-r--r--   0        0        0     1827 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin
+-rw-r--r--   0        0        0     2023 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin
+-rw-r--r--   0        0        0     1963 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin
+-rw-r--r--   0        0        0     2138 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin
+-rw-r--r--   0        0        0     1963 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin
+-rw-r--r--   0        0        0     2138 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.3.xml.bin
+-rw-r--r--   0        0        0     2577 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin
+-rw-r--r--   0        0        0     2822 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin
+-rw-r--r--   0        0        0     2713 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin
+-rw-r--r--   0        0        0     2937 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin
+-rw-r--r--   0        0        0     2713 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin
+-rw-r--r--   0        0        0     2937 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.1.xml.bin
+-rw-r--r--   0        0        0     1081 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin
+-rw-r--r--   0        0        0     1083 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin
+-rw-r--r--   0        0        0     1081 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin
+-rw-r--r--   0        0        0     1083 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2201 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2273 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2337 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2388 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2337 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2388 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.0.xml.bin
+-rw-r--r--   0        0        0      308 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.1.xml.bin
+-rw-r--r--   0        0        0      886 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin
+-rw-r--r--   0        0        0      821 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin
+-rw-r--r--   0        0        0      886 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin
+-rw-r--r--   0        0        0      821 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin
+-rw-r--r--   0        0        0     2006 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin
+-rw-r--r--   0        0        0     2011 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin
+-rw-r--r--   0        0        0     2142 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin
+-rw-r--r--   0        0        0     2126 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin
+-rw-r--r--   0        0        0     2142 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin
+-rw-r--r--   0        0        0     2126 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.3.xml.bin
+-rw-r--r--   0        0        0     2014 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin
+-rw-r--r--   0        0        0     2243 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin
+-rw-r--r--   0        0        0     2150 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin
+-rw-r--r--   0        0        0     2358 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin
+-rw-r--r--   0        0        0     2150 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin
+-rw-r--r--   0        0        0     2358 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.1.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.2.xml.bin
+-rw-r--r--   0        0        0      413 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.json.bin
+-rw-r--r--   0        0        0      404 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.3.xml.bin
+-rw-r--r--   0        0        0     2025 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin
+-rw-r--r--   0        0        0     2268 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin
+-rw-r--r--   0        0        0     2161 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin
+-rw-r--r--   0        0        0     2383 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin
+-rw-r--r--   0        0        0     2161 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin
+-rw-r--r--   0        0        0     2383 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin
+-rw-r--r--   0        0        0      596 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin
+-rw-r--r--   0        0        0      695 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1561 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin
+-rw-r--r--   0        0        0     1597 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1561 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin
+-rw-r--r--   0        0        0     1597 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2702 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin
+-rw-r--r--   0        0        0     2804 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2838 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin
+-rw-r--r--   0        0        0     2919 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2838 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin
+-rw-r--r--   0        0        0     2919 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin
+-rw-r--r--   0        0        0      662 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin
+-rw-r--r--   0        0        0      678 2024-05-23 05:42:26.448826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin
+-rw-r--r--   0        0        0     1385 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin
+-rw-r--r--   0        0        0     1402 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin
+-rw-r--r--   0        0        0     1385 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin
+-rw-r--r--   0        0        0     1402 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin
+-rw-r--r--   0        0        0     2526 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin
+-rw-r--r--   0        0        0     2609 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin
+-rw-r--r--   0        0        0     2662 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin
+-rw-r--r--   0        0        0     2724 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin
+-rw-r--r--   0        0        0     2662 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin
+-rw-r--r--   0        0        0     2724 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin
+-rw-r--r--   0        0        0      246 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.0.xml.bin
+-rw-r--r--   0        0        0      847 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin
+-rw-r--r--   0        0        0     1085 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin
+-rw-r--r--   0        0        0     1163 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin
+-rw-r--r--   0        0        0     1085 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin
+-rw-r--r--   0        0        0     1163 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin
+-rw-r--r--   0        0        0     2205 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin
+-rw-r--r--   0        0        0     2353 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin
+-rw-r--r--   0        0        0     2341 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin
+-rw-r--r--   0        0        0     2468 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin
+-rw-r--r--   0        0        0     2341 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin
+-rw-r--r--   0        0        0     2468 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin
+-rw-r--r--   0        0        0      581 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.0.xml.bin
+-rw-r--r--   0        0        0      612 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.1.xml.bin
+-rw-r--r--   0        0        0      939 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.json.bin
+-rw-r--r--   0        0        0      962 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.xml.bin
+-rw-r--r--   0        0        0      939 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.json.bin
+-rw-r--r--   0        0        0      962 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.xml.bin
+-rw-r--r--   0        0        0     2080 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.json.bin
+-rw-r--r--   0        0        0     2169 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.xml.bin
+-rw-r--r--   0        0        0     2216 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.json.bin
+-rw-r--r--   0        0        0     2284 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.xml.bin
+-rw-r--r--   0        0        0     2216 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.json.bin
+-rw-r--r--   0        0        0     2284 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.1.xml.bin
+-rw-r--r--   0        0        0     8540 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin
+-rw-r--r--   0        0        0     8315 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin
+-rw-r--r--   0        0        0    10266 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin
+-rw-r--r--   0        0        0     9628 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin
+-rw-r--r--   0        0        0    13173 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin
+-rw-r--r--   0        0        0    12575 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin
+-rw-r--r--   0        0        0    13309 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin
+-rw-r--r--   0        0        0    12690 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin
+-rw-r--r--   0        0        0    14474 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin
+-rw-r--r--   0        0        0    14004 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0     2739 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin
+-rw-r--r--   0        0        0     3108 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin
+-rw-r--r--   0        0        0     2449 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin
+-rw-r--r--   0        0        0     2636 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin
+-rw-r--r--   0        0        0     3086 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin
+-rw-r--r--   0        0        0     3518 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin
+-rw-r--r--   0        0        0     2634 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin
+-rw-r--r--   0        0        0     2831 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin
+-rw-r--r--   0        0        0     2164 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin
+-rw-r--r--   0        0        0     2217 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin
+-rw-r--r--   0        0        0     2164 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin
+-rw-r--r--   0        0        0     2217 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin
+-rw-r--r--   0        0        0     1199 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin
+-rw-r--r--   0        0        0     4993 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin
+-rw-r--r--   0        0        0     7631 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin
+-rw-r--r--   0        0        0     7396 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin
+-rw-r--r--   0        0        0     8830 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin
+-rw-r--r--   0        0        0     8293 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin
+-rw-r--r--   0        0        0    11737 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin
+-rw-r--r--   0        0        0    11240 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin
+-rw-r--r--   0        0        0    11873 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin
+-rw-r--r--   0        0        0    11355 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin
+-rw-r--r--   0        0        0    12042 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin
+-rw-r--r--   0        0        0    11556 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin
+-rw-r--r--   0        0        0      307 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.0.xml.bin
+-rw-r--r--   0        0        0      477 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.1.xml.bin
+-rw-r--r--   0        0        0      860 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin
+-rw-r--r--   0        0        0      859 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin
+-rw-r--r--   0        0        0      860 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin
+-rw-r--r--   0        0        0      859 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin
+-rw-r--r--   0        0        0     1980 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin
+-rw-r--r--   0        0        0     2049 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin
+-rw-r--r--   0        0        0     2116 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin
+-rw-r--r--   0        0        0     2164 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin
+-rw-r--r--   0        0        0     2116 2024-05-23 05:42:26.452826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin
+-rw-r--r--   0        0        0     2164 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin
+-rw-r--r--   0        0        0      395 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.0.xml.bin
+-rw-r--r--   0        0        0      572 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin
+-rw-r--r--   0        0        0      952 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin
+-rw-r--r--   0        0        0      961 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin
+-rw-r--r--   0        0        0      952 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin
+-rw-r--r--   0        0        0      961 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin
+-rw-r--r--   0        0        0     2093 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin
+-rw-r--r--   0        0        0     2168 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin
+-rw-r--r--   0        0        0     2229 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin
+-rw-r--r--   0        0        0     2283 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin
+-rw-r--r--   0        0        0     2229 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin
+-rw-r--r--   0        0        0     2283 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin
+-rw-r--r--   0        0        0     3848 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin
+-rw-r--r--   0        0        0     3888 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin
+-rw-r--r--   0        0        0     3984 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin
+-rw-r--r--   0        0        0     4003 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin
+-rw-r--r--   0        0        0     3984 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin
+-rw-r--r--   0        0        0     4003 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin
+-rw-r--r--   0        0        0     2028 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin
+-rw-r--r--   0        0        0     2102 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin
+-rw-r--r--   0        0        0     2164 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin
+-rw-r--r--   0        0        0     2217 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin
+-rw-r--r--   0        0        0     3918 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin
+-rw-r--r--   0        0        0     4052 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin
+-rw-r--r--   0        0        0      329 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.0.xml.bin
+-rw-r--r--   0        0        0      506 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.1.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin
+-rw-r--r--   0        0        0      887 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin
+-rw-r--r--   0        0        0      895 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin
+-rw-r--r--   0        0        0     5189 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin
+-rw-r--r--   0        0        0     5704 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin
+-rw-r--r--   0        0        0     5325 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin
+-rw-r--r--   0        0        0     5819 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin
+-rw-r--r--   0        0        0     5518 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin
+-rw-r--r--   0        0        0     6044 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin
+-rw-r--r--   0        0        0     1056 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin
+-rw-r--r--   0        0        0     1071 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin
+-rw-r--r--   0        0        0     1243 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin
+-rw-r--r--   0        0        0     1214 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin
+-rw-r--r--   0        0        0     2384 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin
+-rw-r--r--   0        0        0     2421 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin
+-rw-r--r--   0        0        0     2520 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin
+-rw-r--r--   0        0        0     2536 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin
+-rw-r--r--   0        0        0     2520 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin
+-rw-r--r--   0        0        0     2536 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin
+-rw-r--r--   0        0        0     2950 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin
+-rw-r--r--   0        0        0     3403 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin
+-rw-r--r--   0        0        0      655 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin
+-rw-r--r--   0        0        0      980 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin
+-rw-r--r--   0        0        0     1582 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin
+-rw-r--r--   0        0        0     1579 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin
+-rw-r--r--   0        0        0     1769 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin
+-rw-r--r--   0        0        0     1722 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin
+-rw-r--r--   0        0        0     2889 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin
+-rw-r--r--   0        0        0     2912 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin
+-rw-r--r--   0        0        0     3025 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin
+-rw-r--r--   0        0        0     3027 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin
+-rw-r--r--   0        0        0     3025 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin
+-rw-r--r--   0        0        0     3027 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin
+-rw-r--r--   0        0        0      654 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin
+-rw-r--r--   0        0        0     1045 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin
+-rw-r--r--   0        0        0     1562 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin
+-rw-r--r--   0        0        0     1749 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin
+-rw-r--r--   0        0        0     2890 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin
+-rw-r--r--   0        0        0     3026 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin
+-rw-r--r--   0        0        0     3042 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin
+-rw-r--r--   0        0        0     3026 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin
+-rw-r--r--   0        0        0     3042 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.0.xml.bin
+-rw-r--r--   0        0        0      431 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.1.xml.bin
+-rw-r--r--   0        0        0      629 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin
+-rw-r--r--   0        0        0      666 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin
+-rw-r--r--   0        0        0      792 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin
+-rw-r--r--   0        0        0      797 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin
+-rw-r--r--   0        0        0     1933 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin
+-rw-r--r--   0        0        0     2004 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin
+-rw-r--r--   0        0        0     2069 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin
+-rw-r--r--   0        0        0     2119 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin
+-rw-r--r--   0        0        0     2069 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin
+-rw-r--r--   0        0        0     2119 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin
+-rw-r--r--   0        0        0      516 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0     1123 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     3019 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     2676 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     3119 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     2767 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     4176 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     3906 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     4312 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     4021 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     4482 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     4131 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      448 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.0.xml.bin
+-rw-r--r--   0        0        0      723 2024-05-23 05:42:26.456826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin
+-rw-r--r--   0        0        0     1575 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin
+-rw-r--r--   0        0        0     1577 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin
+-rw-r--r--   0        0        0     1762 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin
+-rw-r--r--   0        0        0     1720 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin
+-rw-r--r--   0        0        0     2903 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin
+-rw-r--r--   0        0        0     2927 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin
+-rw-r--r--   0        0        0     3039 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin
+-rw-r--r--   0        0        0     3042 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin
+-rw-r--r--   0        0        0     3039 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin
+-rw-r--r--   0        0        0     3042 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin
+-rw-r--r--   0        0        0      245 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.0.xml.bin
+-rw-r--r--   0        0        0      459 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.1.xml.bin
+-rw-r--r--   0        0        0     1475 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin
+-rw-r--r--   0        0        0     1382 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin
+-rw-r--r--   0        0        0     1649 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin
+-rw-r--r--   0        0        0     1533 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin
+-rw-r--r--   0        0        0     2748 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin
+-rw-r--r--   0        0        0     2706 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin
+-rw-r--r--   0        0        0     2884 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin
+-rw-r--r--   0        0        0     2821 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin
+-rw-r--r--   0        0        0     2884 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin
+-rw-r--r--   0        0        0     2821 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.1.xml.bin
+-rw-r--r--   0        0        0     3900 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin
+-rw-r--r--   0        0        0     4021 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin
+-rw-r--r--   0        0        0     4263 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin
+-rw-r--r--   0        0        0     4295 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin
+-rw-r--r--   0        0        0     7224 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin
+-rw-r--r--   0        0        0     7288 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin
+-rw-r--r--   0        0        0     7360 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin
+-rw-r--r--   0        0        0     7403 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin
+-rw-r--r--   0        0        0     7915 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin
+-rw-r--r--   0        0        0     8054 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.1.xml.bin
+-rw-r--r--   0        0        0     2106 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin
+-rw-r--r--   0        0        0     2196 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin
+-rw-r--r--   0        0        0     2469 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin
+-rw-r--r--   0        0        0     2470 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin
+-rw-r--r--   0        0        0     5430 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin
+-rw-r--r--   0        0        0     5463 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin
+-rw-r--r--   0        0        0     5566 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin
+-rw-r--r--   0        0        0     5578 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin
+-rw-r--r--   0        0        0     5735 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin
+-rw-r--r--   0        0        0     5779 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin
+-rw-r--r--   0        0        0      108 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.0.xml.bin
+-rw-r--r--   0        0        0      169 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.1.xml.bin
+-rw-r--r--   0        0        0     1030 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin
+-rw-r--r--   0        0        0     1040 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin
+-rw-r--r--   0        0        0     1030 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin
+-rw-r--r--   0        0        0     1040 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin
+-rw-r--r--   0        0        0     2171 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin
+-rw-r--r--   0        0        0     2247 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin
+-rw-r--r--   0        0        0     2307 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin
+-rw-r--r--   0        0        0     2362 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin
+-rw-r--r--   0        0        0     2307 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin
+-rw-r--r--   0        0        0     2362 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin
+-rw-r--r--   0        0        0     2957 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_component.py
+-rw-r--r--   0        0        0     3727 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_deserialize_json.py
+-rw-r--r--   0        0        0     1764 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_deserialize_xml.py
+-rw-r--r--   0        0        0    19038 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_enums.py
+-rw-r--r--   0        0        0     5728 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_factory_license.py
+-rw-r--r--   0        0        0    22602 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model.py
+-rw-r--r--   0        0        0    13254 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_bom.py
+-rw-r--r--   0        0        0     2782 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_bom_ref.py
+-rw-r--r--   0        0        0    18544 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_component.py
+-rw-r--r--   0        0        0     1793 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_dependency.py
+-rw-r--r--   0        0        0     4064 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_issue.py
+-rw-r--r--   0        0        0     4295 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_license.py
+-rw-r--r--   0        0        0     2758 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_release_note.py
+-rw-r--r--   0        0        0     3390 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_service.py
+-rw-r--r--   0        0        0    14370 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_model_vulnerability.py
+-rw-r--r--   0        0        0     3154 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_output.py
+-rw-r--r--   0        0        0     4587 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_output_json.py
+-rw-r--r--   0        0        0     4029 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_output_xml.py
+-rw-r--r--   0        0        0     1307 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_real_world_examples.py
+-rw-r--r--   0        0        0     2509 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_schema_SchemaVersion.py
+-rw-r--r--   0        0        0     1248 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_schema__res.py
+-rw-r--r--   0        0        0     2873 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_spdx.py
+-rw-r--r--   0        0        0     1977 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_validation.py
+-rw-r--r--   0        0        0     4939 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_validation_json.py
+-rw-r--r--   0        0        0     3414 2024-05-23 05:42:26.460826 cyclonedx_python_lib-7.4.0/tests/test_validation_xml.py
+-rw-r--r--   0        0        0     6666 1970-01-01 00:00:00.000000 cyclonedx_python_lib-7.4.0/PKG-INFO
```

### Comparing `cyclonedx_python_lib-7.3.4/CHANGELOG.md` & `cyclonedx_python_lib-7.4.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 # CHANGELOG
 
 
 
+## v7.3.4 (2024-05-06)
+
+### Fix
+
+* fix: allow suppliers with empty-string names (#611)
+
+fixes #600
+
+---------
+
+Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`b331aeb`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/b331aeb4b7261c7b1359c592b2dcda27bd35e369))
+
+
 ## v7.3.3 (2024-05-06)
 
 ### Chore
 
 * chore: shield_ossf-best-practices subbary
 
 Signed-off-by: Jan Kowalleck &lt;jan.kowalleck@gmail.com&gt; ([`0d00496`](https://github.com/CycloneDX/cyclonedx-python-lib/commit/0d00496ca2191394276d0410cc8e81e5630d674d))
```

### Comparing `cyclonedx_python_lib-7.3.4/LICENSE` & `cyclonedx_python_lib-7.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/README.md` & `cyclonedx_python_lib-7.4.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 [license_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/LICENSE
 [chaneglog_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/CHANGELOG.md
 [contributing_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/CONTRIBUTING.md
 
 [shield_gh-workflow-test]: https://img.shields.io/github/actions/workflow/status/CycloneDX/cyclonedx-python-lib/python.yml?branch=main&logo=GitHub&logoColor=white "build"
 [shield_coverage]: https://img.shields.io/codacy/coverage/1f9d451e9cdc49ce99c2a1247adab341?logo=Codacy&logoColor=white "test coverage"
-[shield_ossf-best-practices]: https://img.shields.io/cii/summary/7956?label=OpenSSF%20best%20practices "OpenSSF best practices"
+[shield_ossf-best-practices]: https://img.shields.io/cii/percentage/7956?label=OpenSSF%20best%20practices "OpenSSF best practices"
 [shield_pypi-version]: https://img.shields.io/pypi/v/cyclonedx-python-lib?logo=pypi&logoColor=white&label=PyPI "PyPI"
 [shield_conda-forge-version]: https://img.shields.io/conda/vn/conda-forge/cyclonedx-python-lib?logo=anaconda&logoColor=white&label=conda-forge "conda-forge"
 [shield_rtfd]: https://img.shields.io/readthedocs/cyclonedx-python-library?logo=readthedocs&logoColor=white "Read the Docs"
 [shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-python-lib?logo=open%20source%20initiative&logoColor=white "license"
 [shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"
 [shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"
 [shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/_internal/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,13 +11,10 @@
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 
 
 """
-Python library for CycloneDX
+!!! ALL SYMBOLS IN HERE ARE INTERNAL.
+Everything might change without any notice.
 """
-
-# !! version is managed by semantic_release
-# do not use typing here, or else `semantic_release` might have issues finding the variable
-__version__ = "7.3.4"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/_internal/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/_internal/time.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,7 +14,14 @@
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 
 
 """
 !!! ALL SYMBOLS IN HERE ARE INTERNAL.
 Everything might change without any notice.
 """
+
+
+from datetime import datetime, timezone
+
+
+def get_now_utc() -> datetime:
+    return datetime.now(tz=timezone.utc)
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/_internal/compare.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/_internal/compare.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/_internal/hash.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/_internal/hash.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/_internal/time.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,13 @@
 # limitations under the License.
 #
 # SPDX-License-Identifier: Apache-2.0
 # Copyright (c) OWASP Foundation. All Rights Reserved.
 
 
 """
-!!! ALL SYMBOLS IN HERE ARE INTERNAL.
-Everything might change without any notice.
+Python library for CycloneDX
 """
 
-
-from datetime import datetime, timezone
-
-
-def get_now_utc() -> datetime:
-    return datetime.now(tz=timezone.utc)
+# !! version is managed by semantic_release
+# do not use typing here, or else `semantic_release` might have issues finding the variable
+__version__ = "7.4.0"  # noqa:Q000
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/exception/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/exception/factory.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/exception/factory.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/exception/model.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/exception/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/exception/output.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/exception/output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/exception/serialization.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/exception/serialization.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/factory/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/factory/license.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/factory/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/bom.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/bom_ref.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/component.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/contact.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/contact.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/crypto.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/crypto.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/dependency.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/impact_analysis.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/impact_analysis.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/issue.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/license.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/release_note.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/service.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/model/vulnerability.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/model/vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/output/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/output/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/output/json.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/output/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/output/xml.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/output/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/README.md` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Resources: Schema files
 
 some schema for offline use as download via [script](../../../tools/schema-downloader.py).
 original sources: <https://github.com/CycloneDX/specification/tree/master/schema>
 
 Currently using version
-[55343ba19dee1785acf1ce9191540d5fd7b590db](https://github.com/CycloneDX/specification/commit/55343ba19dee1785acf1ce9191540d5fd7b590db)
+[5f3ee8066491d31ec6a6d02968243d9688d7e49c](https://github.com/CycloneDX/specification/commit/5f3ee8066491d31ec6a6d02968243d9688d7e49c)
 
 | file | note |
 |------|------|
 | [`bom-1.0.SNAPSHOT.xsd`](bom-1.0.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.1.SNAPSHOT.xsd`](bom-1.1.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.2.SNAPSHOT.xsd`](bom-1.2.SNAPSHOT.xsd) | applied changes: 1 |
 | [`bom-1.3.SNAPSHOT.xsd`](bom-1.3.SNAPSHOT.xsd) | applied changes: 1 |
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.0.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.1.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.2.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3-strict.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.3.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.4.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.5.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/bom-1.6.SNAPSHOT.xsd`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/jsf-0.82.SNAPSHOT.schema.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/spdx.SNAPSHOT.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8965706447187929%*

 * *Differences: {"'$comment'": "'v1.0-3.24.0'",*

 * * "'enum'": "{insert: [(1, '3D-Slicer-1.0'), (23, 'AMD-newlib'), (30, 'any-OSI'), (66, "*

 * *           "'BSD-2-Clause-first-lines'), (107, 'Catharon'), (204, 'cve-tou'), (301, 'Gutmann'), "*

 * *           "(312, 'HPND-export-US-acknowledgement'), (314, 'HPND-export2-US'), (317, "*

 * *           "'HPND-Intel'), (320, 'HPND-merchantability-variant'), (327, "*

 * *           "'HPND-sell-variant-MIT-disclaimer-rev'), (329, 'HPND-UC-export-US'), (417, "*

 * *           "'MIT-Khronos-old'), (445, 'NCBI- […]*

```diff
@@ -1,13 +1,14 @@
 {
-    "$comment": "v1.0-3.23",
+    "$comment": "v1.0-3.24.0",
     "$id": "http://cyclonedx.org/schema/spdx.schema.json",
     "$schema": "http://json-schema.org/draft-07/schema#",
     "enum": [
         "0BSD",
+        "3D-Slicer-1.0",
         "AAL",
         "Abstyles",
         "AdaCore-doc",
         "Adobe-2006",
         "Adobe-Display-PostScript",
         "Adobe-Glyph",
         "Adobe-Utopia",
@@ -21,20 +22,22 @@
         "AGPL-1.0",
         "AGPL-1.0-only",
         "AGPL-1.0-or-later",
         "AGPL-3.0",
         "AGPL-3.0-only",
         "AGPL-3.0-or-later",
         "Aladdin",
+        "AMD-newlib",
         "AMDPLPA",
         "AML",
         "AML-glslang",
         "AMPAS",
         "ANTLR-PD",
         "ANTLR-PD-fallback",
+        "any-OSI",
         "Apache-1.0",
         "Apache-1.1",
         "Apache-2.0",
         "APAFML",
         "APL-1.0",
         "App-s2p",
         "APSL-1.0",
@@ -62,14 +65,15 @@
         "Boehm-GC",
         "Borceux",
         "Brian-Gladman-2-Clause",
         "Brian-Gladman-3-Clause",
         "BSD-1-Clause",
         "BSD-2-Clause",
         "BSD-2-Clause-Darwin",
+        "BSD-2-Clause-first-lines",
         "BSD-2-Clause-FreeBSD",
         "BSD-2-Clause-NetBSD",
         "BSD-2-Clause-Patent",
         "BSD-2-Clause-Views",
         "BSD-3-Clause",
         "BSD-3-Clause-acpica",
         "BSD-3-Clause-Attribution",
@@ -102,14 +106,15 @@
         "bzip2-1.0.5",
         "bzip2-1.0.6",
         "C-UDA-1.0",
         "CAL-1.0",
         "CAL-1.0-Combined-Work-Exception",
         "Caldera",
         "Caldera-no-preamble",
+        "Catharon",
         "CATOSL-1.1",
         "CC-BY-1.0",
         "CC-BY-2.0",
         "CC-BY-2.5",
         "CC-BY-2.5-AU",
         "CC-BY-3.0",
         "CC-BY-3.0-AT",
@@ -198,14 +203,15 @@
         "CPOL-1.02",
         "Cronyx",
         "Crossword",
         "CrystalStacker",
         "CUA-OPL-1.0",
         "Cube",
         "curl",
+        "cve-tou",
         "D-FSL-1.0",
         "DEC-3-Clause",
         "diffmark",
         "DL-DE-BY-2.0",
         "DL-DE-ZERO-2.0",
         "DOC",
         "Dotseqn",
@@ -294,36 +300,43 @@
         "GPL-3.0-only",
         "GPL-3.0-or-later",
         "GPL-3.0-with-autoconf-exception",
         "GPL-3.0-with-GCC-exception",
         "Graphics-Gems",
         "gSOAP-1.3b",
         "gtkbook",
+        "Gutmann",
         "HaskellReport",
         "hdparm",
         "Hippocratic-2.1",
         "HP-1986",
         "HP-1989",
         "HPND",
         "HPND-DEC",
         "HPND-doc",
         "HPND-doc-sell",
         "HPND-export-US",
+        "HPND-export-US-acknowledgement",
         "HPND-export-US-modify",
+        "HPND-export2-US",
         "HPND-Fenneberg-Livingston",
         "HPND-INRIA-IMAG",
+        "HPND-Intel",
         "HPND-Kevlin-Henney",
         "HPND-Markus-Kuhn",
+        "HPND-merchantability-variant",
         "HPND-MIT-disclaimer",
         "HPND-Pbmplus",
         "HPND-sell-MIT-disclaimer-xserver",
         "HPND-sell-regexpr",
         "HPND-sell-variant",
         "HPND-sell-variant-MIT-disclaimer",
+        "HPND-sell-variant-MIT-disclaimer-rev",
         "HPND-UC",
+        "HPND-UC-export-US",
         "HTMLTIDY",
         "IBM-pibs",
         "ICU",
         "IEC-Code-Components-EULA",
         "IJG",
         "IJG-short",
         "ImageMagick",
@@ -403,14 +416,15 @@
         "MIT",
         "MIT-0",
         "MIT-advertising",
         "MIT-CMU",
         "MIT-enna",
         "MIT-feh",
         "MIT-Festival",
+        "MIT-Khronos-old",
         "MIT-Modern-Variant",
         "MIT-open-group",
         "MIT-testregex",
         "MIT-Wu",
         "MITNFA",
         "MMIXware",
         "Motosoto",
@@ -430,15 +444,17 @@
         "MulanPSL-2.0",
         "Multics",
         "Mup",
         "NAIST-2003",
         "NASA-1.3",
         "Naumen",
         "NBPL-1.0",
+        "NCBI-PD",
         "NCGL-UK-2.0",
+        "NCL",
         "NCSA",
         "Net-SNMP",
         "NetCDF",
         "Newsletr",
         "NGPL",
         "NICTA-1.0",
         "NIST-PD",
@@ -454,14 +470,15 @@
         "NPL-1.1",
         "NPOSL-3.0",
         "NRL",
         "NTP",
         "NTP-0",
         "Nunit",
         "O-UDA-1.0",
+        "OAR",
         "OCCT-PL",
         "OCLC-2.0",
         "ODbL-1.0",
         "ODC-By-1.0",
         "OFFIS",
         "OFL-1.0",
         "OFL-1.0-no-RFN",
@@ -510,19 +527,21 @@
         "PADL",
         "Parity-6.0.0",
         "Parity-7.0.0",
         "PDDL-1.0",
         "PHP-3.0",
         "PHP-3.01",
         "Pixar",
+        "pkgconf",
         "Plexus",
         "pnmstitch",
         "PolyForm-Noncommercial-1.0.0",
         "PolyForm-Small-Business-1.0.0",
         "PostgreSQL",
+        "PPL",
         "PSF-2.0",
         "psfrag",
         "psutils",
         "Python-2.0",
         "Python-2.0.1",
         "python-ldap",
         "Qhull",
@@ -570,23 +589,25 @@
         "SSH-OpenSSH",
         "SSH-short",
         "SSLeay-standalone",
         "SSPL-1.0",
         "StandardML-NJ",
         "SugarCRM-1.1.3",
         "Sun-PPP",
+        "Sun-PPP-2000",
         "SunPro",
         "SWL",
         "swrule",
         "Symlinks",
         "TAPR-OHL-1.0",
         "TCL",
         "TCP-wrappers",
         "TermReadKey",
         "TGPPL-1.0",
+        "threeparttable",
         "TMate",
         "TORQUE-1.1",
         "TOSL",
         "TPDL",
         "TPL-1.0",
         "TTWL",
         "TTYP0",
@@ -624,28 +645,30 @@
         "XFree86-1.1",
         "xinetd",
         "xkeyboard-config-Zinoviev",
         "xlock",
         "Xnet",
         "xpp",
         "XSkat",
+        "xzoom",
         "YPL-1.0",
         "YPL-1.1",
         "Zed",
         "Zeeff",
         "Zend-2.0",
         "Zimbra-1.3",
         "Zimbra-1.4",
         "Zlib",
         "zlib-acknowledgement",
         "ZPL-1.1",
         "ZPL-2.0",
         "ZPL-2.1",
         "389-exception",
         "Asterisk-exception",
+        "Asterisk-linking-protocols-exception",
         "Autoconf-exception-2.0",
         "Autoconf-exception-3.0",
         "Autoconf-exception-generic",
         "Autoconf-exception-generic-3.0",
         "Autoconf-exception-macro",
         "Bison-exception-1.24",
         "Bison-exception-2.2",
@@ -685,19 +708,21 @@
         "LZMA-exception",
         "mif-exception",
         "Nokia-Qt-exception-1.1",
         "OCaml-LGPL-linking-exception",
         "OCCT-exception-1.0",
         "OpenJDK-assembly-exception-1.0",
         "openvpn-openssl-exception",
+        "PCRE2-exception",
         "PS-or-PDF-font-exception-20170817",
         "QPL-1.0-INRIA-2004-exception",
         "Qt-GPL-exception-1.0",
         "Qt-LGPL-exception-1.1",
         "Qwt-exception-1.0",
+        "RRDtool-FLOSS-exception-2.0",
         "SANE-exception",
         "SHL-2.0",
         "SHL-2.1",
         "stunnel-exception",
         "SWI-exception",
         "Swift-exception",
         "Texinfo-exception",
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

 * *Files 0% similar despite different names*

#### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/_res/spdx.SNAPSHOT.xsd`

```diff
@@ -1,17 +1,22 @@
 <?xml version="1.0" encoding="utf-8"?>
-<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" targetNamespace="http://cyclonedx.org/schema/spdx" version="1.0-3.23">
+<xs:schema xmlns:xs="http://www.w3.org/2001/XMLSchema" elementFormDefault="qualified" targetNamespace="http://cyclonedx.org/schema/spdx" version="1.0-3.24.0">
   <xs:simpleType name="licenseId">
     <xs:restriction base="xs:string">
       <!-- Licenses -->
       <xs:enumeration value="0BSD">
         <xs:annotation>
           <xs:documentation>BSD Zero Clause License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="3D-Slicer-1.0">
+        <xs:annotation>
+          <xs:documentation>3D Slicer License v1.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="AAL">
         <xs:annotation>
           <xs:documentation>Attribution Assurance License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Abstyles">
         <xs:annotation>
@@ -109,14 +114,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Aladdin">
         <xs:annotation>
           <xs:documentation>Aladdin Free Public License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="AMD-newlib">
+        <xs:annotation>
+          <xs:documentation>AMD newlib License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="AMDPLPA">
         <xs:annotation>
           <xs:documentation>AMD's plpa_map.c License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="AML">
         <xs:annotation>
@@ -139,14 +149,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="ANTLR-PD-fallback">
         <xs:annotation>
           <xs:documentation>ANTLR Software Rights Notice with license fallback</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="any-OSI">
+        <xs:annotation>
+          <xs:documentation>Any OSI License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Apache-1.0">
         <xs:annotation>
           <xs:documentation>Apache License 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Apache-1.1">
         <xs:annotation>
@@ -314,14 +329,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause-Darwin">
         <xs:annotation>
           <xs:documentation>BSD 2-Clause - Ian Darwin variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="BSD-2-Clause-first-lines">
+        <xs:annotation>
+          <xs:documentation>BSD 2-Clause - first lines requirement</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause-FreeBSD">
         <xs:annotation>
           <xs:documentation>BSD 2-Clause FreeBSD License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="BSD-2-Clause-NetBSD">
         <xs:annotation>
@@ -514,14 +534,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Caldera-no-preamble">
         <xs:annotation>
           <xs:documentation>Caldera License (without preamble)</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Catharon">
+        <xs:annotation>
+          <xs:documentation>Catharon License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="CATOSL-1.1">
         <xs:annotation>
           <xs:documentation>Computer Associates Trusted Open Source License 1.1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="CC-BY-1.0">
         <xs:annotation>
@@ -994,14 +1019,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="curl">
         <xs:annotation>
           <xs:documentation>curl License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="cve-tou">
+        <xs:annotation>
+          <xs:documentation>Common Vulnerability Enumeration ToU License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="D-FSL-1.0">
         <xs:annotation>
           <xs:documentation>Deutsche Freie Software Lizenz</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="DEC-3-Clause">
         <xs:annotation>
@@ -1474,14 +1504,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="gtkbook">
         <xs:annotation>
           <xs:documentation>gtkbook License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Gutmann">
+        <xs:annotation>
+          <xs:documentation>Gutmann License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HaskellReport">
         <xs:annotation>
           <xs:documentation>Haskell Language Report License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="hdparm">
         <xs:annotation>
@@ -1524,39 +1559,59 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-export-US">
         <xs:annotation>
           <xs:documentation>HPND with US Government export control warning</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-export-US-acknowledgement">
+        <xs:annotation>
+          <xs:documentation>HPND with US Government export control warning and acknowledgment</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-export-US-modify">
         <xs:annotation>
           <xs:documentation>HPND with US Government export control warning and modification rqmt</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-export2-US">
+        <xs:annotation>
+          <xs:documentation>HPND with US Government export control and 2 disclaimers</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-Fenneberg-Livingston">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - Fenneberg-Livingston variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-INRIA-IMAG">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer    - INRIA-IMAG variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-Intel">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - Intel variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-Kevlin-Henney">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - Kevlin Henney variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-Markus-Kuhn">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - Markus Kuhn variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-merchantability-variant">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - merchantability variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-MIT-disclaimer">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer with MIT disclaimer</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-Pbmplus">
         <xs:annotation>
@@ -1579,19 +1634,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="HPND-sell-variant-MIT-disclaimer">
         <xs:annotation>
           <xs:documentation>HPND sell variant with MIT disclaimer</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-sell-variant-MIT-disclaimer-rev">
+        <xs:annotation>
+          <xs:documentation>HPND sell variant with MIT disclaimer - reverse</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HPND-UC">
         <xs:annotation>
           <xs:documentation>Historical Permission Notice and Disclaimer - University of California variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="HPND-UC-export-US">
+        <xs:annotation>
+          <xs:documentation>Historical Permission Notice and Disclaimer - University of California, US export warning</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="HTMLTIDY">
         <xs:annotation>
           <xs:documentation>HTML Tidy License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="IBM-pibs">
         <xs:annotation>
@@ -2019,14 +2084,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="MIT-Festival">
         <xs:annotation>
           <xs:documentation>MIT Festival Variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="MIT-Khronos-old">
+        <xs:annotation>
+          <xs:documentation>MIT Khronos - old variant</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="MIT-Modern-Variant">
         <xs:annotation>
           <xs:documentation>MIT License Modern Variant</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="MIT-open-group">
         <xs:annotation>
@@ -2154,19 +2224,29 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="NBPL-1.0">
         <xs:annotation>
           <xs:documentation>Net Boolean Public License v1</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="NCBI-PD">
+        <xs:annotation>
+          <xs:documentation>NCBI Public Domain Notice</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="NCGL-UK-2.0">
         <xs:annotation>
           <xs:documentation>Non-Commercial Government Licence</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="NCL">
+        <xs:annotation>
+          <xs:documentation>NCL Source Code License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="NCSA">
         <xs:annotation>
           <xs:documentation>University of Illinois/NCSA Open Source License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Net-SNMP">
         <xs:annotation>
@@ -2274,14 +2354,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="O-UDA-1.0">
         <xs:annotation>
           <xs:documentation>Open Use of Data Agreement v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="OAR">
+        <xs:annotation>
+          <xs:documentation>OAR License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="OCCT-PL">
         <xs:annotation>
           <xs:documentation>Open CASCADE Technology Public License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="OCLC-2.0">
         <xs:annotation>
@@ -2554,14 +2639,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Pixar">
         <xs:annotation>
           <xs:documentation>Pixar License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="pkgconf">
+        <xs:annotation>
+          <xs:documentation>pkgconf License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Plexus">
         <xs:annotation>
           <xs:documentation>Plexus Classworlds License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="pnmstitch">
         <xs:annotation>
@@ -2579,14 +2669,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="PostgreSQL">
         <xs:annotation>
           <xs:documentation>PostgreSQL License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="PPL">
+        <xs:annotation>
+          <xs:documentation>Peer Production License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="PSF-2.0">
         <xs:annotation>
           <xs:documentation>Python Software Foundation License 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="psfrag">
         <xs:annotation>
@@ -2854,14 +2949,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Sun-PPP">
         <xs:annotation>
           <xs:documentation>Sun PPP License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Sun-PPP-2000">
+        <xs:annotation>
+          <xs:documentation>Sun PPP License (2000)</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SunPro">
         <xs:annotation>
           <xs:documentation>SunPro License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SWL">
         <xs:annotation>
@@ -2899,14 +2999,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TGPPL-1.0">
         <xs:annotation>
           <xs:documentation>Transitive Grace Period Public Licence 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="threeparttable">
+        <xs:annotation>
+          <xs:documentation>threeparttable License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="TMate">
         <xs:annotation>
           <xs:documentation>TMate Open Source License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="TORQUE-1.1">
         <xs:annotation>
@@ -3124,14 +3229,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="XSkat">
         <xs:annotation>
           <xs:documentation>XSkat License</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="xzoom">
+        <xs:annotation>
+          <xs:documentation>xzoom License</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="YPL-1.0">
         <xs:annotation>
           <xs:documentation>Yahoo! Public License v1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="YPL-1.1">
         <xs:annotation>
@@ -3195,14 +3305,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Asterisk-exception">
         <xs:annotation>
           <xs:documentation>Asterisk exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="Asterisk-linking-protocols-exception">
+        <xs:annotation>
+          <xs:documentation>Asterisk linking protocols exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="Autoconf-exception-2.0">
         <xs:annotation>
           <xs:documentation>Autoconf exception 2.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Autoconf-exception-3.0">
         <xs:annotation>
@@ -3430,14 +3545,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="openvpn-openssl-exception">
         <xs:annotation>
           <xs:documentation>OpenVPN OpenSSL Exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="PCRE2-exception">
+        <xs:annotation>
+          <xs:documentation>PCRE2 exception</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="PS-or-PDF-font-exception-20170817">
         <xs:annotation>
           <xs:documentation>PS/PDF font exception (2017-08-17)</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="QPL-1.0-INRIA-2004-exception">
         <xs:annotation>
@@ -3455,14 +3575,19 @@
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="Qwt-exception-1.0">
         <xs:annotation>
           <xs:documentation>Qwt exception 1.0</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
+      <xs:enumeration value="RRDtool-FLOSS-exception-2.0">
+        <xs:annotation>
+          <xs:documentation>RRDtool FLOSS exception 2.0</xs:documentation>
+        </xs:annotation>
+      </xs:enumeration>
       <xs:enumeration value="SANE-exception">
         <xs:annotation>
           <xs:documentation>SANE Exception</xs:documentation>
         </xs:annotation>
       </xs:enumeration>
       <xs:enumeration value="SHL-2.0">
         <xs:annotation>
```

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/schema/schema.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/schema/schema.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/serialization/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/spdx.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/validation/__init__.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/validation/json.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/validation/json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/validation/model.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/validation/model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/cyclonedx/validation/xml.py` & `cyclonedx_python_lib-7.4.0/cyclonedx/validation/xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/Makefile` & `cyclonedx_python_lib-7.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/architecture.rst` & `cyclonedx_python_lib-7.4.0/docs/architecture.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/changelog.rst` & `cyclonedx_python_lib-7.4.0/docs/changelog.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/conf.py` & `cyclonedx_python_lib-7.4.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 project = 'CycloneDX Python Library'
 copyright = '2022, Copyright (c) OWASP Foundation'
 author = 'Paul Horton, Jan Kowalleck, Steve Springett, Patrick Dwyer'
 
 # The full version, including alpha/beta/rc tags
 # !! version is managed by semantic_release
-release = '7.3.4'
+release = '7.4.0'
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
```

### Comparing `cyclonedx_python_lib-7.3.4/docs/examples.rst` & `cyclonedx_python_lib-7.4.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/index.rst` & `cyclonedx_python_lib-7.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/install.rst` & `cyclonedx_python_lib-7.4.0/docs/install.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/make.bat` & `cyclonedx_python_lib-7.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/modelling.rst` & `cyclonedx_python_lib-7.4.0/docs/modelling.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/outputting.rst` & `cyclonedx_python_lib-7.4.0/docs/outputting.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/schema-support.rst` & `cyclonedx_python_lib-7.4.0/docs/schema-support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/docs/support.rst` & `cyclonedx_python_lib-7.4.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/examples/complex_deserialize.py` & `cyclonedx_python_lib-7.4.0/examples/complex_deserialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/examples/complex_serialize.py` & `cyclonedx_python_lib-7.4.0/examples/complex_serialize.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/pyproject.toml` & `cyclonedx_python_lib-7.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cyclonedx-python-lib"
 # !! version is managed by semantic_release
-version = "7.3.4"
+version = "7.4.0"
 description = "Python library for CycloneDX"
 authors = [
   "Paul Horton <phorton@sonatype.com>",
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
 ]
 maintainers = [
   "Jan Kowalleck <jan.kowalleck@gmail.com>",
@@ -80,25 +80,25 @@
 json-validation = ["jsonschema"]
 xml-validation = ["lxml"]
 
 [tool.poetry.group.dev.dependencies]
 ddt = "1.7.2"
 coverage = "7.5.1"
 flake8 = { version="7.0.0", python=">=3.8.1" }
-flake8-annotations = { version="3.0.1", python=">=3.8.1" }
+flake8-annotations = { version="3.1.1", python=">=3.8.1" }
 flake8-bugbear = { version="24.4.26", python=">=3.8.1" }
 flake8-isort = "6.1.1"
 flake8-quotes = "3.4.0"
 flake8-use-fstring = "1.4"
-pep8-naming = "0.13.3"
+pep8-naming = "0.14.1"
 isort = "5.13.2"
 autopep8 = "2.1.0"
 mypy = "1.10.0"
 tox = "4.15.0"
-xmldiff = "2.6.3"
+xmldiff = "2.7.0"
 bandit = "1.7.8"
 
 [tool.semantic_release]
 # see https://python-semantic-release.readthedocs.io/en/latest/configuration.html
 commit_author = "semantic-release <semantic-release@bot.local>"
 commit_message = "chore(release): {version}\n\nAutomatically generated by python-semantic-release\n\nSigned-off-by: semantic-release <semantic-release@bot.local>"
 upload_to_vcs_release = true
```

### Comparing `cyclonedx_python_lib-7.3.4/tests/__init__.py` & `cyclonedx_python_lib-7.4.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/__init__.py` & `cyclonedx_python_lib-7.4.0/tests/_data/__init__.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/models.py` & `cyclonedx_python_lib-7.4.0/tests/_data/models.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.2/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.2/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.3/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.3/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.4/bom_with_mixed_licenses.json` & `cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.4/bom_with_mixed_licenses.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/json/1.4/empty_supplier.json` & `cyclonedx_python_lib-7.4.0/tests/_data/own/json/1.4/empty_supplier.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/xml/1.4/bom_setuptools.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/own/xml/1.4/bom_setuptools.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/own/xml/1.4/webgoat-6.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/own/xml/1.4/webgoat-6.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.0/valid-bom-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.0/valid-component-hashes-1.0.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-alg-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-md5-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha1-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha256-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-hash-sha512-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-choice-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-encoding-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-id-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-license-name-count-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-namespace-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/invalid-serialnumber-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-bom-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-hashes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-ref-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-component-types-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-external-elements-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-expression-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-id-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-license-name-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-random-attributes-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.1/valid-xml-signature-1.1.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-alg-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-md5-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha1-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha256-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-hash-sha512-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-issue-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-choice-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-encoding-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-id-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-license-name-count-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-namespace-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-patch-type-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/invalid-serialnumber-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-assembly-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-bom-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-hashes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-ref-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-swid-full-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-component-types-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-dependency-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-external-elements-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-expression-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-id-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-license-name-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-metadata-tool-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-patch-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-random-attributes-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-1.2.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-1.2.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-service-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-service-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.2/valid-xml-signature-1.2.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-alg-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-md5-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha1-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha256-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-hash-sha512-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-issue-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-choice-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-encoding-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-id-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-license-name-count-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-namespace-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-patch-type-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/invalid-serialnumber-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-assembly-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-bom-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-hashes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-ref-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-swid-full-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-component-types-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-compositions-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-dependency-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-evidence-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-elements-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-external-reference-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-expression-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-id-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-license-name-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-metadata-tool-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-patch-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-properties-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-random-attributes-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-1.3.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-1.3.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-service-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-service-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.3/valid-xml-signature-1.3.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-alg-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-md5-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha1-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha256-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-hash-sha512-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-issue-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-choice-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-encoding-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-id-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-license-name-count-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-namespace-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-patch-type-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/invalid-serialnumber-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-assembly-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-bom-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-hashes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-ref-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-swid-full-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-component-types-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-compositions-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-dependency-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-evidence-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-elements-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-external-reference-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-expression-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-id-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-license-name-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-metadata-tool-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-patch-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-properties-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-random-attributes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-release-notes-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-service-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-service-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-signatures-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-vulnerability-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.4/valid-xml-signature-1.4.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-alg-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-md5-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha1-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha256-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-hash-sha512-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-issue-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-choice-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-encoding-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-id-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-license-name-count-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-namespace-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-patch-type-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/invalid-serialnumber-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-annotation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-assembly-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-bom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-hashes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-ref-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-swid-full-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-component-types-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-compositions-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-dependency-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-evidence-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-elements-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-external-reference-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-formulation-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-expression-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-id-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-licensing-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-license-name-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-machine-learning-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-lifecycle-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-manufacture-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-metadata-tool-deprecated-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-patch-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-properties-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-random-attributes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-release-notes-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-saasbom-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-service-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-service-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-signatures-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-vulnerability-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.5/valid-xml-signature-1.5.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-alg-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-md5-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha1-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha256-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-hash-sha512-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-issue-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-choice-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-encoding-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-id-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-license-name-count-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-namespace-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-patch-type-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/invalid-serialnumber-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-annotation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-assembly-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-attestation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-bom-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-bom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-hashes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-identifiers-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-ref-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-swid-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-component-types-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-compositions-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-full-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-cryptography-implementation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-dependency-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-evidence-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-elements-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-external-reference-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-formulation-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-expression-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-id-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-licensing-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-license-name-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-machine-learning-considerations-env-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-lifecycle-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacture-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-manufacturer-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-metadata-tool-deprecated-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-patch-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-patch-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-properties-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-properties-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-random-attributes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-release-notes-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-saasbom-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-service-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-service-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-signatures-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-standard-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-standard-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-tags-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.json`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-vulnerability-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/1.6/valid-xml-signature-1.6.xml`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/schemaTestData/fetch.sh` & `cyclonedx_python_lib-7.4.0/tests/_data/schemaTestData/fetch.sh`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentScope-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ComponentType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_DataFlow-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_Encoding-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_Encoding-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ExternalReferenceType-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_HashAlgorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisAffectedStatus-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisJustification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisResponse-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_ImpactAnalysisState-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_IssueClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_PatchClassification-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilityScoreSource-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/enum_VulnerabilitySeverity-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_275_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_328_components-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_497_urls-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_for_issue_598_multiple_components_with_purl_qualifiers-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_just_complete_metadata-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_algorithm-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_certificate-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_protocol-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_v1_6_with_crypto_related_material-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_basic-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_complete-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_no_component_version-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_cpe-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_release_notes-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_v16_fields-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_setuptools_with_vulnerability-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_component_toml_1-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_crypto-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_crypto-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_hanging-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_dependencies_valid-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_external_references-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.0.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_licenses-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.1.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_metadata_component_and_dependencies-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_multiple_licenses-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_nested_services-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_complex-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.2.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.3.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.4.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.5.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.json.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin` & `cyclonedx_python_lib-7.4.0/tests/_data/snapshots/get_bom_with_services_simple-1.6.xml.bin`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_component.py` & `cyclonedx_python_lib-7.4.0/tests/test_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_deserialize_json.py` & `cyclonedx_python_lib-7.4.0/tests/test_deserialize_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_deserialize_xml.py` & `cyclonedx_python_lib-7.4.0/tests/test_deserialize_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_enums.py` & `cyclonedx_python_lib-7.4.0/tests/test_enums.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_factory_license.py` & `cyclonedx_python_lib-7.4.0/tests/test_factory_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model.py` & `cyclonedx_python_lib-7.4.0/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_bom.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_bom.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_bom_ref.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_bom_ref.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_component.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_component.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_dependency.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_dependency.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_issue.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_issue.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_license.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_license.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_release_note.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_release_note.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_service.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_service.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_model_vulnerability.py` & `cyclonedx_python_lib-7.4.0/tests/test_model_vulnerability.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_output.py` & `cyclonedx_python_lib-7.4.0/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_output_json.py` & `cyclonedx_python_lib-7.4.0/tests/test_output_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_output_xml.py` & `cyclonedx_python_lib-7.4.0/tests/test_output_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_real_world_examples.py` & `cyclonedx_python_lib-7.4.0/tests/test_real_world_examples.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_schema_SchemaVersion.py` & `cyclonedx_python_lib-7.4.0/tests/test_schema_SchemaVersion.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_schema__res.py` & `cyclonedx_python_lib-7.4.0/tests/test_schema__res.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_spdx.py` & `cyclonedx_python_lib-7.4.0/tests/test_spdx.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_validation.py` & `cyclonedx_python_lib-7.4.0/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_validation_json.py` & `cyclonedx_python_lib-7.4.0/tests/test_validation_json.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/tests/test_validation_xml.py` & `cyclonedx_python_lib-7.4.0/tests/test_validation_xml.py`

 * *Files identical despite different names*

### Comparing `cyclonedx_python_lib-7.3.4/PKG-INFO` & `cyclonedx_python_lib-7.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyclonedx-python-lib
-Version: 7.3.4
+Version: 7.4.0
 Summary: Python library for CycloneDX
 Home-page: https://github.com/CycloneDX/cyclonedx-python-lib/#readme
 License: Apache-2.0
 Keywords: CycloneDX,library,OWASP,SCA,Software Bill of Materials,Bill of Materials,BOM,SBOM,VEX,VDR,OBOM,MBOM,SaaSBOM,SPDX,PackageURL,PURL
 Author: Paul Horton
 Author-email: phorton@sonatype.com
 Maintainer: Jan Kowalleck
@@ -100,15 +100,15 @@
 
 [license_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/LICENSE
 [chaneglog_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/CHANGELOG.md
 [contributing_file]: https://github.com/CycloneDX/cyclonedx-python-lib/blob/master/CONTRIBUTING.md
 
 [shield_gh-workflow-test]: https://img.shields.io/github/actions/workflow/status/CycloneDX/cyclonedx-python-lib/python.yml?branch=main&logo=GitHub&logoColor=white "build"
 [shield_coverage]: https://img.shields.io/codacy/coverage/1f9d451e9cdc49ce99c2a1247adab341?logo=Codacy&logoColor=white "test coverage"
-[shield_ossf-best-practices]: https://img.shields.io/cii/summary/7956?label=OpenSSF%20best%20practices "OpenSSF best practices"
+[shield_ossf-best-practices]: https://img.shields.io/cii/percentage/7956?label=OpenSSF%20best%20practices "OpenSSF best practices"
 [shield_pypi-version]: https://img.shields.io/pypi/v/cyclonedx-python-lib?logo=pypi&logoColor=white&label=PyPI "PyPI"
 [shield_conda-forge-version]: https://img.shields.io/conda/vn/conda-forge/cyclonedx-python-lib?logo=anaconda&logoColor=white&label=conda-forge "conda-forge"
 [shield_rtfd]: https://img.shields.io/readthedocs/cyclonedx-python-library?logo=readthedocs&logoColor=white "Read the Docs"
 [shield_license]: https://img.shields.io/github/license/CycloneDX/cyclonedx-python-lib?logo=open%20source%20initiative&logoColor=white "license"
 [shield_website]: https://img.shields.io/badge/https://-cyclonedx.org-blue.svg "homepage"
 [shield_slack]: https://img.shields.io/badge/slack-join-blue?logo=Slack&logoColor=white "slack join"
 [shield_groups]: https://img.shields.io/badge/discussion-groups.io-blue.svg "groups discussion"
```

