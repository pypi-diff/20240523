# Comparing `tmp/jpy-0.7.4.zip` & `tmp/jpy-0.7.5.zip`

## zipinfo {}

```diff
@@ -1,80 +1,80 @@
-Zip file size: 143154 bytes, number of entries: 78
--rw-rw-rw-  2.0 fat     1367 b- defN 14-Jul-11 13:56 jpy-0.7.4/CHANGES.txt
--rw-rw-rw-  2.0 fat    35795 b- defN 14-May-07 13:22 jpy-0.7.4/LICENSE.txt
--rw-rw-rw-  2.0 fat     2142 b- defN 14-Jul-15 17:33 jpy-0.7.4/PKG-INFO
--rw-rw-rw-  2.0 fat     5325 b- defN 14-Jul-15 17:26 jpy-0.7.4/pom.xml
--rw-rw-rw-  2.0 fat     5407 b- defN 14-Jul-15 17:26 jpy-0.7.4/setup.py
--rw-rw-rw-  2.0 fat     8445 b- defN 14-May-09 18:06 jpy-0.7.4/doc/conf.py
--rw-rw-rw-  2.0 fat      607 b- defN 14-May-08 11:33 jpy-0.7.4/doc/index.rst
--rw-rw-rw-  2.0 fat     8515 b- defN 14-Jun-12 14:00 jpy-0.7.4/doc/install.rst
--rw-rw-rw-  2.0 fat     5307 b- defN 14-Jun-03 17:57 jpy-0.7.4/doc/intro.rst
--rwx---     2.0 fat     6695 b- defN 14-May-07 13:22 jpy-0.7.4/doc/make.bat
--rw-rw-rw-  2.0 fat     6927 b- defN 14-May-07 13:22 jpy-0.7.4/doc/Makefile
--rw-rw-rw-  2.0 fat     3340 b- defN 14-May-08 12:06 jpy-0.7.4/doc/modify.rst
--rw-rw-rw-  2.0 fat    23125 b- defN 14-Jun-03 17:57 jpy-0.7.4/doc/reference.rst
--rw-rw-rw-  2.0 fat     1107 b- defN 14-May-08 11:45 jpy-0.7.4/doc/tutorial.rst
--rw-rw-rw-  2.0 fat     1137 b- defN 14-Jul-11 12:55 jpy-0.7.4/src/main/c/jpy_compat.c
--rw-rw-rw-  2.0 fat     2214 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_compat.h
--rw-rw-rw-  2.0 fat     7835 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_conv.c
--rw-rw-rw-  2.0 fat     4108 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_conv.h
--rw-rw-rw-  2.0 fat     5799 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_diag.c
--rw-rw-rw-  2.0 fat     1547 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jpy_diag.h
--rw-rw-rw-  2.0 fat    11507 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_jarray.c
--rw-rw-rw-  2.0 fat     1642 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jpy_jarray.h
--rw-rw-rw-  2.0 fat     4732 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_jfield.c
--rw-rw-rw-  2.0 fat     1565 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jpy_jfield.h
--rw-rw-rw-  2.0 fat    31727 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_jmethod.c
--rw-rw-rw-  2.0 fat     3208 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jpy_jmethod.h
--rw-rw-rw-  2.0 fat    29114 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_jobj.c
--rw-rw-rw-  2.0 fat     1418 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jpy_jobj.h
--rw-rw-rw-  2.0 fat    77120 b- defN 14-Jun-30 17:29 jpy-0.7.4/src/main/c/jpy_jtype.c
--rw-rw-rw-  2.0 fat     4185 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_jtype.h
--rw-rw-rw-  2.0 fat    33491 b- defN 14-Jul-11 11:35 jpy-0.7.4/src/main/c/jpy_module.c
--rw-rw-rw-  2.0 fat     5959 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/c/jpy_module.h
--rw-rw-rw-  2.0 fat    30450 b- defN 14-Jul-11 13:47 jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.c
--rw-rw-rw-  2.0 fat     4057 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.h
--rw-rw-rw-  2.0 fat      299 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jni/org_jpy_PyLib_CallableKind.h
--rw-rw-rw-  2.0 fat     1056 b- defN 14-May-07 13:22 jpy-0.7.4/src/main/c/jni/org_jpy_PyLib_Diag.h
--rw-rw-rw-  2.0 fat     1543 b- defN 14-May-09 14:11 jpy-0.7.4/src/main/java/org/jpy/package-info.java
--rw-rw-rw-  2.0 fat    13626 b- defN 14-May-09 18:06 jpy-0.7.4/src/main/java/org/jpy/PyLib.java
--rw-rw-rw-  2.0 fat     2756 b- defN 14-May-09 14:11 jpy-0.7.4/src/main/java/org/jpy/PyLibConfig.java
--rw-rw-rw-  2.0 fat     2157 b- defN 14-May-09 14:11 jpy-0.7.4/src/main/java/org/jpy/PyModule.java
--rw-rw-rw-  2.0 fat    10472 b- defN 14-May-12 09:07 jpy-0.7.4/src/main/java/org/jpy/PyObject.java
--rw-rw-rw-  2.0 fat     2550 b- defN 14-May-12 09:07 jpy-0.7.4/src/main/java/org/jpy/PyProxyHandler.java
--rw-rw-rw-  2.0 fat     1254 b- defN 14-May-09 14:11 jpy-0.7.4/src/main/java/org/jpy/annotations/Mutable.java
--rw-rw-rw-  2.0 fat     1271 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/main/java/org/jpy/annotations/Output.java
--rw-rw-rw-  2.0 fat     1246 b- defN 14-May-09 14:11 jpy-0.7.4/src/main/java/org/jpy/annotations/Return.java
--rw-rw-rw-  2.0 fat     5325 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/JavaReflectionTest.java
--rw-rw-rw-  2.0 fat     4234 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/java/org/jpy/PyLibTest.java
--rw-rw-rw-  2.0 fat     3280 b- defN 14-Jul-11 13:52 jpy-0.7.4/src/test/java/org/jpy/PyModuleTest.java
--rw-rw-rw-  2.0 fat     8941 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/java/org/jpy/PyObjectTest.java
--rw-rw-rw-  2.0 fat     2954 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/java/org/jpy/UseCases.java
--rw-rw-rw-  2.0 fat     1689 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java
--rw-rw-rw-  2.0 fat     1515 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java
--rw-rw-rw-  2.0 fat     2100 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/FieldTestFixture.java
--rw-rw-rw-  2.0 fat     4087 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java
--rw-rw-rw-  2.0 fat     3852 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java
--rw-rw-rw-  2.0 fat     2426 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java
--rw-rw-rw-  2.0 fat      955 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/Processor.java
--rw-rw-rw-  2.0 fat     1546 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/Thing.java
--rw-rw-rw-  2.0 fat     1427 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java
--rw-rw-rw-  2.0 fat     1253 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java
--rw-rw-rw-  2.0 fat     7640 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/python/jpy_array_test.py
--rw-rw-rw-  2.0 fat     1350 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_diag_test.py
--rw-rw-rw-  2.0 fat     2121 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_exception_test.py
--rw-rw-rw-  2.0 fat     4241 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_field_test.py
--rw-rw-rw-  2.0 fat     2059 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/python/jpy_gettype_test.py
--rw-rw-rw-  2.0 fat     9392 b- defN 14-Jun-03 17:57 jpy-0.7.4/src/test/python/jpy_modretparam_test.py
--rw-rw-rw-  2.0 fat     1070 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_mt_test.py
--rw-rw-rw-  2.0 fat     3879 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_overload_test.py
--rw-rw-rw-  2.0 fat     1347 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_perf_test.py
--rw-rw-rw-  2.0 fat     4201 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_retval_test.py
--rw-rw-rw-  2.0 fat     6542 b- defN 14-Jul-11 11:49 jpy-0.7.4/src/test/python/jpy_rt_test.py
--rw-rw-rw-  2.0 fat     2229 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_typeconv_test.py
--rw-rw-rw-  2.0 fat     1554 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/jpy_typeres_test.py
--rw-rw-rw-  2.0 fat      430 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/fixtures/proc_class.py
--rw-rw-rw-  2.0 fat      306 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/fixtures/proc_module.py
--rw-rw-rw-  2.0 fat       84 b- defN 14-Jul-11 11:35 jpy-0.7.4/src/test/python/fixtures/raise_errors.py
--rw-rw-rw-  2.0 fat     4196 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/imp/import_ex1.py
--rw-rw-rw-  2.0 fat     2461 b- defN 14-May-07 13:22 jpy-0.7.4/src/test/python/imp/import_ex2.py
-78 files, 515835 bytes uncompressed, 130720 bytes compressed:  74.7%
+Zip file size: 144021 bytes, number of entries: 78
+-rw-rw-rw-  2.0 fat     1517 b- defN 14-Jul-24 15:53 jpy-0.7.5/CHANGES.txt
+-rw-rw-rw-  2.0 fat    35795 b- defN 14-May-07 13:22 jpy-0.7.5/LICENSE.txt
+-rw-rw-rw-  2.0 fat     4269 b- defN 14-Jul-24 15:53 jpy-0.7.5/PKG-INFO
+-rw-rw-rw-  2.0 fat     5325 b- defN 14-Jul-24 15:42 jpy-0.7.5/pom.xml
+-rw-rw-rw-  2.0 fat     5491 b- defN 14-Jul-24 15:42 jpy-0.7.5/setup.py
+-rw-rw-rw-  2.0 fat     8445 b- defN 14-May-09 18:06 jpy-0.7.5/doc/conf.py
+-rw-rw-rw-  2.0 fat      607 b- defN 14-May-08 11:33 jpy-0.7.5/doc/index.rst
+-rw-rw-rw-  2.0 fat     8515 b- defN 14-Jun-12 14:00 jpy-0.7.5/doc/install.rst
+-rw-rw-rw-  2.0 fat     5314 b- defN 14-Jul-24 15:45 jpy-0.7.5/doc/intro.rst
+-rwx---     2.0 fat     6695 b- defN 14-May-07 13:22 jpy-0.7.5/doc/make.bat
+-rw-rw-rw-  2.0 fat     6927 b- defN 14-May-07 13:22 jpy-0.7.5/doc/Makefile
+-rw-rw-rw-  2.0 fat     3340 b- defN 14-May-08 12:06 jpy-0.7.5/doc/modify.rst
+-rw-rw-rw-  2.0 fat    23125 b- defN 14-Jun-03 17:57 jpy-0.7.5/doc/reference.rst
+-rw-rw-rw-  2.0 fat     1107 b- defN 14-May-08 11:45 jpy-0.7.5/doc/tutorial.rst
+-rw-rw-rw-  2.0 fat     1036 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_compat.c
+-rw-rw-rw-  2.0 fat     2301 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_compat.h
+-rw-rw-rw-  2.0 fat     7609 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_conv.c
+-rw-rw-rw-  2.0 fat     4054 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_conv.h
+-rw-rw-rw-  2.0 fat     5799 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/main/c/jpy_diag.c
+-rw-rw-rw-  2.0 fat     1514 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_diag.h
+-rw-rw-rw-  2.0 fat    11214 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jarray.c
+-rw-rw-rw-  2.0 fat     1619 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jarray.h
+-rw-rw-rw-  2.0 fat     4732 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/main/c/jpy_jfield.c
+-rw-rw-rw-  2.0 fat     1534 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jfield.h
+-rw-rw-rw-  2.0 fat    30977 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jmethod.c
+-rw-rw-rw-  2.0 fat     3140 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jmethod.h
+-rw-rw-rw-  2.0 fat    28396 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jobj.c
+-rw-rw-rw-  2.0 fat     1266 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jobj.h
+-rw-rw-rw-  2.0 fat    77120 b- defN 14-Jun-30 17:29 jpy-0.7.5/src/main/c/jpy_jtype.c
+-rw-rw-rw-  2.0 fat     4082 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_jtype.h
+-rw-rw-rw-  2.0 fat    33609 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_module.c
+-rw-rw-rw-  2.0 fat     5800 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jpy_module.h
+-rw-rw-rw-  2.0 fat    30633 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.c
+-rw-rw-rw-  2.0 fat     4057 b- defN 14-May-07 13:22 jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.h
+-rw-rw-rw-  2.0 fat      299 b- defN 14-May-07 13:22 jpy-0.7.5/src/main/c/jni/org_jpy_PyLib_CallableKind.h
+-rw-rw-rw-  2.0 fat     1056 b- defN 14-May-07 13:22 jpy-0.7.5/src/main/c/jni/org_jpy_PyLib_Diag.h
+-rw-rw-rw-  2.0 fat     1543 b- defN 14-May-09 14:11 jpy-0.7.5/src/main/java/org/jpy/package-info.java
+-rw-rw-rw-  2.0 fat    13626 b- defN 14-May-09 18:06 jpy-0.7.5/src/main/java/org/jpy/PyLib.java
+-rw-rw-rw-  2.0 fat     2756 b- defN 14-May-09 14:11 jpy-0.7.5/src/main/java/org/jpy/PyLibConfig.java
+-rw-rw-rw-  2.0 fat     2157 b- defN 14-May-09 14:11 jpy-0.7.5/src/main/java/org/jpy/PyModule.java
+-rw-rw-rw-  2.0 fat    10472 b- defN 14-May-12 09:07 jpy-0.7.5/src/main/java/org/jpy/PyObject.java
+-rw-rw-rw-  2.0 fat     2550 b- defN 14-May-12 09:07 jpy-0.7.5/src/main/java/org/jpy/PyProxyHandler.java
+-rw-rw-rw-  2.0 fat     1254 b- defN 14-May-09 14:11 jpy-0.7.5/src/main/java/org/jpy/annotations/Mutable.java
+-rw-rw-rw-  2.0 fat     1271 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/main/java/org/jpy/annotations/Output.java
+-rw-rw-rw-  2.0 fat     1246 b- defN 14-May-09 14:11 jpy-0.7.5/src/main/java/org/jpy/annotations/Return.java
+-rw-rw-rw-  2.0 fat     5325 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/JavaReflectionTest.java
+-rw-rw-rw-  2.0 fat     4234 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/java/org/jpy/PyLibTest.java
+-rw-rw-rw-  2.0 fat     3282 b- defN 14-Jul-24 12:45 jpy-0.7.5/src/test/java/org/jpy/PyModuleTest.java
+-rw-rw-rw-  2.0 fat     8941 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/java/org/jpy/PyObjectTest.java
+-rw-rw-rw-  2.0 fat     2954 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/java/org/jpy/UseCases.java
+-rw-rw-rw-  2.0 fat     1689 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java
+-rw-rw-rw-  2.0 fat     1515 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java
+-rw-rw-rw-  2.0 fat     2100 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/FieldTestFixture.java
+-rw-rw-rw-  2.0 fat     4087 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java
+-rw-rw-rw-  2.0 fat     3852 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java
+-rw-rw-rw-  2.0 fat     2426 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java
+-rw-rw-rw-  2.0 fat      955 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/Processor.java
+-rw-rw-rw-  2.0 fat     1546 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/Thing.java
+-rw-rw-rw-  2.0 fat     1427 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java
+-rw-rw-rw-  2.0 fat     1253 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java
+-rw-rw-rw-  2.0 fat     7640 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/python/jpy_array_test.py
+-rw-rw-rw-  2.0 fat     1350 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_diag_test.py
+-rw-rw-rw-  2.0 fat     2121 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_exception_test.py
+-rw-rw-rw-  2.0 fat     4241 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_field_test.py
+-rw-rw-rw-  2.0 fat     2059 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/python/jpy_gettype_test.py
+-rw-rw-rw-  2.0 fat     9392 b- defN 14-Jun-03 17:57 jpy-0.7.5/src/test/python/jpy_modretparam_test.py
+-rw-rw-rw-  2.0 fat     1070 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_mt_test.py
+-rw-rw-rw-  2.0 fat     3879 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_overload_test.py
+-rw-rw-rw-  2.0 fat     1347 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_perf_test.py
+-rw-rw-rw-  2.0 fat     4201 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_retval_test.py
+-rw-rw-rw-  2.0 fat     6542 b- defN 14-Jul-11 11:49 jpy-0.7.5/src/test/python/jpy_rt_test.py
+-rw-rw-rw-  2.0 fat     2229 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_typeconv_test.py
+-rw-rw-rw-  2.0 fat     1554 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/jpy_typeres_test.py
+-rw-rw-rw-  2.0 fat      430 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/fixtures/proc_class.py
+-rw-rw-rw-  2.0 fat      306 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/fixtures/proc_module.py
+-rw-rw-rw-  2.0 fat       84 b- defN 14-Jul-11 11:35 jpy-0.7.5/src/test/python/fixtures/raise_errors.py
+-rw-rw-rw-  2.0 fat     4196 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/imp/import_ex1.py
+-rw-rw-rw-  2.0 fat     2461 b- defN 14-May-07 13:22 jpy-0.7.5/src/test/python/imp/import_ex2.py
+78 files, 515882 bytes uncompressed, 131587 bytes compressed:  74.5%
```

## zipnote {}

```diff
@@ -1,235 +1,235 @@
-Filename: jpy-0.7.4/CHANGES.txt
+Filename: jpy-0.7.5/CHANGES.txt
 Comment: 
 
-Filename: jpy-0.7.4/LICENSE.txt
+Filename: jpy-0.7.5/LICENSE.txt
 Comment: 
 
-Filename: jpy-0.7.4/PKG-INFO
+Filename: jpy-0.7.5/PKG-INFO
 Comment: 
 
-Filename: jpy-0.7.4/pom.xml
+Filename: jpy-0.7.5/pom.xml
 Comment: 
 
-Filename: jpy-0.7.4/setup.py
+Filename: jpy-0.7.5/setup.py
 Comment: 
 
-Filename: jpy-0.7.4/doc/conf.py
+Filename: jpy-0.7.5/doc/conf.py
 Comment: 
 
-Filename: jpy-0.7.4/doc/index.rst
+Filename: jpy-0.7.5/doc/index.rst
 Comment: 
 
-Filename: jpy-0.7.4/doc/install.rst
+Filename: jpy-0.7.5/doc/install.rst
 Comment: 
 
-Filename: jpy-0.7.4/doc/intro.rst
+Filename: jpy-0.7.5/doc/intro.rst
 Comment: 
 
-Filename: jpy-0.7.4/doc/make.bat
+Filename: jpy-0.7.5/doc/make.bat
 Comment: 
 
-Filename: jpy-0.7.4/doc/Makefile
+Filename: jpy-0.7.5/doc/Makefile
 Comment: 
 
-Filename: jpy-0.7.4/doc/modify.rst
+Filename: jpy-0.7.5/doc/modify.rst
 Comment: 
 
-Filename: jpy-0.7.4/doc/reference.rst
+Filename: jpy-0.7.5/doc/reference.rst
 Comment: 
 
-Filename: jpy-0.7.4/doc/tutorial.rst
+Filename: jpy-0.7.5/doc/tutorial.rst
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_compat.c
+Filename: jpy-0.7.5/src/main/c/jpy_compat.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_compat.h
+Filename: jpy-0.7.5/src/main/c/jpy_compat.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_conv.c
+Filename: jpy-0.7.5/src/main/c/jpy_conv.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_conv.h
+Filename: jpy-0.7.5/src/main/c/jpy_conv.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_diag.c
+Filename: jpy-0.7.5/src/main/c/jpy_diag.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_diag.h
+Filename: jpy-0.7.5/src/main/c/jpy_diag.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jarray.c
+Filename: jpy-0.7.5/src/main/c/jpy_jarray.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jarray.h
+Filename: jpy-0.7.5/src/main/c/jpy_jarray.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jfield.c
+Filename: jpy-0.7.5/src/main/c/jpy_jfield.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jfield.h
+Filename: jpy-0.7.5/src/main/c/jpy_jfield.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jmethod.c
+Filename: jpy-0.7.5/src/main/c/jpy_jmethod.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jmethod.h
+Filename: jpy-0.7.5/src/main/c/jpy_jmethod.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jobj.c
+Filename: jpy-0.7.5/src/main/c/jpy_jobj.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jobj.h
+Filename: jpy-0.7.5/src/main/c/jpy_jobj.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jtype.c
+Filename: jpy-0.7.5/src/main/c/jpy_jtype.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_jtype.h
+Filename: jpy-0.7.5/src/main/c/jpy_jtype.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_module.c
+Filename: jpy-0.7.5/src/main/c/jpy_module.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jpy_module.h
+Filename: jpy-0.7.5/src/main/c/jpy_module.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.c
+Filename: jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.c
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.h
+Filename: jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jni/org_jpy_PyLib_CallableKind.h
+Filename: jpy-0.7.5/src/main/c/jni/org_jpy_PyLib_CallableKind.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/c/jni/org_jpy_PyLib_Diag.h
+Filename: jpy-0.7.5/src/main/c/jni/org_jpy_PyLib_Diag.h
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/package-info.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/package-info.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/PyLib.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/PyLib.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/PyLibConfig.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/PyLibConfig.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/PyModule.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/PyModule.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/PyObject.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/PyObject.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/PyProxyHandler.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/PyProxyHandler.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/annotations/Mutable.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/annotations/Mutable.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/annotations/Output.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/annotations/Output.java
 Comment: 
 
-Filename: jpy-0.7.4/src/main/java/org/jpy/annotations/Return.java
+Filename: jpy-0.7.5/src/main/java/org/jpy/annotations/Return.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/JavaReflectionTest.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/JavaReflectionTest.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/PyLibTest.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/PyLibTest.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/PyModuleTest.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/PyModuleTest.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/PyObjectTest.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/PyObjectTest.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/UseCases.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/UseCases.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/FieldTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/FieldTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/Processor.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/Processor.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/Thing.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/Thing.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java
+Filename: jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_array_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_array_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_diag_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_diag_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_exception_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_exception_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_field_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_field_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_gettype_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_gettype_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_modretparam_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_modretparam_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_mt_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_mt_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_overload_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_overload_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_perf_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_perf_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_retval_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_retval_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_rt_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_rt_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_typeconv_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_typeconv_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/jpy_typeres_test.py
+Filename: jpy-0.7.5/src/test/python/jpy_typeres_test.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/fixtures/proc_class.py
+Filename: jpy-0.7.5/src/test/python/fixtures/proc_class.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/fixtures/proc_module.py
+Filename: jpy-0.7.5/src/test/python/fixtures/proc_module.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/fixtures/raise_errors.py
+Filename: jpy-0.7.5/src/test/python/fixtures/raise_errors.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/imp/import_ex1.py
+Filename: jpy-0.7.5/src/test/python/imp/import_ex1.py
 Comment: 
 
-Filename: jpy-0.7.4/src/test/python/imp/import_ex2.py
+Filename: jpy-0.7.5/src/test/python/imp/import_ex2.py
 Comment: 
 
 Zip file comment:
```

## Comparing `jpy-0.7.4/CHANGES.txt` & `jpy-0.7.5/CHANGES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+*************
+jpy Changelog
+*************
+
+Version 0.7.5
+=============
+
+* Fixed bad pointer in C-code which caused unpredictable crashes (issue #43)
+
 Version 0.7.4
 =============
 
 * Fixed a problem where jpy crashes with unicode arguments (issue #42)
 * Fixed segmentation fault occurring occasionally during installation of jpy (issue #40)
 * Improved Java exception messages on Python errors (issue #39)
```

## Comparing `jpy-0.7.4/LICENSE.txt` & `jpy-0.7.5/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/pom.xml` & `jpy-0.7.5/pom.xml`

 * *Files 1% similar despite different names*

### Comparing `jpy-0.7.4/pom.xml` & `jpy-0.7.5/pom.xml`

```diff
@@ -14,15 +14,15 @@
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <properties>
     <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
   </properties>
   <groupId>org.jpy</groupId>
   <artifactId>jpy</artifactId>
-  <version>0.7.4</version>
+  <version>0.7.5</version>
   <description>jpy is a bi-directional Java-Python bridge which you can use to embed Java code in Python programs or the other
         way round.</description>
   <licenses>
     <license>
       <name>GPL 3</name>
       <url>http://www.gnu.org/licenses/gpl-3.0</url>
       <distribution>repo</distribution>
```

## Comparing `jpy-0.7.4/setup.py` & `jpy-0.7.5/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 __author__ = "Norman Fomferra, Brockmann Consult GmbH"
 __copyright__ = "Copyright (C) 2014 Brockmann Consult GmbH"
 __license__ = "GPL v3"
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 sources = [
     'src/main/c/jpy_module.c',
     'src/main/c/jpy_diag.c',
     'src/main/c/jpy_conv.c',
     'src/main/c/jpy_compat.c',
     'src/main/c/jpy_jtype.c',
@@ -96,18 +96,21 @@
                     JDK_HOME + '/lib',
                     os.path.join(sys.exec_prefix, 'lib')]
 
 
 with open('README.rst') as file:
     long_description = file.read()
 
+with open('CHANGES.txt') as file:
+    changelog = file.read()
+
 
 setup(name='jpy',
       description='Bi-directional Python-Java bridge',
-      long_description=long_description,
+      long_description=long_description + '\n\n' + changelog,
       version=__version__,
       platforms='Python ' + ('3.3+' if ISPY3 else '2.7') + ', Java 1.7',
       author=__author__,
       author_email='norman.fomferra@brockmann-consult.de',
       maintainer='Brockmann Consult GmbH',
       maintainer_email='norman.fomferra@brockmann-consult.de',
       license='GPL 3',
```

## Comparing `jpy-0.7.4/doc/conf.py` & `jpy-0.7.5/doc/conf.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/index.rst` & `jpy-0.7.5/doc/index.rst`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/install.rst` & `jpy-0.7.5/doc/install.rst`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/intro.rst` & `jpy-0.7.5/doc/intro.rst`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 * Support of Java multi-threading
 * Fast and memory-efficient support of primitive Java array parameters via `Python buffers <http://docs.python.org/3.3/c-api/buffer.html>`_
   (e.g. `numpy arrays <http://docs.scipy.org/doc/numpy/reference/arrays.html>`_)
 * Support of Java methods that modify primitive Java array parameters (mutable parameters)
 * Java arrays translate into Python sequence objects
 * Java API for accessing Python objects (``jpy.jar``)
 
-jpy has been tested with Python 2.7 and 3.3 and an Oracle Java 7 JDK. It will presumably also work with Python 2.6 or
+jpy has been tested with Python 2.7, 3.3, 3.4 and  Oracle Java 7 and 8 JDKs. It will presumably also work with Python 2.6 or
 3.2 and a Java 6 JDK.
 
 The initial development of jpy has been driven by the need to write Python extensions to an established scientific
 imaging application programmed in Java, namely the `BEAM <http://www.brockmann-consult.de/beam/>`_ toolbox
 funded by the European Space Agency (ESA).
 Writing such Python plug-ins for a Java application usually requires a bi-directional communication between Python and
 Java since the Python extension code must be able to call back into the Java APIs.
```

## Comparing `jpy-0.7.4/doc/make.bat` & `jpy-0.7.5/doc/make.bat`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/Makefile` & `jpy-0.7.5/doc/Makefile`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/modify.rst` & `jpy-0.7.5/doc/modify.rst`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/reference.rst` & `jpy-0.7.5/doc/reference.rst`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/doc/tutorial.rst` & `jpy-0.7.5/doc/tutorial.rst`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/c/jpy_compat.h` & `jpy-0.7.5/src/main/c/jpy_compat.h`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,66 @@
-#ifndef JPY_COMPAT_H
-#define JPY_COMPAT_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include <Python.h>
-
-
-#if PY_MAJOR_VERSION >= 3
-
-#define JPy_IS_CLONG(pyArg)      PyLong_Check(pyArg)
-#define JPy_AS_CLONG(pyArg)      PyLong_AsLong(pyArg)
-#define JPy_AS_CLONGLONG(pyArg)  PyLong_AsLongLong(pyArg)
-#define JPy_FROM_CLONG(cl)       PyLong_FromLong(cl)
-
-// todo: py27: use the following macros where appropriate
-#define JPy_IS_STR(pyArg)        PyUnicode_Check(pyArg)
-#define JPy_FROM_CSTR(cstr)      PyUnicode_FromString(cstr)
-#define JPy_FROM_FORMAT          PyUnicode_FromFormat
-
-#else
-
-#define JPy_IS_CLONG(pyArg)      (PyInt_Check(pyArg) || PyLong_Check(pyArg))
-#define JPy_AS_CLONG(pyArg)      (PyInt_Check(pyArg) ? PyInt_AsLong(pyArg) : PyLong_AsLong(pyArg))
-#define JPy_AS_CLONGLONG(pyArg)  (PyInt_Check(pyArg) ? PyInt_AsLong(pyArg) : PyLong_AsLongLong(pyArg))
-#define JPy_FROM_CLONG(cl)        PyInt_FromLong(cl)
-
-// todo: py27: use the following macros where appropriate
-#define JPy_IS_STR(pyArg)        (PyString_Check(pyArg) || PyUnicode_Check(pyArg))
-#define JPy_FROM_CSTR(cstr)      PyString_FromString(cstr)
-#define JPy_FROM_FORMAT          PyString_FromFormat
-
-#endif
-
-
-
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
-
-#define JPy_AS_UTF8(unicode)                 PyUnicode_AsUTF8(unicode)
-#define JPy_AS_WIDE_CHAR_STR(unicode, size)  PyUnicode_AsWideCharString(unicode, size)
-#define JPy_FROM_WIDE_CHAR_STR(wc, size)     PyUnicode_FromKindAndData(PyUnicode_2BYTE_KIND, wc, size)
-
-#else
-
-// Implement conversion rules from Python 2 to 3 as given here:
-// https://docs.python.org/3.3/howto/cporting.html
-// http://lucumr.pocoo.org/2011/1/22/forwards-compatible-python/
-
-const char* JPy_AsUTF8_PriorToPy33(PyObject* unicode);
-wchar_t* JPy_AsWideCharString_PriorToPy33(PyObject *unicode, Py_ssize_t *size);
-
-#define JPy_AS_UTF8(unicode)                 JPy_AsUTF8_PriorToPy33(unicode)
-#define JPy_AS_WIDE_CHAR_STR(unicode, size)  JPy_AsWideCharString_PriorToPy33(unicode, size)
-#define JPy_FROM_WIDE_CHAR_STR(wc, size)     PyUnicode_FromWideChar(wc, size)
-
-#endif
-
-
-#ifdef __cplusplus
-} /* extern "C" */
-#endif
+#ifndef JPY_COMPAT_H
+#define JPY_COMPAT_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include <Python.h>
+
+#define JPY_VERSION_ERROR "jpy requires either Python 2.7 or Python 3.3+"
+
+#if PY_MAJOR_VERSION == 2 && PY_MINOR_VERSION == 7
+#define JPY_COMPAT_27 1
+#undef JPY_COMPAT_33P
+#elif PY_MAJOR_VERSION == 3 && PY_MINOR_VERSION >= 3
+#define JPY_COMPAT_33P 1
+#undef JPY_COMPAT_27
+#else
+#error JPY_VERSION_ERROR
+#endif
+
+
+#if defined(JPY_COMPAT_33P)
+
+#define JPy_IS_CLONG(pyArg)      PyLong_Check(pyArg)
+#define JPy_AS_CLONG(pyArg)      PyLong_AsLong(pyArg)
+#define JPy_AS_CLONGLONG(pyArg)  PyLong_AsLongLong(pyArg)
+#define JPy_FROM_CLONG(cl)       PyLong_FromLong(cl)
+
+#define JPy_IS_STR(pyArg)        PyUnicode_Check(pyArg)
+#define JPy_FROM_CSTR(cstr)      PyUnicode_FromString(cstr)
+#define JPy_FROM_FORMAT          PyUnicode_FromFormat
+
+#define JPy_AS_UTF8(unicode)                 PyUnicode_AsUTF8(unicode)
+#define JPy_AS_WIDE_CHAR_STR(unicode, size)  PyUnicode_AsWideCharString(unicode, size)
+#define JPy_FROM_WIDE_CHAR_STR(wc, size)     PyUnicode_FromKindAndData(PyUnicode_2BYTE_KIND, wc, size)
+
+#elif defined(JPY_COMPAT_27)
+
+#define JPy_IS_CLONG(pyArg)      (PyInt_Check(pyArg) || PyLong_Check(pyArg))
+#define JPy_AS_CLONG(pyArg)      (PyInt_Check(pyArg) ? PyInt_AsLong(pyArg) : PyLong_AsLong(pyArg))
+#define JPy_AS_CLONGLONG(pyArg)  (PyInt_Check(pyArg) ? PyInt_AsLong(pyArg) : PyLong_AsLongLong(pyArg))
+#define JPy_FROM_CLONG(cl)        PyInt_FromLong(cl)
+
+#define JPy_IS_STR(pyArg)        (PyString_Check(pyArg) || PyUnicode_Check(pyArg))
+#define JPy_FROM_CSTR(cstr)      PyString_FromString(cstr)
+#define JPy_FROM_FORMAT          PyString_FromFormat
+
+// Implement conversion rules from Python 2 to 3 as given here:
+// https://docs.python.org/3.3/howto/cporting.html
+// http://lucumr.pocoo.org/2011/1/22/forwards-compatible-python/
+
+const char* JPy_AsUTF8_PriorToPy33(PyObject* unicode);
+wchar_t* JPy_AsWideCharString_PriorToPy33(PyObject *unicode, Py_ssize_t *size);
+
+#define JPy_AS_UTF8(unicode)                 JPy_AsUTF8_PriorToPy33(unicode)
+#define JPy_AS_WIDE_CHAR_STR(unicode, size)  JPy_AsWideCharString_PriorToPy33(unicode, size)
+#define JPy_FROM_WIDE_CHAR_STR(wc, size)     PyUnicode_FromWideChar(wc, size)
+
+#endif
+
+
+#ifdef __cplusplus
+} /* extern "C" */
+#endif
 #endif /* !JPY_COMPAT_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_conv.c` & `jpy-0.7.5/src/main/c/jpy_conv.c`

 * *Files 15% similar despite different names*

```diff
@@ -1,292 +1,298 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#include "jpy_module.h"
-#include "jpy_diag.h"
-#include "jpy_jtype.h"
-#include "jpy_jobj.h"
-#include "jpy_conv.h"
-#include "jpy_compat.h"
-
-
-
-int JPy_AsJObject(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef)
-{
-    return JType_ConvertPythonToJavaObject(jenv, JPy_JObject, pyObj, objectRef);
-}
-
-int JPy_AsJObjectWithType(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, JPy_JType* type)
-{
-    return JType_ConvertPythonToJavaObject(jenv, type, pyObj, objectRef);
-}
-
-int JPy_AsJObjectWithClass(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, jclass classRef)
-{
-    *objectRef = NULL;
-
-    if (pyObj == Py_None) {
-        return 0;
-    }
-
-    if (classRef != NULL) {
-        JPy_JType* valueType;
-
-        valueType = JType_GetType(jenv, classRef, JNI_FALSE);
-        if (valueType == NULL) {
-            return -1;
-        }
-        if (JPy_AsJObjectWithType(jenv, pyObj, objectRef, valueType) < 0) {
-            return -1;
-        }
-    } else {
-        if (JPy_AsJObject(jenv, pyObj, objectRef) < 0) {
-            return -1;
-        }
-    }
-
-    return 0;
-}
-
-
-
-PyObject* JPy_FromJObject(JNIEnv* jenv, jobject objectRef)
-{
-    jclass classRef;
-    JPy_JType* type;
-
-    classRef = (*jenv)->GetObjectClass(jenv, objectRef);
-    type = JType_GetType(jenv, classRef, JNI_FALSE);
-    (*jenv)->DeleteLocalRef(jenv, classRef);
-    if (type == NULL) {
-        return NULL;
-    }
-
-    return JPy_FromJObjectWithType(jenv, objectRef, type);
-}
-
-PyObject* JPy_FromJObjectWithType(JNIEnv* jenv, jobject objectRef, JPy_JType* type)
-{
-    return JType_ConvertJavaToPythonObject(jenv, type, objectRef);
-}
-
-
-/**
- * Copies the UTF, zero-terminated C-string.
- * Caller is responsible for freeing the returned string using PyMem_Del().
- */
-char* JPy_CopyUTFString(const char* utfChars)
-{
-    char* utfCharsCopy;
-
-    utfCharsCopy = PyMem_New(char, strlen(utfChars) + 1);
-    if (utfCharsCopy == NULL) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    strcpy(utfCharsCopy, utfChars);
-    return utfCharsCopy;
-}
-
-/**
- * Copies the given jchar string used by Java into a wchar_t string used by Python.
- * Caller is responsible for freeing the returned string using PyMem_Del().
- */
-wchar_t* JPy_ConvertToWCharString(const jchar* jChars, jint length)
-{
-    wchar_t* wChars;
-    jint i;
-
-    wChars = PyMem_New(wchar_t, length + 1);
-    if (wChars == NULL) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    for (i = 0; i < length; i++) {
-        wChars[i] = (wchar_t) jChars[i];
-    }
-    wChars[length] = 0;
-
-    return wChars;
-}
-
-/**
- * Copies the given wchar_t string used by Python into a jchar string used by Python.
- * Caller is responsible for freeing the returned string using PyMem_Del().
- */
-jchar* JPy_ConvertToJCharString(const wchar_t* wChars, jint length)
-{
-    jchar* jChars;
-    jint i;
-
-    jChars = PyMem_New(jchar, length + 1);
-    if (jChars == NULL) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    for (i = 0; i < length; i++) {
-        jChars[i] = (jchar) wChars[i];
-    }
-    jChars[length] = (jchar) 0;
-
-    return jChars;
-}
-
-/**
- * Gets the UTF name of thie given class.
- * Caller is responsible for freeing the returned string using Py_Del().
- */
-char* JPy_GetTypeName(JNIEnv* jenv, jclass classRef)
-{
-    jstring jTypeName;
-    const char* jTypeNameChars;
-    char* typeNameCopy;
-
-    jTypeName = (*jenv)->CallObjectMethod(jenv, classRef, JPy_Class_GetName_MID);
-    JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-
-    jTypeNameChars = (*jenv)->GetStringUTFChars(jenv, jTypeName, NULL);
-    if (jTypeNameChars == NULL) {
-        PyErr_NoMemory();
-        typeNameCopy = NULL;
-    } else {
-        typeNameCopy = JPy_CopyUTFString(jTypeNameChars);
-        (*jenv)->ReleaseStringUTFChars(jenv, jTypeName, jTypeNameChars);
-    }
-    (*jenv)->DeleteLocalRef(jenv, jTypeName);
-    return typeNameCopy;
-}
-
-/**
- * Gets a string object representing the name of the given class.
- * Returns a new reference.
- */
-PyObject* JPy_FromTypeName(JNIEnv* jenv, jclass classRef)
-{
-    PyObject* pyTypeName;
-    jstring jTypeName;
-    const char* jTypeNameChars;
-
-    jTypeName = (*jenv)->CallObjectMethod(jenv, classRef, JPy_Class_GetName_MID);
-    JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-
-    jTypeNameChars = (*jenv)->GetStringUTFChars(jenv, jTypeName, NULL);
-    JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JPy_FromTypeName: classRef=%p, jTypeNameChars=\"%s\"\n", classRef, jTypeNameChars);
-
-    if (jTypeNameChars == NULL) {
-        PyErr_NoMemory();
-        pyTypeName = NULL;
-    } else {
-        pyTypeName = Py_BuildValue("s", jTypeNameChars);
-        (*jenv)->ReleaseStringUTFChars(jenv, jTypeName, jTypeNameChars);
-    }
-    (*jenv)->DeleteLocalRef(jenv, jTypeName);
-    return pyTypeName;
-}
-
-
-PyObject* JPy_FromJString(JNIEnv* jenv, jstring stringRef)
-{
-    PyObject* returnValue;
-#if PY_MAJOR_VERSION >= 3
-    const jchar* jChars;
-    jint length;
-
-    if (stringRef == NULL) {
-        return Py_BuildValue("");
-    }
-
-    length = (*jenv)->GetStringLength(jenv, stringRef);
-    if (length == 0) {
-        return Py_BuildValue("s", "");
-    }
-
-    jChars = (*jenv)->GetStringChars(jenv, stringRef, NULL);
-    if (jChars == NULL) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    returnValue = JPy_FROM_WIDE_CHAR_STR(jChars, length);
-    (*jenv)->ReleaseStringChars(jenv, stringRef, jChars);
-#else
-    const char* utfChars;
-
-    if (stringRef == NULL) {
-        return Py_BuildValue("");
-    }
-
-    utfChars = (*jenv)->GetStringUTFChars(jenv, stringRef, NULL);
-    if (utfChars != NULL) {
-        returnValue = Py_BuildValue("s", utfChars);
-        (*jenv)->ReleaseStringUTFChars(jenv, stringRef, utfChars);
-    } else {
-        PyErr_NoMemory();
-        returnValue = NULL;
-    }
-#endif
-    return returnValue;
-}
-
-/**
- * Returns a new Java string (a local reference).
- */
-int JPy_AsJString(JNIEnv* jenv, PyObject* arg, jstring* stringRef)
-{
-    Py_ssize_t length;
-    wchar_t* wChars;
-
-    if (arg == Py_None) {
-        *stringRef = NULL;
-        return 0;
-    }
-
-#if PY_MAJOR_VERSION < 3
-    if (PyString_Check(arg)) {
-        char* cstr = PyString_AsString(arg);
-        *stringRef = (*jenv)->NewStringUTF(jenv, cstr);
-        return *stringRef != NULL ? 0 : -1;
-    }
-#endif
-
-    wChars = JPy_AS_WIDE_CHAR_STR(arg, &length);
-    if (wChars == NULL) {
-        *stringRef = NULL;
-        return -1;
-    }
-
-    if (sizeof(wchar_t) == sizeof(jchar)) {
-        *stringRef = (*jenv)->NewString(jenv, (const jchar*) wChars, length);
-    } else {
-        jchar* jChars;
-        jChars = JPy_ConvertToJCharString(wChars, length);
-        if (jChars == NULL) {
-            goto error;
-        }
-        *stringRef = (*jenv)->NewString(jenv, jChars, length);
-        PyMem_Del(jChars);
-    }
-    if (*stringRef == NULL) {
-        PyMem_Del(wChars);
-        PyErr_NoMemory();
-        return -1;
-    }
-
-error:
-    PyMem_Del(wChars);
-
-    return 0;
-}
-
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#include "jpy_module.h"
+#include "jpy_diag.h"
+#include "jpy_jtype.h"
+#include "jpy_jobj.h"
+#include "jpy_conv.h"
+#include "jpy_compat.h"
+
+
+
+int JPy_AsJObject(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef)
+{
+    return JType_ConvertPythonToJavaObject(jenv, JPy_JObject, pyObj, objectRef);
+}
+
+int JPy_AsJObjectWithType(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, JPy_JType* type)
+{
+    return JType_ConvertPythonToJavaObject(jenv, type, pyObj, objectRef);
+}
+
+int JPy_AsJObjectWithClass(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, jclass classRef)
+{
+    *objectRef = NULL;
+
+    if (pyObj == Py_None) {
+        return 0;
+    }
+
+    if (classRef != NULL) {
+        JPy_JType* valueType;
+
+        valueType = JType_GetType(jenv, classRef, JNI_FALSE);
+        if (valueType == NULL) {
+            return -1;
+        }
+        if (JPy_AsJObjectWithType(jenv, pyObj, objectRef, valueType) < 0) {
+            return -1;
+        }
+    } else {
+        if (JPy_AsJObject(jenv, pyObj, objectRef) < 0) {
+            return -1;
+        }
+    }
+
+    return 0;
+}
+
+
+
+PyObject* JPy_FromJObject(JNIEnv* jenv, jobject objectRef)
+{
+    jclass classRef;
+    JPy_JType* type;
+
+    classRef = (*jenv)->GetObjectClass(jenv, objectRef);
+    type = JType_GetType(jenv, classRef, JNI_FALSE);
+    (*jenv)->DeleteLocalRef(jenv, classRef);
+    if (type == NULL) {
+        return NULL;
+    }
+
+    return JPy_FromJObjectWithType(jenv, objectRef, type);
+}
+
+PyObject* JPy_FromJObjectWithType(JNIEnv* jenv, jobject objectRef, JPy_JType* type)
+{
+    return JType_ConvertJavaToPythonObject(jenv, type, objectRef);
+}
+
+
+/**
+ * Copies the UTF, zero-terminated C-string.
+ * Caller is responsible for freeing the returned string using PyMem_Del().
+ */
+char* JPy_CopyUTFString(const char* utfChars)
+{
+    char* utfCharsCopy;
+
+    utfCharsCopy = PyMem_New(char, strlen(utfChars) + 1);
+    if (utfCharsCopy == NULL) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    strcpy(utfCharsCopy, utfChars);
+    return utfCharsCopy;
+}
+
+/**
+ * Copies the given jchar string used by Java into a wchar_t string used by Python.
+ * Caller is responsible for freeing the returned string using PyMem_Del().
+ */
+wchar_t* JPy_ConvertToWCharString(const jchar* jChars, jint length)
+{
+    wchar_t* wChars;
+    jint i;
+
+    wChars = PyMem_New(wchar_t, length + 1);
+    if (wChars == NULL) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    for (i = 0; i < length; i++) {
+        wChars[i] = (wchar_t) jChars[i];
+    }
+    wChars[length] = 0;
+
+    return wChars;
+}
+
+/**
+ * Copies the given wchar_t string used by Python into a jchar string used by Python.
+ * Caller is responsible for freeing the returned string using PyMem_Del().
+ */
+jchar* JPy_ConvertToJCharString(const wchar_t* wChars, jint length)
+{
+    jchar* jChars;
+    jint i;
+
+    jChars = PyMem_New(jchar, length + 1);
+    if (jChars == NULL) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    for (i = 0; i < length; i++) {
+        jChars[i] = (jchar) wChars[i];
+    }
+    jChars[length] = (jchar) 0;
+
+    return jChars;
+}
+
+/**
+ * Gets the UTF name of thie given class.
+ * Caller is responsible for freeing the returned string using Py_Del().
+ */
+char* JPy_GetTypeName(JNIEnv* jenv, jclass classRef)
+{
+    jstring jTypeName;
+    const char* jTypeNameChars;
+    char* typeNameCopy;
+
+    jTypeName = (*jenv)->CallObjectMethod(jenv, classRef, JPy_Class_GetName_MID);
+    JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+
+    jTypeNameChars = (*jenv)->GetStringUTFChars(jenv, jTypeName, NULL);
+    if (jTypeNameChars == NULL) {
+        PyErr_NoMemory();
+        typeNameCopy = NULL;
+    } else {
+        typeNameCopy = JPy_CopyUTFString(jTypeNameChars);
+        (*jenv)->ReleaseStringUTFChars(jenv, jTypeName, jTypeNameChars);
+    }
+    (*jenv)->DeleteLocalRef(jenv, jTypeName);
+    return typeNameCopy;
+}
+
+/**
+ * Gets a string object representing the name of the given class.
+ * Returns a new reference.
+ */
+PyObject* JPy_FromTypeName(JNIEnv* jenv, jclass classRef)
+{
+    PyObject* pyTypeName;
+    jstring jTypeName;
+    const char* jTypeNameChars;
+
+    jTypeName = (*jenv)->CallObjectMethod(jenv, classRef, JPy_Class_GetName_MID);
+    JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+
+    jTypeNameChars = (*jenv)->GetStringUTFChars(jenv, jTypeName, NULL);
+    JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JPy_FromTypeName: classRef=%p, jTypeNameChars=\"%s\"\n", classRef, jTypeNameChars);
+
+    if (jTypeNameChars == NULL) {
+        PyErr_NoMemory();
+        pyTypeName = NULL;
+    } else {
+        pyTypeName = Py_BuildValue("s", jTypeNameChars);
+        (*jenv)->ReleaseStringUTFChars(jenv, jTypeName, jTypeNameChars);
+    }
+    (*jenv)->DeleteLocalRef(jenv, jTypeName);
+    return pyTypeName;
+}
+
+
+PyObject* JPy_FromJString(JNIEnv* jenv, jstring stringRef)
+{
+    PyObject* returnValue;
+
+#if defined(JPY_COMPAT_33P)
+
+    const jchar* jChars;
+    jint length;
+
+    if (stringRef == NULL) {
+        return Py_BuildValue("");
+    }
+
+    length = (*jenv)->GetStringLength(jenv, stringRef);
+    if (length == 0) {
+        return Py_BuildValue("s", "");
+    }
+
+    jChars = (*jenv)->GetStringChars(jenv, stringRef, NULL);
+    if (jChars == NULL) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    returnValue = JPy_FROM_WIDE_CHAR_STR(jChars, length);
+    (*jenv)->ReleaseStringChars(jenv, stringRef, jChars);
+
+#elif defined(JPY_COMPAT_27)
+
+    const char* utfChars;
+
+    if (stringRef == NULL) {
+        return Py_BuildValue("");
+    }
+
+    utfChars = (*jenv)->GetStringUTFChars(jenv, stringRef, NULL);
+    if (utfChars != NULL) {
+        returnValue = Py_BuildValue("s", utfChars);
+        (*jenv)->ReleaseStringUTFChars(jenv, stringRef, utfChars);
+    } else {
+        PyErr_NoMemory();
+        returnValue = NULL;
+    }
+#else
+    #error JPY_VERSION_ERROR
+#endif
+    return returnValue;
+}
+
+/**
+ * Returns a new Java string (a local reference).
+ */
+int JPy_AsJString(JNIEnv* jenv, PyObject* arg, jstring* stringRef)
+{
+    Py_ssize_t length;
+    wchar_t* wChars;
+
+    if (arg == Py_None) {
+        *stringRef = NULL;
+        return 0;
+    }
+
+#if defined(JPY_COMPAT_27)
+    if (PyString_Check(arg)) {
+        char* cstr = PyString_AsString(arg);
+        *stringRef = (*jenv)->NewStringUTF(jenv, cstr);
+        return *stringRef != NULL ? 0 : -1;
+    }
+#endif
+
+    wChars = JPy_AS_WIDE_CHAR_STR(arg, &length);
+    if (wChars == NULL) {
+        *stringRef = NULL;
+        return -1;
+    }
+
+    if (sizeof(wchar_t) == sizeof(jchar)) {
+        *stringRef = (*jenv)->NewString(jenv, (const jchar*) wChars, length);
+    } else {
+        jchar* jChars;
+        jChars = JPy_ConvertToJCharString(wChars, length);
+        if (jChars == NULL) {
+            goto error;
+        }
+        *stringRef = (*jenv)->NewString(jenv, jChars, length);
+        PyMem_Del(jChars);
+    }
+    if (*stringRef == NULL) {
+        PyMem_Del(wChars);
+        PyErr_NoMemory();
+        return -1;
+    }
+
+error:
+    PyMem_Del(wChars);
+
+    return 0;
+}
+
```

## Comparing `jpy-0.7.4/src/main/c/jpy_conv.h` & `jpy-0.7.5/src/main/c/jpy_conv.h`

 * *Files 21% similar despite different names*

```diff
@@ -1,113 +1,117 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_CONV_H
-#define JPY_CONV_H
-
-#include "jpy_compat.h"
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#define JPy_AS_JBOOLEAN(pyArg)   (jboolean) (pyArg == Py_True ? 1 : (pyArg == Py_False || pyArg == Py_None) ? 0 : (JPy_AS_CLONG(pyArg)) != 0)
-#define JPy_AS_JCHAR(pyArg)      (jchar) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
-#define JPy_AS_JBYTE(pyArg)      (jbyte) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
-#define JPy_AS_JSHORT(pyArg)     (jshort) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
-#define JPy_AS_JINT(pyArg)       (jint) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
-#define JPy_AS_JLONG(pyArg)      (jlong) (pyArg == Py_None ? 0 : JPy_AS_CLONGLONG(pyArg))
-#define JPy_AS_JFLOAT(pyArg)     (jfloat) (pyArg == Py_None ? 0 : PyFloat_AsDouble(pyArg))
-#define JPy_AS_JDOUBLE(pyArg)    (jdouble) (pyArg == Py_None ? 0 : PyFloat_AsDouble(pyArg))
-
-#if PY_MAJOR_VERSION >= 3
-
-#define JPy_FROM_JBOOLEAN(jArg)  PyBool_FromLong(jArg)
-#define JPy_FROM_JCHAR(jArg)     PyLong_FromLong(jArg)
-#define JPy_FROM_JBYTE(jArg)     PyLong_FromLong(jArg)
-#define JPy_FROM_JSHORT(jArg)    PyLong_FromLong(jArg)
-#define JPy_FROM_JINT(jArg)      PyLong_FromLong(jArg)
-#define JPy_FROM_JLONG(jArg)     PyLong_FromLongLong(jArg)
-#define JPy_FROM_JFLOAT(jArg)    PyFloat_FromDouble(jArg)
-#define JPy_FROM_JDOUBLE(jArg)   PyFloat_FromDouble(jArg)
-
-#else
-
-#define JPy_FROM_JBOOLEAN(jArg)  PyBool_FromLong(jArg)
-#define JPy_FROM_JCHAR(jArg)     PyInt_FromLong(jArg)
-#define JPy_FROM_JBYTE(jArg)     PyInt_FromLong(jArg)
-#define JPy_FROM_JSHORT(jArg)    PyInt_FromLong(jArg)
-#define JPy_FROM_JINT(jArg)      PyLong_FromLong(jArg)
-#define JPy_FROM_JLONG(jArg)     PyLong_FromLongLong(jArg)
-#define JPy_FROM_JFLOAT(jArg)    PyFloat_FromDouble(jArg)
-#define JPy_FROM_JDOUBLE(jArg)   PyFloat_FromDouble(jArg)
-
-#endif
-
-#define JPy_FROM_JVOID()         Py_BuildValue("")
-#define JPy_FROM_JNULL()         Py_BuildValue("")
-
-
-/**
- * Convert Java string to Python unicode object.
- */
-PyObject* JPy_FromJString(JNIEnv* jenv, jstring stringRef);
-
-/**
- * Convert any Java Object to Python Object.
- */
-PyObject* JPy_FromJObject(JNIEnv* jenv, jobject objectRef);
-
-/**
- * Convert any Java Object of known type to Python Object.
- */
-PyObject* JPy_FromJObjectWithType(JNIEnv* jenv, jobject objectRef, JPy_JType* type);
-
-/**
- * Convert Python unicode object to Java String.
- */
-int JPy_AsJString(JNIEnv* jenv, PyObject* pyObj, jstring* stringRef);
-
-/**
- * Convert any Python objects to Java object.
- */
-int JPy_AsJObject(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef);
-
-/**
- * Convert Python objects to Java object with known type.
- */
-int JPy_AsJObjectWithType(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, JPy_JType* type);
-
-/**
- * Convert Python objects to Java object with known type.
- */
-int JPy_AsJObjectWithClass(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, jclass classRef);
-
-
-/**
- * Creates a Python unicode object representing the name of the given class.
- * Returns a new reference.
- */
-PyObject* JPy_FromTypeName(JNIEnv* jenv, jclass classRef);
-
-/**
- * Gets the UTF8-encoded name of the given Java type.
- * Caller is responsible for freeing the returned string using PyMem_Del().
- */
-char* JPy_GetTypeName(JNIEnv* jenv, jclass classRef);
-
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
-
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_CONV_H
+#define JPY_CONV_H
+
+#include "jpy_compat.h"
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#define JPy_AS_JBOOLEAN(pyArg)   (jboolean) (pyArg == Py_True ? 1 : (pyArg == Py_False || pyArg == Py_None) ? 0 : (JPy_AS_CLONG(pyArg)) != 0)
+#define JPy_AS_JCHAR(pyArg)      (jchar) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
+#define JPy_AS_JBYTE(pyArg)      (jbyte) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
+#define JPy_AS_JSHORT(pyArg)     (jshort) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
+#define JPy_AS_JINT(pyArg)       (jint) (pyArg == Py_None ? 0 : JPy_AS_CLONG(pyArg))
+#define JPy_AS_JLONG(pyArg)      (jlong) (pyArg == Py_None ? 0 : JPy_AS_CLONGLONG(pyArg))
+#define JPy_AS_JFLOAT(pyArg)     (jfloat) (pyArg == Py_None ? 0 : PyFloat_AsDouble(pyArg))
+#define JPy_AS_JDOUBLE(pyArg)    (jdouble) (pyArg == Py_None ? 0 : PyFloat_AsDouble(pyArg))
+
+#if defined(JPY_COMPAT_33P)
+
+#define JPy_FROM_JBOOLEAN(jArg)  PyBool_FromLong(jArg)
+#define JPy_FROM_JCHAR(jArg)     PyLong_FromLong(jArg)
+#define JPy_FROM_JBYTE(jArg)     PyLong_FromLong(jArg)
+#define JPy_FROM_JSHORT(jArg)    PyLong_FromLong(jArg)
+#define JPy_FROM_JINT(jArg)      PyLong_FromLong(jArg)
+#define JPy_FROM_JLONG(jArg)     PyLong_FromLongLong(jArg)
+#define JPy_FROM_JFLOAT(jArg)    PyFloat_FromDouble(jArg)
+#define JPy_FROM_JDOUBLE(jArg)   PyFloat_FromDouble(jArg)
+
+#elif defined(JPY_COMPAT_27)
+
+#define JPy_FROM_JBOOLEAN(jArg)  PyBool_FromLong(jArg)
+#define JPy_FROM_JCHAR(jArg)     PyInt_FromLong(jArg)
+#define JPy_FROM_JBYTE(jArg)     PyInt_FromLong(jArg)
+#define JPy_FROM_JSHORT(jArg)    PyInt_FromLong(jArg)
+#define JPy_FROM_JINT(jArg)      PyLong_FromLong(jArg)
+#define JPy_FROM_JLONG(jArg)     PyLong_FromLongLong(jArg)
+#define JPy_FROM_JFLOAT(jArg)    PyFloat_FromDouble(jArg)
+#define JPy_FROM_JDOUBLE(jArg)   PyFloat_FromDouble(jArg)
+
+#else
+
+#error JPY_VERSION_ERROR
+
+#endif
+
+#define JPy_FROM_JVOID()         Py_BuildValue("")
+#define JPy_FROM_JNULL()         Py_BuildValue("")
+
+
+/**
+ * Convert Java string to Python unicode object.
+ */
+PyObject* JPy_FromJString(JNIEnv* jenv, jstring stringRef);
+
+/**
+ * Convert any Java Object to Python Object.
+ */
+PyObject* JPy_FromJObject(JNIEnv* jenv, jobject objectRef);
+
+/**
+ * Convert any Java Object of known type to Python Object.
+ */
+PyObject* JPy_FromJObjectWithType(JNIEnv* jenv, jobject objectRef, JPy_JType* type);
+
+/**
+ * Convert Python unicode object to Java String.
+ */
+int JPy_AsJString(JNIEnv* jenv, PyObject* pyObj, jstring* stringRef);
+
+/**
+ * Convert any Python objects to Java object.
+ */
+int JPy_AsJObject(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef);
+
+/**
+ * Convert Python objects to Java object with known type.
+ */
+int JPy_AsJObjectWithType(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, JPy_JType* type);
+
+/**
+ * Convert Python objects to Java object with known type.
+ */
+int JPy_AsJObjectWithClass(JNIEnv* jenv, PyObject* pyObj, jobject* objectRef, jclass classRef);
+
+
+/**
+ * Creates a Python unicode object representing the name of the given class.
+ * Returns a new reference.
+ */
+PyObject* JPy_FromTypeName(JNIEnv* jenv, jclass classRef);
+
+/**
+ * Gets the UTF8-encoded name of the given Java type.
+ * Caller is responsible for freeing the returned string using PyMem_Del().
+ */
+char* JPy_GetTypeName(JNIEnv* jenv, jclass classRef);
+
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
+
 #endif /* !JPY_CONV_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_diag.c` & `jpy-0.7.5/src/main/c/jpy_diag.c`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/c/jpy_diag.h` & `jpy-0.7.5/src/main/c/jpy_diag.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,59 +1,61 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_DIAG_H
-#define JPY_DIAG_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-typedef struct JPy_Diag
-{
-    PyObject_HEAD
-    int flags;
-    int F_OFF;
-    int F_TYPE;
-    int F_METH;
-    int F_EXEC;
-    int F_MEM;
-    int F_JVM;
-    int F_ERR;
-    int F_ALL;
-}
-JPy_Diag;
-
-
-#define JPy_DIAG_F_OFF    0x00
-#define JPy_DIAG_F_TYPE   0x01
-#define JPy_DIAG_F_METH   0x02
-#define JPy_DIAG_F_EXEC   0x04
-#define JPy_DIAG_F_MEM    0x08
-#define JPy_DIAG_F_JVM    0x10
-#define JPy_DIAG_F_ERR    0x20
-#define JPy_DIAG_F_ALL    0xff
-
-extern PyTypeObject Diag_Type;
-extern int JPy_DiagFlags;
-
-PyObject* Diag_New(void);
-
-void JPy_DiagPrint(int diagFlags, const char * format, ...);
-
-#define JPy_DIAG_PRINT if (JPy_DiagFlags != 0) JPy_DiagPrint
-
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_DIAG_H
+#define JPY_DIAG_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+typedef struct JPy_Diag
+{
+    PyObject_HEAD
+    int flags;
+    int F_OFF;
+    int F_TYPE;
+    int F_METH;
+    int F_EXEC;
+    int F_MEM;
+    int F_JVM;
+    int F_ERR;
+    int F_ALL;
+}
+JPy_Diag;
+
+
+#define JPy_DIAG_F_OFF    0x00
+#define JPy_DIAG_F_TYPE   0x01
+#define JPy_DIAG_F_METH   0x02
+#define JPy_DIAG_F_EXEC   0x04
+#define JPy_DIAG_F_MEM    0x08
+#define JPy_DIAG_F_JVM    0x10
+#define JPy_DIAG_F_ERR    0x20
+#define JPy_DIAG_F_ALL    0xff
+
+extern PyTypeObject Diag_Type;
+extern int JPy_DiagFlags;
+
+PyObject* Diag_New(void);
+
+void JPy_DiagPrint(int diagFlags, const char * format, ...);
+
+#define JPy_DIAG_PRINT if (JPy_DiagFlags != 0) JPy_DiagPrint
+
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
 #endif /* !JPY_DIAG_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jarray.c` & `jpy-0.7.5/src/main/c/jpy_jarray.c`

 * *Files 19% similar despite different names*

```diff
@@ -1,351 +1,355 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#include "jpy_module.h"
-#include "jpy_diag.h"
-#include "jpy_jarray.h"
-
-
-#define PRINT_FLAG(F) printf("JArray_GetBufferProc: %s = %d\n", #F, (flags & F) != 0);
-#define PRINT_MEMB(F, M) printf("JArray_GetBufferProc: %s = " ## F ## "\n", #M, M);
-
-//#define JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL 1
-
-
-/*
- * Implements the getbuffer() method of the buffer protocol for JPy_JArray objects.
- * Regarding the format parameter, refer to the Python 'struct' module documentation:
- * http://docs.python.org/2/library/struct.html#module-struct
- */
-int JArray_GetBufferProc(JPy_JArray* self, Py_buffer* view, int flags, char javaType, jint itemSize, const char* format)
-{
-    JNIEnv* jenv;
-    jint itemCount;
-    jboolean isCopy;
-    void* buf;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
-
-    /*
-    printf("JArray_GetBufferProc:\n");
-    PRINT_FLAG(PyBUF_ANY_CONTIGUOUS);
-    PRINT_FLAG(PyBUF_CONTIG);
-    PRINT_FLAG(PyBUF_CONTIG_RO);
-    PRINT_FLAG(PyBUF_C_CONTIGUOUS);
-    PRINT_FLAG(PyBUF_FORMAT);
-    PRINT_FLAG(PyBUF_FULL);
-    PRINT_FLAG(PyBUF_FULL_RO);
-    PRINT_FLAG(PyBUF_F_CONTIGUOUS);
-    PRINT_FLAG(PyBUF_INDIRECT);
-    PRINT_FLAG(PyBUF_ND);
-    PRINT_FLAG(PyBUF_READ);
-    PRINT_FLAG(PyBUF_RECORDS);
-    PRINT_FLAG(PyBUF_RECORDS_RO);
-    PRINT_FLAG(PyBUF_SIMPLE);
-    PRINT_FLAG(PyBUF_STRIDED);
-    PRINT_FLAG(PyBUF_STRIDED_RO);
-    PRINT_FLAG(PyBUF_STRIDES);
-    PRINT_FLAG(PyBUF_WRITE);
-    PRINT_FLAG(PyBUF_WRITEABLE);
-    */
-
-    itemCount = (*jenv)->GetArrayLength(jenv, self->objectRef);
-
-    // According to Python documentation,
-    // buffer allocation shall be done in the 5 following steps;
-
-    // Step 1/5
-#ifdef JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL
-    buf = (*jenv)->GetPrimitiveArrayCritical(jenv, self->objectRef, &isCopy);
-#else
-    if (javaType == 'Z') {
-        buf = (*jenv)->GetBooleanArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'C') {
-        buf = (*jenv)->GetCharArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'B') {
-        buf = (*jenv)->GetByteArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'S') {
-        buf = (*jenv)->GetShortArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'I') {
-        buf = (*jenv)->GetIntArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'J') {
-        buf = (*jenv)->GetLongArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'F') {
-        buf = (*jenv)->GetFloatArrayElements(jenv, self->objectRef, &isCopy);
-    } else if (javaType == 'D') {
-        buf = (*jenv)->GetDoubleArrayElements(jenv, self->objectRef, &isCopy);
-    } else {
-        PyErr_Format(PyExc_RuntimeError, "internal error: illegal Java array type '%c'", javaType);
-        return -1;
-    }
-#endif
-    if (buf == NULL) {
-        PyErr_NoMemory();
-        return -1;
-    }
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JArray_GetBufferProc: buf=%p, type='%s', format='%s', itemSize=%d, itemCount=%d, isCopy=%d\n", buf, Py_TYPE(self)->tp_name, format, itemSize, itemCount, isCopy);
-
-    // Step 2/5
-    view->buf = buf;
-    view->len = itemCount * itemSize;
-    view->itemsize = itemSize;
-    view->readonly = (flags & (PyBUF_WRITE | PyBUF_WRITEABLE)) == 0;
-    view->ndim = 1;
-    view->shape = PyMem_New(Py_ssize_t, 1);
-    *view->shape = itemCount;
-    view->strides = PyMem_New(Py_ssize_t, 1);
-    *view->strides = itemSize;
-    view->suboffsets = NULL;
-    if ((flags & PyBUF_FORMAT) != 0) {
-        view->format = (char*) format;
-    } else {
-        view->format = (char*) "B";
-    }
-
-    /*
-    PRINT_MEMB("%d", view->len);
-    PRINT_MEMB("%d", view->ndim);
-    PRINT_MEMB("%s", view->format);
-    PRINT_MEMB("%d", view->itemsize);
-    PRINT_MEMB("%d", view->readonly);
-    PRINT_MEMB("%d", view->shape[0]);
-    PRINT_MEMB("%d", view->strides[0]);
-    */
-
-    // Step 3/5
-    self->bufferExportCount++;
-
-    // Step 4/5
-    view->obj = (PyObject*) self;
-    Py_INCREF(view->obj);
-
-    // Step 5/5
-    return 0;
-}
-
-int JArray_getbufferproc_boolean(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'Z', 1, "B");
-}
-
-int JArray_getbufferproc_char(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'C', 2, "H");
-}
-
-int JArray_getbufferproc_byte(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'B', 1, "b");
-}
-
-int JArray_getbufferproc_short(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'S', 2, "h");
-}
-
-int JArray_getbufferproc_int(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'I', 4, "i");
-}
-
-int JArray_getbufferproc_long(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'J', 8, "q");
-}
-
-int JArray_getbufferproc_float(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'F', 4, "f");
-}
-
-int JArray_getbufferproc_double(JPy_JArray* self, Py_buffer* view, int flags)
-{
-    return JArray_GetBufferProc(self, view, flags, 'D', 8, "d");
-}
-
-
-/*
- * Implements the releasebuffer() method the buffer protocol for JPy_JArray objects
- */
-void JArray_ReleaseBufferProc(JPy_JArray* self, Py_buffer* view, char javaType)
-{
-    // Step 1
-    self->bufferExportCount--;
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JArray_ReleaseBufferProc: buf=%p, bufferExportCount=%d\n", view->buf, self->bufferExportCount);
-
-    // Step 2
-    if (self->bufferExportCount == 0 && view->buf != NULL) {
-        JNIEnv* jenv = JPy_GetJNIEnv();
-        if (jenv != NULL) {
-#ifdef JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL
-           (*jenv)->ReleasePrimitiveArrayCritical(jenv, self->objectRef, view->buf, 0);
-#else
-            if (javaType == 'Z') {
-                (*jenv)->ReleaseBooleanArrayElements(jenv, self->objectRef, (jboolean*) view->buf, 0);
-            } else if (javaType == 'C') {
-                (*jenv)->ReleaseCharArrayElements(jenv, self->objectRef, (jchar*) view->buf, 0);
-            } else if (javaType == 'B') {
-                (*jenv)->ReleaseByteArrayElements(jenv, self->objectRef, (jbyte*) view->buf, 0);
-            } else if (javaType == 'S') {
-                (*jenv)->ReleaseShortArrayElements(jenv, self->objectRef, (jshort*) view->buf, 0);
-            } else if (javaType == 'I') {
-                (*jenv)->ReleaseIntArrayElements(jenv, self->objectRef, (jint*) view->buf, 0);
-            } else if (javaType == 'J') {
-                (*jenv)->ReleaseLongArrayElements(jenv, self->objectRef, (jlong*) view->buf, 0);
-            } else if (javaType == 'F') {
-                (*jenv)->ReleaseFloatArrayElements(jenv, self->objectRef, (jfloat*) view->buf, 0);
-            } else if (javaType == 'D') {
-                (*jenv)->ReleaseDoubleArrayElements(jenv, self->objectRef, (jdouble*) view->buf, 0);
-            }
-#endif
-        }
-        view->buf = NULL;
-    }
-
-    // todo - check if we must Py_DECREF here
-    //Py_DECREF(view->obj);
-}
-
-// todo: py27: fix all releasebufferproc() functions which have different parameter types in 2.7
-
-void JArray_releasebufferproc_boolean(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'Z');
-}
-
-void JArray_releasebufferproc_char(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'C');
-}
-
-void JArray_releasebufferproc_byte(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'B');
-}
-
-void JArray_releasebufferproc_short(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'S');
-}
-
-void JArray_releasebufferproc_int(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'I');
-}
-
-void JArray_releasebufferproc_long(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'J');
-}
-
-void JArray_releasebufferproc_float(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'F');
-}
-
-void JArray_releasebufferproc_double(JPy_JArray* self, Py_buffer* view)
-{
-    JArray_ReleaseBufferProc(self, view, 'D');
-}
-
-// PyBufferProcs 3.x
-//
-// struct PyBufferProcs {
-//    getbufferproc bf_getbuffer;
-//    releasebufferproc bf_releasebuffer;
-// }
-//
-// PyBufferProcs 2.6 and 2.7 (3.x backport)
-//
-// struct PyBufferProcs {
-//    readbufferproc bf_getreadbuffer;
-//    writebufferproc bf_getwritebuffer;
-//    segcountproc bf_getsegcount;
-//    charbufferproc bf_getcharbuffer;
-//    getbufferproc bf_getbuffer;
-//    releasebufferproc bf_releasebuffer;
-// }
-//
-// PyBufferProcs <= 2.5 (not supported by jpy)
-//
-// struct PyBufferProcs {
-//    readbufferproc bf_getreadbuffer;
-//    writebufferproc bf_getwritebuffer;
-//    segcountproc bf_getsegcount;
-//    charbufferproc bf_getcharbuffer;
-// }
-
-#if PY_MAJOR_VERSION >= 3
-
-#define JPY_PY27_OLD_BUFFER_PROCS
-
-#else
-
-#define JPY_PY27_OLD_BUFFER_PROCS \
-    (getreadbufferproc) NULL, \
-    (getwritebufferproc) NULL, \
-    (segcountproc) NULL, \
-    (getcharbufferproc) NULL,
-
-#endif
-
-
-PyBufferProcs JArray_as_buffer_boolean = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_boolean,
-    (releasebufferproc) JArray_releasebufferproc_boolean
-};
-
-PyBufferProcs JArray_as_buffer_char = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_char,
-    (releasebufferproc) JArray_releasebufferproc_char
-};
-
-PyBufferProcs JArray_as_buffer_byte = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_byte,
-    (releasebufferproc) JArray_releasebufferproc_byte
-};
-
-PyBufferProcs JArray_as_buffer_short = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_short,
-    (releasebufferproc) JArray_releasebufferproc_short
-};
-
-PyBufferProcs JArray_as_buffer_int = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_int,
-    (releasebufferproc) JArray_releasebufferproc_int
-};
-
-PyBufferProcs JArray_as_buffer_long = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_long,
-    (releasebufferproc) JArray_releasebufferproc_long
-};
-
-PyBufferProcs JArray_as_buffer_float = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_float,
-    (releasebufferproc) JArray_releasebufferproc_float
-};
-
-PyBufferProcs JArray_as_buffer_double = {
-    JPY_PY27_OLD_BUFFER_PROCS
-    (getbufferproc) JArray_getbufferproc_double,
-    (releasebufferproc) JArray_releasebufferproc_double
-};
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#include "jpy_module.h"
+#include "jpy_diag.h"
+#include "jpy_jarray.h"
+
+
+#define PRINT_FLAG(F) printf("JArray_GetBufferProc: %s = %d\n", #F, (flags & F) != 0);
+#define PRINT_MEMB(F, M) printf("JArray_GetBufferProc: %s = " ## F ## "\n", #M, M);
+
+//#define JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL 1
+
+
+/*
+ * Implements the getbuffer() method of the buffer protocol for JPy_JArray objects.
+ * Regarding the format parameter, refer to the Python 'struct' module documentation:
+ * http://docs.python.org/2/library/struct.html#module-struct
+ */
+int JArray_GetBufferProc(JPy_JArray* self, Py_buffer* view, int flags, char javaType, jint itemSize, const char* format)
+{
+    JNIEnv* jenv;
+    jint itemCount;
+    jboolean isCopy;
+    void* buf;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
+
+    /*
+    printf("JArray_GetBufferProc:\n");
+    PRINT_FLAG(PyBUF_ANY_CONTIGUOUS);
+    PRINT_FLAG(PyBUF_CONTIG);
+    PRINT_FLAG(PyBUF_CONTIG_RO);
+    PRINT_FLAG(PyBUF_C_CONTIGUOUS);
+    PRINT_FLAG(PyBUF_FORMAT);
+    PRINT_FLAG(PyBUF_FULL);
+    PRINT_FLAG(PyBUF_FULL_RO);
+    PRINT_FLAG(PyBUF_F_CONTIGUOUS);
+    PRINT_FLAG(PyBUF_INDIRECT);
+    PRINT_FLAG(PyBUF_ND);
+    PRINT_FLAG(PyBUF_READ);
+    PRINT_FLAG(PyBUF_RECORDS);
+    PRINT_FLAG(PyBUF_RECORDS_RO);
+    PRINT_FLAG(PyBUF_SIMPLE);
+    PRINT_FLAG(PyBUF_STRIDED);
+    PRINT_FLAG(PyBUF_STRIDED_RO);
+    PRINT_FLAG(PyBUF_STRIDES);
+    PRINT_FLAG(PyBUF_WRITE);
+    PRINT_FLAG(PyBUF_WRITEABLE);
+    */
+
+    itemCount = (*jenv)->GetArrayLength(jenv, self->objectRef);
+
+    // According to Python documentation,
+    // buffer allocation shall be done in the 5 following steps;
+
+    // Step 1/5
+#ifdef JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL
+    buf = (*jenv)->GetPrimitiveArrayCritical(jenv, self->objectRef, &isCopy);
+#else
+    if (javaType == 'Z') {
+        buf = (*jenv)->GetBooleanArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'C') {
+        buf = (*jenv)->GetCharArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'B') {
+        buf = (*jenv)->GetByteArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'S') {
+        buf = (*jenv)->GetShortArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'I') {
+        buf = (*jenv)->GetIntArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'J') {
+        buf = (*jenv)->GetLongArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'F') {
+        buf = (*jenv)->GetFloatArrayElements(jenv, self->objectRef, &isCopy);
+    } else if (javaType == 'D') {
+        buf = (*jenv)->GetDoubleArrayElements(jenv, self->objectRef, &isCopy);
+    } else {
+        PyErr_Format(PyExc_RuntimeError, "internal error: illegal Java array type '%c'", javaType);
+        return -1;
+    }
+#endif
+    if (buf == NULL) {
+        PyErr_NoMemory();
+        return -1;
+    }
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JArray_GetBufferProc: buf=%p, type='%s', format='%s', itemSize=%d, itemCount=%d, isCopy=%d\n", buf, Py_TYPE(self)->tp_name, format, itemSize, itemCount, isCopy);
+
+    // Step 2/5
+    view->buf = buf;
+    view->len = itemCount * itemSize;
+    view->itemsize = itemSize;
+    view->readonly = (flags & (PyBUF_WRITE | PyBUF_WRITEABLE)) == 0;
+    view->ndim = 1;
+    view->shape = PyMem_New(Py_ssize_t, 1);
+    *view->shape = itemCount;
+    view->strides = PyMem_New(Py_ssize_t, 1);
+    *view->strides = itemSize;
+    view->suboffsets = NULL;
+    if ((flags & PyBUF_FORMAT) != 0) {
+        view->format = (char*) format;
+    } else {
+        view->format = (char*) "B";
+    }
+
+    /*
+    PRINT_MEMB("%d", view->len);
+    PRINT_MEMB("%d", view->ndim);
+    PRINT_MEMB("%s", view->format);
+    PRINT_MEMB("%d", view->itemsize);
+    PRINT_MEMB("%d", view->readonly);
+    PRINT_MEMB("%d", view->shape[0]);
+    PRINT_MEMB("%d", view->strides[0]);
+    */
+
+    // Step 3/5
+    self->bufferExportCount++;
+
+    // Step 4/5
+    view->obj = (PyObject*) self;
+    Py_INCREF(view->obj);
+
+    // Step 5/5
+    return 0;
+}
+
+int JArray_getbufferproc_boolean(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'Z', 1, "B");
+}
+
+int JArray_getbufferproc_char(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'C', 2, "H");
+}
+
+int JArray_getbufferproc_byte(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'B', 1, "b");
+}
+
+int JArray_getbufferproc_short(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'S', 2, "h");
+}
+
+int JArray_getbufferproc_int(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'I', 4, "i");
+}
+
+int JArray_getbufferproc_long(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'J', 8, "q");
+}
+
+int JArray_getbufferproc_float(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'F', 4, "f");
+}
+
+int JArray_getbufferproc_double(JPy_JArray* self, Py_buffer* view, int flags)
+{
+    return JArray_GetBufferProc(self, view, flags, 'D', 8, "d");
+}
+
+
+/*
+ * Implements the releasebuffer() method the buffer protocol for JPy_JArray objects
+ */
+void JArray_ReleaseBufferProc(JPy_JArray* self, Py_buffer* view, char javaType)
+{
+    // Step 1
+    self->bufferExportCount--;
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JArray_ReleaseBufferProc: buf=%p, bufferExportCount=%d\n", view->buf, self->bufferExportCount);
+
+    // Step 2
+    if (self->bufferExportCount == 0 && view->buf != NULL) {
+        JNIEnv* jenv = JPy_GetJNIEnv();
+        if (jenv != NULL) {
+#ifdef JPy_USE_GET_PRIMITIVE_ARRAY_CRITICAL
+           (*jenv)->ReleasePrimitiveArrayCritical(jenv, self->objectRef, view->buf, 0);
+#else
+            if (javaType == 'Z') {
+                (*jenv)->ReleaseBooleanArrayElements(jenv, self->objectRef, (jboolean*) view->buf, 0);
+            } else if (javaType == 'C') {
+                (*jenv)->ReleaseCharArrayElements(jenv, self->objectRef, (jchar*) view->buf, 0);
+            } else if (javaType == 'B') {
+                (*jenv)->ReleaseByteArrayElements(jenv, self->objectRef, (jbyte*) view->buf, 0);
+            } else if (javaType == 'S') {
+                (*jenv)->ReleaseShortArrayElements(jenv, self->objectRef, (jshort*) view->buf, 0);
+            } else if (javaType == 'I') {
+                (*jenv)->ReleaseIntArrayElements(jenv, self->objectRef, (jint*) view->buf, 0);
+            } else if (javaType == 'J') {
+                (*jenv)->ReleaseLongArrayElements(jenv, self->objectRef, (jlong*) view->buf, 0);
+            } else if (javaType == 'F') {
+                (*jenv)->ReleaseFloatArrayElements(jenv, self->objectRef, (jfloat*) view->buf, 0);
+            } else if (javaType == 'D') {
+                (*jenv)->ReleaseDoubleArrayElements(jenv, self->objectRef, (jdouble*) view->buf, 0);
+            }
+#endif
+        }
+        view->buf = NULL;
+    }
+
+    // todo - check if we must Py_DECREF here
+    //Py_DECREF(view->obj);
+}
+
+// todo: py27: fix all releasebufferproc() functions which have different parameter types in 2.7
+
+void JArray_releasebufferproc_boolean(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'Z');
+}
+
+void JArray_releasebufferproc_char(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'C');
+}
+
+void JArray_releasebufferproc_byte(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'B');
+}
+
+void JArray_releasebufferproc_short(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'S');
+}
+
+void JArray_releasebufferproc_int(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'I');
+}
+
+void JArray_releasebufferproc_long(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'J');
+}
+
+void JArray_releasebufferproc_float(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'F');
+}
+
+void JArray_releasebufferproc_double(JPy_JArray* self, Py_buffer* view)
+{
+    JArray_ReleaseBufferProc(self, view, 'D');
+}
+
+// PyBufferProcs 3.x
+//
+// struct PyBufferProcs {
+//    getbufferproc bf_getbuffer;
+//    releasebufferproc bf_releasebuffer;
+// }
+//
+// PyBufferProcs 2.6 and 2.7 (3.x backport)
+//
+// struct PyBufferProcs {
+//    readbufferproc bf_getreadbuffer;
+//    writebufferproc bf_getwritebuffer;
+//    segcountproc bf_getsegcount;
+//    charbufferproc bf_getcharbuffer;
+//    getbufferproc bf_getbuffer;
+//    releasebufferproc bf_releasebuffer;
+// }
+//
+// PyBufferProcs <= 2.5 (not supported by jpy)
+//
+// struct PyBufferProcs {
+//    readbufferproc bf_getreadbuffer;
+//    writebufferproc bf_getwritebuffer;
+//    segcountproc bf_getsegcount;
+//    charbufferproc bf_getcharbuffer;
+// }
+
+#if defined(JPY_COMPAT_33P)
+
+#define JPY_PY27_OLD_BUFFER_PROCS
+
+#elif defined(JPY_COMPAT_27)
+
+#define JPY_PY27_OLD_BUFFER_PROCS \
+    (getreadbufferproc) NULL, \
+    (getwritebufferproc) NULL, \
+    (segcountproc) NULL, \
+    (getcharbufferproc) NULL,
+
+#else
+
+#error JPY_VERSION_ERROR
+
+#endif
+
+
+PyBufferProcs JArray_as_buffer_boolean = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_boolean,
+    (releasebufferproc) JArray_releasebufferproc_boolean
+};
+
+PyBufferProcs JArray_as_buffer_char = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_char,
+    (releasebufferproc) JArray_releasebufferproc_char
+};
+
+PyBufferProcs JArray_as_buffer_byte = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_byte,
+    (releasebufferproc) JArray_releasebufferproc_byte
+};
+
+PyBufferProcs JArray_as_buffer_short = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_short,
+    (releasebufferproc) JArray_releasebufferproc_short
+};
+
+PyBufferProcs JArray_as_buffer_int = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_int,
+    (releasebufferproc) JArray_releasebufferproc_int
+};
+
+PyBufferProcs JArray_as_buffer_long = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_long,
+    (releasebufferproc) JArray_releasebufferproc_long
+};
+
+PyBufferProcs JArray_as_buffer_float = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_float,
+    (releasebufferproc) JArray_releasebufferproc_float
+};
+
+PyBufferProcs JArray_as_buffer_double = {
+    JPY_PY27_OLD_BUFFER_PROCS
+    (getbufferproc) JArray_getbufferproc_double,
+    (releasebufferproc) JArray_releasebufferproc_double
+};
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jarray.h` & `jpy-0.7.5/src/main/c/jpy_jarray.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_JARRAY_H
-#define JPY_JARRAY_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-/**
- * The Java primitive array representation in Python.
- *
- * IMPORTANT: JPy_JArray must only differ from the JPy_JObj structure by the 'bufferExportCount' member
- * since we use the same basic type, name JPy_JType for it. DON'T ever change member positions!
- * @see JPy_JObj
- */
-typedef struct JPy_JArray
-{
-    PyObject_HEAD
-    jobject objectRef;
-    jint bufferExportCount;
-}
-JPy_JArray;
-
-extern PyBufferProcs JArray_as_buffer_boolean;
-extern PyBufferProcs JArray_as_buffer_char;
-extern PyBufferProcs JArray_as_buffer_byte;
-extern PyBufferProcs JArray_as_buffer_short;
-extern PyBufferProcs JArray_as_buffer_int;
-extern PyBufferProcs JArray_as_buffer_long;
-extern PyBufferProcs JArray_as_buffer_float;
-extern PyBufferProcs JArray_as_buffer_double;
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
-#endif /* !JPY_JARRAY_H */
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_JARRAY_H
+#define JPY_JARRAY_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+/**
+ * The Java primitive array representation in Python.
+ *
+ * IMPORTANT: JPy_JArray must only differ from the JPy_JObj structure by the 'bufferExportCount' member
+ * since we use the same basic type, name JPy_JType for it. DON'T ever change member positions!
+ * @see JPy_JObj
+ */
+typedef struct JPy_JArray
+{
+    PyObject_HEAD
+    jobject objectRef;
+    jint bufferExportCount;
+}
+JPy_JArray;
+
+extern PyBufferProcs JArray_as_buffer_boolean;
+extern PyBufferProcs JArray_as_buffer_char;
+extern PyBufferProcs JArray_as_buffer_byte;
+extern PyBufferProcs JArray_as_buffer_short;
+extern PyBufferProcs JArray_as_buffer_int;
+extern PyBufferProcs JArray_as_buffer_long;
+extern PyBufferProcs JArray_as_buffer_float;
+extern PyBufferProcs JArray_as_buffer_double;
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
+#endif /* !JPY_JARRAY_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jfield.c` & `jpy-0.7.5/src/main/c/jpy_jfield.c`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/c/jpy_jfield.h` & `jpy-0.7.5/src/main/c/jpy_jfield.h`

 * *Files 22% similar despite different names*

```diff
@@ -1,56 +1,57 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_JFIELD_H
-#define JPY_JFIELD_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-
-/**
- * Python object representing a Java method. It's type is 'JMethod'.
- */
-typedef struct
-{
-    PyObject_HEAD
-
-    // The declaring class.
-    JPy_JType* declaringClass;
-    // Field name.
-    PyObject* name;
-    // Field type.
-    JPy_JType* type;
-    // Method is static?
-    char isStatic;
-    // Method is final?
-    char isFinal;
-    // Field ID retrieved from JNI.
-    jfieldID fid;
-}
-JPy_JField;
-
-/**
- * The Python 'JMethod' type singleton.
- */
-extern PyTypeObject JField_Type;
-
-JPy_JField* JField_New(JPy_JType* declaringType, PyObject* fieldKey, JPy_JType* fieldType, jboolean isStatic, jboolean isFinal, jfieldID fid);
-void JField_Del(JPy_JField* field);
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
-
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_JFIELD_H
+#define JPY_JFIELD_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+/**
+ * Python object representing a Java method. It's type is 'JMethod'.
+ */
+typedef struct
+{
+    PyObject_HEAD
+
+    // The declaring class.
+    JPy_JType* declaringClass;
+    // Field name.
+    PyObject* name;
+    // Field type.
+    JPy_JType* type;
+    // Method is static?
+    char isStatic;
+    // Method is final?
+    char isFinal;
+    // Field ID retrieved from JNI.
+    jfieldID fid;
+}
+JPy_JField;
+
+/**
+ * The Python 'JMethod' type singleton.
+ */
+extern PyTypeObject JField_Type;
+
+JPy_JField* JField_New(JPy_JType* declaringType, PyObject* fieldKey, JPy_JType* fieldType, jboolean isStatic, jboolean isFinal, jfieldID fid);
+void JField_Del(JPy_JField* field);
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
+
 #endif /* !JPY_JFIELD_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jmethod.c` & `jpy-0.7.5/src/main/c/jpy_jmethod.c`

 * *Files 20% similar despite different names*

```diff
@@ -1,843 +1,849 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#include "jpy_module.h"
-#include "jpy_diag.h"
-#include "jpy_jtype.h"
-#include "jpy_jobj.h"
-#include "jpy_jmethod.h"
-#include "jpy_conv.h"
-#include "jpy_compat.h"
-
-
-JPy_JMethod* JMethod_New(PyObject* name,
-                         int paramCount,
-                         JPy_ParamDescriptor* paramDescriptors,
-                         JPy_ReturnDescriptor* returnDescriptor,
-                         jboolean isStatic,
-                         jmethodID mid)
-{
-    PyTypeObject* type = &JMethod_Type;
-    JPy_JMethod* method;
-
-    method = (JPy_JMethod*) type->tp_alloc(type, 0);
-    method->name = name;
-    method->paramCount = paramCount;
-    method->paramDescriptors = paramDescriptors;
-    method->returnDescriptor = returnDescriptor;
-    method->isStatic = isStatic;
-    method->mid = mid;
-
-    Py_INCREF(method->name);
-
-    return method;
-}
-
-
-/**
- * The JMethod type's tp_dealloc slot. 
- */
-void JMethod_dealloc(JPy_JMethod* self)
-{
-    JNIEnv* jenv;
-
-    Py_DECREF(self->name);
-
-    jenv = JPy_GetJNIEnv();
-    if (jenv != NULL) {
-        int i;
-        for (i = 0; i < self->paramCount; i++) {
-            Py_DECREF((self->paramDescriptors + i)->type);
-        }
-        Py_DECREF((self->returnDescriptor + i)->type);
-    }
-
-    PyMem_Del(self->paramDescriptors);
-    PyMem_Del(self->returnDescriptor);
-    
-    Py_TYPE(self)->tp_free((PyObject*) self);
-}
-
-void JMethod_Del(JPy_JMethod* method)
-{
-    JMethod_dealloc(method);
-}
-
-/**
- * Matches the give Python argument tuple against the Java method's formal parameters.
- * Returns the sum of the i-th argument against the i-th Java parameter.
- * The maximum match value returned is 100 * method->paramCount.
- */
-int JMethod_MatchPyArgs(JNIEnv* jenv, JPy_JMethod* method, int argCount, PyObject* pyArgs)
-{
-    JPy_ParamDescriptor* paramDescriptor;
-    PyObject* pyArg;
-    int matchValueSum;
-    int matchValue;
-    int i;
-    int i0;
-
-    if (method->isStatic) {
-        //printf("Static! method->paramCount=%d, argCount=%d\n", method->paramCount, argCount);
-        if (method->paramCount != argCount) {
-            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: argument count mismatch (matchValue=0)\n");
-            // argument count mismatch
-            return 0;
-        }
-        i0 = 0;
-    } else {
-        PyObject* self;
-        //printf("Non-Static! method->paramCount=%d, argCount=%d\n", method->paramCount, argCount);
-        if (method->paramCount != argCount - 1) {
-            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: argument count mismatch (matchValue=0)\n");
-            // argument count mismatch
-            return 0;
-        }
-        self = PyTuple_GetItem(pyArgs, 0);
-        if (!JObj_Check(self)) {
-            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: self argument is not a Java object (matchValue=0)\n");
-            return 0;
-        }
-        i0 = 1;
-    }
-
-    if (method->paramCount == 0) {
-        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: no-argument method (matchValue=100)\n");
-        // There can't be any other method overloads with no parameters
-        return 100;
-    }
-
-    paramDescriptor = method->paramDescriptors;
-    matchValueSum = 0;
-    for (i = i0; i < argCount; i++) {
-
-        pyArg = PyTuple_GetItem(pyArgs, i);
-        matchValue = paramDescriptor->MatchPyArg(jenv, paramDescriptor, pyArg);
-
-        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: pyArgs[%d]: matchValue=%d\n", i, matchValue);
-
-        if (matchValue == 0) {
-            //printf("JMethod_MatchPyArgs 6\n");
-            // current pyArg does not match parameter type at all
-            return 0;
-        }
-
-        matchValueSum += matchValue;
-        paramDescriptor++;
-    }
-
-    //printf("JMethod_MatchPyArgs 7\n");
-    return matchValueSum;
-}
-
-#define JPy_SUPPORT_RETURN_PARAMETER 1
-
-PyObject* JMethod_FromJObject(JNIEnv* jenv, JPy_JMethod* method, PyObject* pyArgs, jvalue* jArgs, int argOffset, JPy_JType* returnType, jobject jReturnValue)
-{
-    #ifdef JPy_SUPPORT_RETURN_PARAMETER
-    if (method->returnDescriptor->paramIndex >= 0) {
-        jint paramIndex = method->returnDescriptor->paramIndex;
-        PyObject* pyReturnArg = PyTuple_GetItem(pyArgs, paramIndex + argOffset);
-        jobject jArg = jArgs[paramIndex].l;
-        //printf("JMethod_FromJObject: paramIndex=%d, jArg=%p, isNone=%d\n", paramIndex, jArg, pyReturnArg == Py_None);
-        if ((JObj_Check(pyReturnArg) || PyObject_CheckBuffer(pyReturnArg))
-            && (*jenv)->IsSameObject(jenv, jReturnValue, jArg)) {
-             Py_INCREF(pyReturnArg);
-             return pyReturnArg;
-        }
-    }
-    #endif
-    return JPy_FromJObjectWithType(jenv, jReturnValue, returnType);
-}
-
-/**
- * Invoke a method. We have already ensured that the Python arguments and expected Java parameters match.
- */
-PyObject* JMethod_InvokeMethod(JNIEnv* jenv, JPy_JMethod* method, JPy_JType* type, PyObject* pyArgs)
-{
-    jvalue* jArgs;
-    JPy_ArgDisposer* argDisposers;
-    PyObject* returnValue;
-    JPy_JType* returnType;
-
-    //printf("JMethod_InvokeMethod 1: typeCode=%c\n", typeCode);
-    if (JMethod_CreateJArgs(jenv, method, pyArgs, &jArgs, &argDisposers) < 0) {
-        return NULL;
-    }
-
-    //printf("JMethod_InvokeMethod 2: typeCode=%c\n", typeCode);
-
-    returnType = method->returnDescriptor->type;
-    returnValue = NULL;
-
-    if (method->isStatic) {
-        jclass classRef = type->classRef;
-
-        JPy_DIAG_PRINT(JPy_DIAG_F_EXEC, "JMethod_InvokeMethod: calling static Java method %s#%s\n", type->javaName, JPy_AS_UTF8(method->name));
-
-        if (returnType == JPy_JVoid) {
-            (*jenv)->CallStaticVoidMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JVOID();
-        } else if (returnType == JPy_JBoolean) {
-            jboolean v = (*jenv)->CallStaticBooleanMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JBOOLEAN(v);
-        } else if (returnType == JPy_JChar) {
-            jchar v = (*jenv)->CallStaticCharMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JCHAR(v);
-        } else if (returnType == JPy_JByte) {
-            jbyte v = (*jenv)->CallStaticByteMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JBYTE(v);
-        } else if (returnType == JPy_JShort) {
-            jshort v = (*jenv)->CallStaticShortMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JSHORT(v);
-        } else if (returnType == JPy_JInt) {
-            jint v = (*jenv)->CallStaticIntMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JINT(v);
-        } else if (returnType == JPy_JLong) {
-            jlong v = (*jenv)->CallStaticIntMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JLONG(v);
-        } else if (returnType == JPy_JFloat) {
-            jfloat v = (*jenv)->CallStaticFloatMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JFLOAT(v);
-        } else if (returnType == JPy_JDouble) {
-            jdouble v = (*jenv)->CallStaticDoubleMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JDOUBLE(v);
-        } else if (returnType == JPy_JString) {
-            jstring v = (*jenv)->CallStaticObjectMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FromJString(jenv, v);
-            (*jenv)->DeleteLocalRef(jenv, v);
-        } else {
-            jobject v = (*jenv)->CallStaticObjectMethodA(jenv, classRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JMethod_FromJObject(jenv, method, pyArgs, jArgs, 0, returnType, v);
-            (*jenv)->DeleteLocalRef(jenv, v);
-        }
-
-    } else {
-        jobject objectRef;
-        PyObject* self;
-
-        JPy_DIAG_PRINT(JPy_DIAG_F_EXEC, "JMethod_InvokeMethod: calling Java method %s#%s\n", type->javaName, JPy_AS_UTF8(method->name));
-
-        self = PyTuple_GetItem(pyArgs, 0);
-        // Note it is already ensured that self is a JPy_JObj*
-        objectRef = ((JPy_JObj*) self)->objectRef;
-
-        if (returnType == JPy_JVoid) {
-            (*jenv)->CallVoidMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JVOID();
-        } else if (returnType == JPy_JBoolean) {
-            jboolean v = (*jenv)->CallBooleanMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JBOOLEAN(v);
-        } else if (returnType == JPy_JChar) {
-            jchar v = (*jenv)->CallCharMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JCHAR(v);
-        } else if (returnType == JPy_JByte) {
-            jbyte v = (*jenv)->CallByteMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JBYTE(v);
-        } else if (returnType == JPy_JShort) {
-            jshort v = (*jenv)->CallShortMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JSHORT(v);
-        } else if (returnType == JPy_JInt) {
-            jint v = (*jenv)->CallIntMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JINT(v);
-        } else if (returnType == JPy_JLong) {
-            jlong v = (*jenv)->CallIntMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JLONG(v);
-        } else if (returnType == JPy_JFloat) {
-            jfloat v = (*jenv)->CallFloatMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JFLOAT(v);
-        } else if (returnType == JPy_JDouble) {
-            jdouble v = (*jenv)->CallDoubleMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FROM_JDOUBLE(v);
-        } else if (returnType == JPy_JString) {
-            jstring v = (*jenv)->CallObjectMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JPy_FromJString(jenv, v);
-            (*jenv)->DeleteLocalRef(jenv, v);
-        } else {
-            jobject v = (*jenv)->CallObjectMethodA(jenv, objectRef, method->mid, jArgs);
-            JPy_ON_JAVA_EXCEPTION_GOTO(error);
-            returnValue = JMethod_FromJObject(jenv, method, pyArgs, jArgs, 1, returnType, v);
-            (*jenv)->DeleteLocalRef(jenv, v);
-        }
-    }
-
-error:
-    if (jArgs != NULL) {
-        JMethod_DisposeJArgs(jenv, method->paramCount, jArgs, argDisposers);
-    }
-
-    return returnValue;
-}
-
-int JMethod_CreateJArgs(JNIEnv* jenv, JPy_JMethod* method, PyObject* pyArgs, jvalue** argValuesRet, JPy_ArgDisposer** argDisposersRet)
-{
-    JPy_ParamDescriptor* paramDescriptor;
-    int i, i0, argCount;
-    PyObject* pyArg;
-    jvalue* jValue;
-    jvalue* jValues;
-    JPy_ArgDisposer* argDisposer;
-    JPy_ArgDisposer* argDisposers;
-
-    if (method->paramCount == 0) {
-        *argValuesRet = NULL;
-        *argDisposersRet = NULL;
-        return 0;
-    }
-
-    argCount = PyTuple_Size(pyArgs);
-
-    i0 = argCount - method->paramCount;
-    if (!(i0 == 0 || i0 == 1)) {
-        PyErr_SetString(PyExc_RuntimeError, "internal error");
-        return -1;
-    }
-
-    jValues = PyMem_New(jvalue, method->paramCount);
-    if (jValues == NULL) {
-        PyErr_NoMemory();
-        return -1;
-    }
-
-    argDisposers = PyMem_New(JPy_ArgDisposer, method->paramCount);
-    if (argDisposers == NULL) {
-        PyMem_Del(jValues);
-        PyErr_NoMemory();
-        return -1;
-    }
-
-    paramDescriptor = method->paramDescriptors;
-    jValue = jValues;
-    argDisposer = argDisposers;
-    for (i = i0; i < argCount; i++) {
-        pyArg = PyTuple_GetItem(pyArgs, i);
-        jValue->l = 0;
-        argDisposer->data = NULL;
-        argDisposer->DisposeArg = NULL;
-        if (paramDescriptor->ConvertPyArg(jenv, paramDescriptor, pyArg, jValue, argDisposer) < 0) {
-            PyMem_Del(jValues);
-            PyMem_Del(argDisposers);
-            return -1;
-        }
-        paramDescriptor++;
-        jValue++;
-        argDisposer++;
-    }
-
-    *argValuesRet = jValues;
-    *argDisposersRet = argDisposers;
-    return 0;
-}
-
-void JMethod_DisposeJArgs(JNIEnv* jenv, int paramCount, jvalue* jArgs, JPy_ArgDisposer* argDisposers)
-{
-    jvalue* jArg;
-    JPy_ArgDisposer* argDisposer;
-    int index;
-
-    jArg = jArgs;
-    argDisposer = argDisposers;
-
-    for (index = 0; index < paramCount; index++) {
-        if (argDisposer->DisposeArg != NULL) {
-            argDisposer->DisposeArg(jenv, jArg, argDisposer->data);
-        }
-        jArg++;
-        argDisposer++;
-    }
-
-    PyMem_Del(jArgs);
-    PyMem_Del(argDisposers);
-}
-
-
-PyObject* JMethod_repr(JPy_JMethod* self)
-{
-    const char* name = JPy_AS_UTF8(self->name);
-    return JPy_FROM_FORMAT("%s(name='%s', param_count=%d, is_static=%d, mid=%p)",
-                           ((PyObject*)self)->ob_type->tp_name,
-                           name,
-                           self->paramCount,
-                           self->isStatic,
-                           self->mid);
-}
-
-PyObject* JMethod_str(JPy_JMethod* self)
-{
-    Py_INCREF(self->name);
-    return self->name;
-}
-
-
-static PyMemberDef JMethod_members[] =
-{
-    {"name",        T_OBJECT_EX, offsetof(JPy_JMethod, name),       READONLY, "Method name"},
-    {"param_count", T_INT,       offsetof(JPy_JMethod, paramCount), READONLY, "Number of method parameters"},
-    {"is_static",   T_BOOL,      offsetof(JPy_JMethod, isStatic),   READONLY, "Tests if this is a static method"},
-    {NULL}  /* Sentinel */
-};
-
-#define JMethod_CHECK_PARAMETER_INDEX(self, index) \
-    if (index < 0 || index >= self->paramCount) { \
-        PyErr_SetString(PyExc_IndexError, "invalid parameter index"); \
-        return NULL; \
-    }
-
-
-PyObject* JMethod_get_param_type(JPy_JMethod* self, PyObject* args)
-{
-    PyObject* type;
-    int index;
-    if (!PyArg_ParseTuple(args, "i:get_param_type", &index)) {
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    type = (PyObject*) self->paramDescriptors[index].type;
-    Py_INCREF(type);
-    return type;
-}
-
-PyObject* JMethod_is_param_mutable(JPy_JMethod* self, PyObject* args)
-{
-    int index;
-    int value;
-    if (!PyArg_ParseTuple(args, "i:is_param_mutable", &index)) {
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    value = self->paramDescriptors[index].isMutable;
-    return PyBool_FromLong(value);
-}
-
-PyObject* JMethod_set_param_mutable(JPy_JMethod* self, PyObject* args)
-{
-    int index;
-    int value;
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
-    if (!PyArg_ParseTuple(args, "ip:set_param_mutable", &index, &value)) {
-#else
-    if (!PyArg_ParseTuple(args, "ii:set_param_mutable", &index, &value)) {
-#endif
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    self->paramDescriptors[index].isMutable = value;
-    return Py_BuildValue("");
-}
-
-PyObject* JMethod_is_param_output(JPy_JMethod* self, PyObject* args)
-{
-    int index = 0;
-    int value = 0;
-    if (!PyArg_ParseTuple(args, "i:is_param_output", &index)) {
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    value = self->paramDescriptors[index].isOutput;
-    return PyBool_FromLong(value);
-}
-
-PyObject* JMethod_set_param_output(JPy_JMethod* self, PyObject* args)
-{
-    int index = 0;
-    int value = 0;
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
-    if (!PyArg_ParseTuple(args, "ip:set_param_output", &index, &value)) {
-#else
-    if (!PyArg_ParseTuple(args, "ii:set_param_output", &index, &value)) {
-#endif
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    self->paramDescriptors[index].isOutput = value;
-    return Py_BuildValue("");
-}
-
-PyObject* JMethod_is_param_return(JPy_JMethod* self, PyObject* args)
-{
-    int index = 0;
-    int value = 0;
-    if (!PyArg_ParseTuple(args, "i:is_param_return", &index)) {
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    value = self->paramDescriptors[index].isReturn;
-    return PyBool_FromLong(value);
-}
-
-PyObject* JMethod_set_param_return(JPy_JMethod* self, PyObject* args)
-{
-    int index = 0;
-    int value = 0;
-#if PY_MAJOR_VERSION >= 3 && PY_MINOR_VERSION >= 3
-    if (!PyArg_ParseTuple(args, "ip:set_param_return", &index, &value)) {
-#else
-    if (!PyArg_ParseTuple(args, "ii:set_param_return", &index, &value)) {
-#endif
-        return NULL;
-    }
-    JMethod_CHECK_PARAMETER_INDEX(self, index);
-    self->paramDescriptors[index].isReturn = value;
-    if (value) {
-        self->returnDescriptor->paramIndex = index;
-    }
-    return Py_BuildValue("");
-}
-
-
-static PyMethodDef JMethod_methods[] =
-{
-    {"get_param_type",    (PyCFunction) JMethod_get_param_type,    METH_VARARGS, "Gets the type of the parameter given by index"},
-    {"is_param_mutable",  (PyCFunction) JMethod_is_param_mutable,  METH_VARARGS, "Tests if the method parameter given by index is mutable"},
-    {"is_param_output",   (PyCFunction) JMethod_is_param_output,   METH_VARARGS, "Tests if the method parameter given by index is a mere output value (and not read from)"},
-    {"is_param_return",   (PyCFunction) JMethod_is_param_return,   METH_VARARGS, "Tests if the method parameter given by index is the return value"},
-    {"set_param_mutable", (PyCFunction) JMethod_set_param_mutable, METH_VARARGS, "Sets whether the method parameter given by index is mutable"},
-    {"set_param_output",  (PyCFunction) JMethod_set_param_output,  METH_VARARGS, "Sets whether the method parameter given by index is a mere output value (and not read from)"},
-    {"set_param_return",  (PyCFunction) JMethod_set_param_return,  METH_VARARGS, "Sets whether the method parameter given by index is the return value"},
-    {NULL}  /* Sentinel */
-};
-
-/**
- * Implements the BeamPy_JObjectType class singleton.
- */
-PyTypeObject JMethod_Type = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "jpy.JMethod",                /* tp_name */
-    sizeof (JPy_JMethod),         /* tp_basicsize */
-    0,                            /* tp_itemsize */
-    (destructor)JMethod_dealloc,  /* tp_dealloc */
-    NULL,                         /* tp_print */
-    NULL,                         /* tp_getattr */
-    NULL,                         /* tp_setattr */
-    NULL,                         /* tp_reserved */
-    (reprfunc)JMethod_repr,       /* tp_repr */
-    NULL,                         /* tp_as_number */
-    NULL,                         /* tp_as_sequence */
-    NULL,                         /* tp_as_mapping */
-    NULL,                         /* tp_hash  */
-    NULL,                         /* tp_call */
-    (reprfunc)JMethod_str,        /* tp_str */
-    NULL,                         /* tp_getattro */
-    NULL,                         /* tp_setattro */
-    NULL,                         /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT,           /* tp_flags */
-    "Java Method Wrapper",        /* tp_doc */
-    NULL,                         /* tp_traverse */
-    NULL,                         /* tp_clear */
-    NULL,                         /* tp_richcompare */
-    0,                            /* tp_weaklistoffset */
-    NULL,                         /* tp_iter */
-    NULL,                         /* tp_iternext */
-    JMethod_methods,              /* tp_methods */
-    JMethod_members,              /* tp_members */
-    NULL,                         /* tp_getset */
-    NULL,                         /* tp_base */
-    NULL,                         /* tp_dict */
-    NULL,                         /* tp_descr_get */
-    NULL,                         /* tp_descr_set */
-    0,                            /* tp_dictoffset */
-    NULL,                         /* tp_init */
-    NULL,                         /* tp_alloc */
-    NULL,                         /* tp_new */
-};
-
-//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-//  JOverloadedMethod
-
-typedef struct JPy_MethodFindResult
-{
-    JPy_JMethod* method;
-    int matchValue;
-    int matchCount;
-}
-JPy_MethodFindResult;
-
-JPy_JMethod* JOverloadedMethod_FindMethod0(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* pyArgs, JPy_MethodFindResult* result)
-{
-    int overloadCount;
-    int argCount;
-    int matchCount;
-    int matchValue;
-    int matchValueMax;
-    JPy_JMethod* currMethod;
-    JPy_JMethod* bestMethod;
-    int i;
-
-    result->method = NULL;
-    result->matchValue = 0;
-    result->matchCount = 0;
-
-    overloadCount = PyList_Size(overloadedMethod->methodList);
-    if (overloadCount <= 0) {
-        PyErr_SetString(PyExc_RuntimeError, "internal error: invalid overloadedMethod->methodList");
-        return NULL;
-    }
-
-    argCount = PyTuple_Size(pyArgs);
-    matchCount = 0;
-    matchValueMax = -1;
-    bestMethod = NULL;
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JOverloadedMethod_FindMethod0: method '%s#%s': overloadCount=%d\n",
-                              overloadedMethod->declaringClass->javaName, JPy_AS_UTF8(overloadedMethod->name), overloadCount);
-
-    for (i = 0; i < overloadCount; i++) {
-        currMethod = (JPy_JMethod*) PyList_GetItem(overloadedMethod->methodList, i);
-        matchValue = JMethod_MatchPyArgs(jenv, currMethod, argCount, pyArgs);
-
-        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JOverloadedMethod_FindMethod0: methodList[%d]: paramCount=%d, matchValue=%d\n", i,
-                                  currMethod->paramCount, matchValue);
-
-        if (matchValue > 0) {
-            if (matchValue > matchValueMax) {
-                matchValueMax = matchValue;
-                bestMethod = currMethod;
-                matchCount = 1;
-            } else if (matchValue == matchValueMax) {
-                matchCount++;
-            }
-            if (matchValue >= 100 * currMethod->paramCount) {
-                // we can't get any better (if so, we have an internal problem)
-                break;
-            }
-        }
-    }
-
-    if (bestMethod == NULL) {
-        matchValueMax = 0;
-        matchCount = 0;
-    }
-
-    result->method = bestMethod;
-    result->matchValue = matchValueMax;
-    result->matchCount = matchCount;
-
-    return bestMethod;
-}
-
-JPy_JMethod* JOverloadedMethod_FindMethod(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* pyArgs, jboolean visitSuperClass)
-{
-    JPy_JOverloadedMethod* currentOM;
-    JPy_MethodFindResult result;
-    JPy_MethodFindResult bestResult;
-    JPy_JType* superClass;
-    PyObject* superOM;
-
-    if ((JPy_DiagFlags & JPy_DIAG_F_METH) != 0) {
-        int i, argCount = PyTuple_Size(pyArgs);
-        printf("JOverloadedMethod_FindMethod: argCount=%d, visitSuperClass=%d\n", argCount, visitSuperClass);
-        for (i = 0; i < argCount; i++) {
-            PyObject* pyArg = PyTuple_GetItem(pyArgs, i);
-            printf("\tPy_TYPE(pyArgs[%d])->tp_name = %s\n", i, Py_TYPE(pyArg)->tp_name);
-        }
-    }
-
-    bestResult.method = NULL;
-    bestResult.matchValue = 0;
-    bestResult.matchCount = 0;
-
-    currentOM = overloadedMethod;
-    while (1) {
-        if (JOverloadedMethod_FindMethod0(jenv, currentOM, pyArgs, &result) < 0) {
-            // oops, error
-            return NULL;
-        }
-        if (result.method != NULL) {
-            if (result.matchValue >= 100 * result.method->paramCount) {
-                // We can't get any better.
-                return result.method;
-            } else if (result.matchValue > 0 && result.matchValue > bestResult.matchValue) {
-                // We may have better matching methods overloads in the super class (if any)
-                bestResult = result;
-            }
-        }
-
-        if (visitSuperClass) {
-            superClass = currentOM->declaringClass->superType;
-            if (superClass != NULL) {
-                superOM = JType_GetOverloadedMethod(jenv, superClass, currentOM->name, JNI_TRUE);
-            } else {
-                superOM = Py_None;
-            }
-        } else {
-            superOM = Py_None;
-        }
-
-        if (superOM == NULL) {
-            // oops, error
-            return NULL;
-        } else if (superOM == Py_None) {
-            // no overloaded methods found in super class, so return best result found so far
-            if (bestResult.method == NULL) {
-                PyErr_SetString(PyExc_RuntimeError, "no matching Java method overloads found");
-                return NULL;
-            } else if (bestResult.matchCount > 1) {
-                PyErr_SetString(PyExc_RuntimeError, "ambiguous Java method call, too many matching method overloads found");
-                return NULL;
-            } else {
-                return bestResult.method;
-            }
-        } else {
-            // Continue trying with overloads from super type
-            currentOM = (JPy_JOverloadedMethod*) superOM;
-        }
-    }
-
-    // Should never come here
-    PyErr_SetString(PyExc_RuntimeError, "internal error");
-    return NULL;
-}
-
-JPy_JOverloadedMethod* JOverloadedMethod_New(JPy_JType* declaringClass, PyObject* name, JPy_JMethod* method)
-{
-    PyTypeObject* methodType = &JOverloadedMethod_Type;
-    JPy_JOverloadedMethod* overloadedMethod;
-
-    overloadedMethod = (JPy_JOverloadedMethod*) methodType->tp_alloc(methodType, 0);
-    overloadedMethod->declaringClass = declaringClass;
-    overloadedMethod->name = name;
-    overloadedMethod->methodList = PyList_New(0);
-
-    Py_INCREF((PyObject*) overloadedMethod->declaringClass);
-    Py_INCREF((PyObject*) overloadedMethod->name);
-    Py_INCREF((PyObject*) overloadedMethod);
-
-    JOverloadedMethod_AddMethod(overloadedMethod, method);
-
-    return overloadedMethod;
-}
-
-int JOverloadedMethod_AddMethod(JPy_JOverloadedMethod* overloadedMethod, JPy_JMethod* method)
-{
-    return PyList_Append(overloadedMethod->methodList, (PyObject*) method);
-}
-
-/**
- * The 'JOverloadedMethod' type's tp_dealloc slot.
- */
-void JOverloadedMethod_dealloc(JPy_JOverloadedMethod* self)
-{
-    Py_DECREF((PyObject*) self->declaringClass);
-    Py_DECREF((PyObject*) self->name);
-    Py_DECREF((PyObject*) self->methodList);
-    Py_TYPE(self)->tp_free((PyObject*) self);
-}
-
-/**
- * The 'JOverloadedMethod' type's tp_call slot. Makes instances of the 'JOverloadedMethod' type callable.
- */
-PyObject* JOverloadedMethod_call(JPy_JOverloadedMethod* self, PyObject *args, PyObject *kw)
-{
-    JNIEnv* jenv;
-    JPy_JMethod* method;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
-
-    method = JOverloadedMethod_FindMethod(jenv, self, args, JNI_TRUE);
-    if (method == NULL) {
-        return NULL;
-    }
-
-    return JMethod_InvokeMethod(jenv, method, self->declaringClass, args);
-}
-
-/**
- * The 'JOverloadedMethod' type's tp_repr slot.
- */
-PyObject* JOverloadedMethod_repr(JPy_JOverloadedMethod* self)
-{
-    const char* name = JPy_AS_UTF8(self->name);
-    int methodCount = PyList_Size(self->methodList);
-    return JPy_FROM_FORMAT("%s(name='%s', methodCount=%d)",
-                           ((PyObject*)self)->ob_type->tp_name,
-                           name,
-                           methodCount);
-}
-
-static PyMemberDef JOverloadedMethod_members[] =
-{
-    {"name",    T_OBJECT_EX, offsetof(JPy_JOverloadedMethod, name),       READONLY, "Overloaded method name"},
-    {"methods", T_OBJECT_EX, offsetof(JPy_JOverloadedMethod, methodList), READONLY, "List of methods"},
-    {NULL}  /* Sentinel */
-};
-
-/**
- * The 'JOverloadedMethod' type's tp_str slot.
- */
-PyObject* JOverloadedMethod_str(JPy_JOverloadedMethod* self)
-{
-    Py_INCREF(self->name);
-    return self->name;
-}
-
-PyTypeObject JOverloadedMethod_Type = {
-    PyVarObject_HEAD_INIT(NULL, 0)
-    "jpy.JOverloadedMethod",                /* tp_name */
-    sizeof (JPy_JOverloadedMethod),         /* tp_basicsize */
-    0,                            /* tp_itemsize */
-    (destructor)JOverloadedMethod_dealloc,  /* tp_dealloc */
-    NULL,                         /* tp_print */
-    NULL,                         /* tp_getattr */
-    NULL,                         /* tp_setattr */
-    NULL,                         /* tp_reserved */
-    (reprfunc)JOverloadedMethod_repr,       /* tp_repr */
-    NULL,                         /* tp_as_number */
-    NULL,                         /* tp_as_sequence */
-    NULL,                         /* tp_as_mapping */
-    NULL,                         /* tp_hash  */
-    (ternaryfunc)JOverloadedMethod_call,    /* tp_call */
-    (reprfunc)JOverloadedMethod_str,        /* tp_str */
-    NULL,                         /* tp_getattro */
-    NULL,                         /* tp_setattro */
-    NULL,                         /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT,           /* tp_flags */
-    "Java Overloaded Method",     /* tp_doc */
-    NULL,                         /* tp_traverse */
-    NULL,                         /* tp_clear */
-    NULL,                         /* tp_richcompare */
-    0,                            /* tp_weaklistoffset */
-    NULL,                         /* tp_iter */
-    NULL,                         /* tp_iternext */
-    NULL,                         /* tp_methods */
-    JOverloadedMethod_members,    /* tp_members */
-    NULL,                         /* tp_getset */
-    NULL,                         /* tp_base */
-    NULL,                         /* tp_dict */
-    NULL,                         /* tp_descr_get */
-    NULL,                         /* tp_descr_set */
-    0,                            /* tp_dictoffset */
-    NULL,                         /* tp_init */
-    NULL,                         /* tp_alloc */
-    NULL,                         /* tp_new */
-};
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#include "jpy_module.h"
+#include "jpy_diag.h"
+#include "jpy_jtype.h"
+#include "jpy_jobj.h"
+#include "jpy_jmethod.h"
+#include "jpy_conv.h"
+#include "jpy_compat.h"
+
+
+JPy_JMethod* JMethod_New(PyObject* name,
+                         int paramCount,
+                         JPy_ParamDescriptor* paramDescriptors,
+                         JPy_ReturnDescriptor* returnDescriptor,
+                         jboolean isStatic,
+                         jmethodID mid)
+{
+    PyTypeObject* type = &JMethod_Type;
+    JPy_JMethod* method;
+
+    method = (JPy_JMethod*) type->tp_alloc(type, 0);
+    method->name = name;
+    method->paramCount = paramCount;
+    method->paramDescriptors = paramDescriptors;
+    method->returnDescriptor = returnDescriptor;
+    method->isStatic = isStatic;
+    method->mid = mid;
+
+    Py_INCREF(method->name);
+
+    return method;
+}
+
+
+/**
+ * The JMethod type's tp_dealloc slot. 
+ */
+void JMethod_dealloc(JPy_JMethod* self)
+{
+    JNIEnv* jenv;
+
+    Py_DECREF(self->name);
+
+    jenv = JPy_GetJNIEnv();
+    if (jenv != NULL) {
+        int i;
+        for (i = 0; i < self->paramCount; i++) {
+            Py_DECREF((self->paramDescriptors + i)->type);
+        }
+        Py_DECREF((self->returnDescriptor + i)->type);
+    }
+
+    PyMem_Del(self->paramDescriptors);
+    PyMem_Del(self->returnDescriptor);
+    
+    Py_TYPE(self)->tp_free((PyObject*) self);
+}
+
+void JMethod_Del(JPy_JMethod* method)
+{
+    JMethod_dealloc(method);
+}
+
+/**
+ * Matches the give Python argument tuple against the Java method's formal parameters.
+ * Returns the sum of the i-th argument against the i-th Java parameter.
+ * The maximum match value returned is 100 * method->paramCount.
+ */
+int JMethod_MatchPyArgs(JNIEnv* jenv, JPy_JMethod* method, int argCount, PyObject* pyArgs)
+{
+    JPy_ParamDescriptor* paramDescriptor;
+    PyObject* pyArg;
+    int matchValueSum;
+    int matchValue;
+    int i;
+    int i0;
+
+    if (method->isStatic) {
+        //printf("Static! method->paramCount=%d, argCount=%d\n", method->paramCount, argCount);
+        if (method->paramCount != argCount) {
+            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: argument count mismatch (matchValue=0)\n");
+            // argument count mismatch
+            return 0;
+        }
+        i0 = 0;
+    } else {
+        PyObject* self;
+        //printf("Non-Static! method->paramCount=%d, argCount=%d\n", method->paramCount, argCount);
+        if (method->paramCount != argCount - 1) {
+            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: argument count mismatch (matchValue=0)\n");
+            // argument count mismatch
+            return 0;
+        }
+        self = PyTuple_GetItem(pyArgs, 0);
+        if (!JObj_Check(self)) {
+            JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: self argument is not a Java object (matchValue=0)\n");
+            return 0;
+        }
+        i0 = 1;
+    }
+
+    if (method->paramCount == 0) {
+        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: no-argument method (matchValue=100)\n");
+        // There can't be any other method overloads with no parameters
+        return 100;
+    }
+
+    paramDescriptor = method->paramDescriptors;
+    matchValueSum = 0;
+    for (i = i0; i < argCount; i++) {
+
+        pyArg = PyTuple_GetItem(pyArgs, i);
+        matchValue = paramDescriptor->MatchPyArg(jenv, paramDescriptor, pyArg);
+
+        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JMethod_MatchPyArgs: pyArgs[%d]: matchValue=%d\n", i, matchValue);
+
+        if (matchValue == 0) {
+            //printf("JMethod_MatchPyArgs 6\n");
+            // current pyArg does not match parameter type at all
+            return 0;
+        }
+
+        matchValueSum += matchValue;
+        paramDescriptor++;
+    }
+
+    //printf("JMethod_MatchPyArgs 7\n");
+    return matchValueSum;
+}
+
+#define JPy_SUPPORT_RETURN_PARAMETER 1
+
+PyObject* JMethod_FromJObject(JNIEnv* jenv, JPy_JMethod* method, PyObject* pyArgs, jvalue* jArgs, int argOffset, JPy_JType* returnType, jobject jReturnValue)
+{
+    #ifdef JPy_SUPPORT_RETURN_PARAMETER
+    if (method->returnDescriptor->paramIndex >= 0) {
+        jint paramIndex = method->returnDescriptor->paramIndex;
+        PyObject* pyReturnArg = PyTuple_GetItem(pyArgs, paramIndex + argOffset);
+        jobject jArg = jArgs[paramIndex].l;
+        //printf("JMethod_FromJObject: paramIndex=%d, jArg=%p, isNone=%d\n", paramIndex, jArg, pyReturnArg == Py_None);
+        if ((JObj_Check(pyReturnArg) || PyObject_CheckBuffer(pyReturnArg))
+            && (*jenv)->IsSameObject(jenv, jReturnValue, jArg)) {
+             Py_INCREF(pyReturnArg);
+             return pyReturnArg;
+        }
+    }
+    #endif
+    return JPy_FromJObjectWithType(jenv, jReturnValue, returnType);
+}
+
+/**
+ * Invoke a method. We have already ensured that the Python arguments and expected Java parameters match.
+ */
+PyObject* JMethod_InvokeMethod(JNIEnv* jenv, JPy_JMethod* method, JPy_JType* type, PyObject* pyArgs)
+{
+    jvalue* jArgs;
+    JPy_ArgDisposer* argDisposers;
+    PyObject* returnValue;
+    JPy_JType* returnType;
+
+    //printf("JMethod_InvokeMethod 1: typeCode=%c\n", typeCode);
+    if (JMethod_CreateJArgs(jenv, method, pyArgs, &jArgs, &argDisposers) < 0) {
+        return NULL;
+    }
+
+    //printf("JMethod_InvokeMethod 2: typeCode=%c\n", typeCode);
+
+    returnType = method->returnDescriptor->type;
+    returnValue = NULL;
+
+    if (method->isStatic) {
+        jclass classRef = type->classRef;
+
+        JPy_DIAG_PRINT(JPy_DIAG_F_EXEC, "JMethod_InvokeMethod: calling static Java method %s#%s\n", type->javaName, JPy_AS_UTF8(method->name));
+
+        if (returnType == JPy_JVoid) {
+            (*jenv)->CallStaticVoidMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JVOID();
+        } else if (returnType == JPy_JBoolean) {
+            jboolean v = (*jenv)->CallStaticBooleanMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JBOOLEAN(v);
+        } else if (returnType == JPy_JChar) {
+            jchar v = (*jenv)->CallStaticCharMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JCHAR(v);
+        } else if (returnType == JPy_JByte) {
+            jbyte v = (*jenv)->CallStaticByteMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JBYTE(v);
+        } else if (returnType == JPy_JShort) {
+            jshort v = (*jenv)->CallStaticShortMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JSHORT(v);
+        } else if (returnType == JPy_JInt) {
+            jint v = (*jenv)->CallStaticIntMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JINT(v);
+        } else if (returnType == JPy_JLong) {
+            jlong v = (*jenv)->CallStaticIntMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JLONG(v);
+        } else if (returnType == JPy_JFloat) {
+            jfloat v = (*jenv)->CallStaticFloatMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JFLOAT(v);
+        } else if (returnType == JPy_JDouble) {
+            jdouble v = (*jenv)->CallStaticDoubleMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JDOUBLE(v);
+        } else if (returnType == JPy_JString) {
+            jstring v = (*jenv)->CallStaticObjectMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FromJString(jenv, v);
+            (*jenv)->DeleteLocalRef(jenv, v);
+        } else {
+            jobject v = (*jenv)->CallStaticObjectMethodA(jenv, classRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JMethod_FromJObject(jenv, method, pyArgs, jArgs, 0, returnType, v);
+            (*jenv)->DeleteLocalRef(jenv, v);
+        }
+
+    } else {
+        jobject objectRef;
+        PyObject* self;
+
+        JPy_DIAG_PRINT(JPy_DIAG_F_EXEC, "JMethod_InvokeMethod: calling Java method %s#%s\n", type->javaName, JPy_AS_UTF8(method->name));
+
+        self = PyTuple_GetItem(pyArgs, 0);
+        // Note it is already ensured that self is a JPy_JObj*
+        objectRef = ((JPy_JObj*) self)->objectRef;
+
+        if (returnType == JPy_JVoid) {
+            (*jenv)->CallVoidMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JVOID();
+        } else if (returnType == JPy_JBoolean) {
+            jboolean v = (*jenv)->CallBooleanMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JBOOLEAN(v);
+        } else if (returnType == JPy_JChar) {
+            jchar v = (*jenv)->CallCharMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JCHAR(v);
+        } else if (returnType == JPy_JByte) {
+            jbyte v = (*jenv)->CallByteMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JBYTE(v);
+        } else if (returnType == JPy_JShort) {
+            jshort v = (*jenv)->CallShortMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JSHORT(v);
+        } else if (returnType == JPy_JInt) {
+            jint v = (*jenv)->CallIntMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JINT(v);
+        } else if (returnType == JPy_JLong) {
+            jlong v = (*jenv)->CallIntMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JLONG(v);
+        } else if (returnType == JPy_JFloat) {
+            jfloat v = (*jenv)->CallFloatMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JFLOAT(v);
+        } else if (returnType == JPy_JDouble) {
+            jdouble v = (*jenv)->CallDoubleMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FROM_JDOUBLE(v);
+        } else if (returnType == JPy_JString) {
+            jstring v = (*jenv)->CallObjectMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JPy_FromJString(jenv, v);
+            (*jenv)->DeleteLocalRef(jenv, v);
+        } else {
+            jobject v = (*jenv)->CallObjectMethodA(jenv, objectRef, method->mid, jArgs);
+            JPy_ON_JAVA_EXCEPTION_GOTO(error);
+            returnValue = JMethod_FromJObject(jenv, method, pyArgs, jArgs, 1, returnType, v);
+            (*jenv)->DeleteLocalRef(jenv, v);
+        }
+    }
+
+error:
+    if (jArgs != NULL) {
+        JMethod_DisposeJArgs(jenv, method->paramCount, jArgs, argDisposers);
+    }
+
+    return returnValue;
+}
+
+int JMethod_CreateJArgs(JNIEnv* jenv, JPy_JMethod* method, PyObject* pyArgs, jvalue** argValuesRet, JPy_ArgDisposer** argDisposersRet)
+{
+    JPy_ParamDescriptor* paramDescriptor;
+    int i, i0, argCount;
+    PyObject* pyArg;
+    jvalue* jValue;
+    jvalue* jValues;
+    JPy_ArgDisposer* argDisposer;
+    JPy_ArgDisposer* argDisposers;
+
+    if (method->paramCount == 0) {
+        *argValuesRet = NULL;
+        *argDisposersRet = NULL;
+        return 0;
+    }
+
+    argCount = PyTuple_Size(pyArgs);
+
+    i0 = argCount - method->paramCount;
+    if (!(i0 == 0 || i0 == 1)) {
+        PyErr_SetString(PyExc_RuntimeError, "internal error");
+        return -1;
+    }
+
+    jValues = PyMem_New(jvalue, method->paramCount);
+    if (jValues == NULL) {
+        PyErr_NoMemory();
+        return -1;
+    }
+
+    argDisposers = PyMem_New(JPy_ArgDisposer, method->paramCount);
+    if (argDisposers == NULL) {
+        PyMem_Del(jValues);
+        PyErr_NoMemory();
+        return -1;
+    }
+
+    paramDescriptor = method->paramDescriptors;
+    jValue = jValues;
+    argDisposer = argDisposers;
+    for (i = i0; i < argCount; i++) {
+        pyArg = PyTuple_GetItem(pyArgs, i);
+        jValue->l = 0;
+        argDisposer->data = NULL;
+        argDisposer->DisposeArg = NULL;
+        if (paramDescriptor->ConvertPyArg(jenv, paramDescriptor, pyArg, jValue, argDisposer) < 0) {
+            PyMem_Del(jValues);
+            PyMem_Del(argDisposers);
+            return -1;
+        }
+        paramDescriptor++;
+        jValue++;
+        argDisposer++;
+    }
+
+    *argValuesRet = jValues;
+    *argDisposersRet = argDisposers;
+    return 0;
+}
+
+void JMethod_DisposeJArgs(JNIEnv* jenv, int paramCount, jvalue* jArgs, JPy_ArgDisposer* argDisposers)
+{
+    jvalue* jArg;
+    JPy_ArgDisposer* argDisposer;
+    int index;
+
+    jArg = jArgs;
+    argDisposer = argDisposers;
+
+    for (index = 0; index < paramCount; index++) {
+        if (argDisposer->DisposeArg != NULL) {
+            argDisposer->DisposeArg(jenv, jArg, argDisposer->data);
+        }
+        jArg++;
+        argDisposer++;
+    }
+
+    PyMem_Del(jArgs);
+    PyMem_Del(argDisposers);
+}
+
+
+PyObject* JMethod_repr(JPy_JMethod* self)
+{
+    const char* name = JPy_AS_UTF8(self->name);
+    return JPy_FROM_FORMAT("%s(name='%s', param_count=%d, is_static=%d, mid=%p)",
+                           ((PyObject*)self)->ob_type->tp_name,
+                           name,
+                           self->paramCount,
+                           self->isStatic,
+                           self->mid);
+}
+
+PyObject* JMethod_str(JPy_JMethod* self)
+{
+    Py_INCREF(self->name);
+    return self->name;
+}
+
+
+static PyMemberDef JMethod_members[] =
+{
+    {"name",        T_OBJECT_EX, offsetof(JPy_JMethod, name),       READONLY, "Method name"},
+    {"param_count", T_INT,       offsetof(JPy_JMethod, paramCount), READONLY, "Number of method parameters"},
+    {"is_static",   T_BOOL,      offsetof(JPy_JMethod, isStatic),   READONLY, "Tests if this is a static method"},
+    {NULL}  /* Sentinel */
+};
+
+#define JMethod_CHECK_PARAMETER_INDEX(self, index) \
+    if (index < 0 || index >= self->paramCount) { \
+        PyErr_SetString(PyExc_IndexError, "invalid parameter index"); \
+        return NULL; \
+    }
+
+
+PyObject* JMethod_get_param_type(JPy_JMethod* self, PyObject* args)
+{
+    PyObject* type;
+    int index;
+    if (!PyArg_ParseTuple(args, "i:get_param_type", &index)) {
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    type = (PyObject*) self->paramDescriptors[index].type;
+    Py_INCREF(type);
+    return type;
+}
+
+PyObject* JMethod_is_param_mutable(JPy_JMethod* self, PyObject* args)
+{
+    int index;
+    int value;
+    if (!PyArg_ParseTuple(args, "i:is_param_mutable", &index)) {
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    value = self->paramDescriptors[index].isMutable;
+    return PyBool_FromLong(value);
+}
+
+PyObject* JMethod_set_param_mutable(JPy_JMethod* self, PyObject* args)
+{
+    int index;
+    int value;
+#if defined(JPY_COMPAT_33P)
+    if (!PyArg_ParseTuple(args, "ip:set_param_mutable", &index, &value)) {
+#elif defined(JPY_COMPAT_27)
+    if (!PyArg_ParseTuple(args, "ii:set_param_mutable", &index, &value)) {
+#else
+#error JPY_VERSION_ERROR
+#endif
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    self->paramDescriptors[index].isMutable = value;
+    return Py_BuildValue("");
+}
+
+PyObject* JMethod_is_param_output(JPy_JMethod* self, PyObject* args)
+{
+    int index = 0;
+    int value = 0;
+    if (!PyArg_ParseTuple(args, "i:is_param_output", &index)) {
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    value = self->paramDescriptors[index].isOutput;
+    return PyBool_FromLong(value);
+}
+
+PyObject* JMethod_set_param_output(JPy_JMethod* self, PyObject* args)
+{
+    int index = 0;
+    int value = 0;
+#if defined(JPY_COMPAT_33P)
+    if (!PyArg_ParseTuple(args, "ip:set_param_output", &index, &value)) {
+#elif defined(JPY_COMPAT_27)
+    if (!PyArg_ParseTuple(args, "ii:set_param_output", &index, &value)) {
+#else
+#error JPY_VERSION_ERROR
+#endif
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    self->paramDescriptors[index].isOutput = value;
+    return Py_BuildValue("");
+}
+
+PyObject* JMethod_is_param_return(JPy_JMethod* self, PyObject* args)
+{
+    int index = 0;
+    int value = 0;
+    if (!PyArg_ParseTuple(args, "i:is_param_return", &index)) {
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    value = self->paramDescriptors[index].isReturn;
+    return PyBool_FromLong(value);
+}
+
+PyObject* JMethod_set_param_return(JPy_JMethod* self, PyObject* args)
+{
+    int index = 0;
+    int value = 0;
+#if defined(JPY_COMPAT_33P)
+    if (!PyArg_ParseTuple(args, "ip:set_param_return", &index, &value)) {
+#elif defined(JPY_COMPAT_27)
+    if (!PyArg_ParseTuple(args, "ii:set_param_return", &index, &value)) {
+#else
+#error JPY_VERSION_ERROR
+#endif
+        return NULL;
+    }
+    JMethod_CHECK_PARAMETER_INDEX(self, index);
+    self->paramDescriptors[index].isReturn = value;
+    if (value) {
+        self->returnDescriptor->paramIndex = index;
+    }
+    return Py_BuildValue("");
+}
+
+
+static PyMethodDef JMethod_methods[] =
+{
+    {"get_param_type",    (PyCFunction) JMethod_get_param_type,    METH_VARARGS, "Gets the type of the parameter given by index"},
+    {"is_param_mutable",  (PyCFunction) JMethod_is_param_mutable,  METH_VARARGS, "Tests if the method parameter given by index is mutable"},
+    {"is_param_output",   (PyCFunction) JMethod_is_param_output,   METH_VARARGS, "Tests if the method parameter given by index is a mere output value (and not read from)"},
+    {"is_param_return",   (PyCFunction) JMethod_is_param_return,   METH_VARARGS, "Tests if the method parameter given by index is the return value"},
+    {"set_param_mutable", (PyCFunction) JMethod_set_param_mutable, METH_VARARGS, "Sets whether the method parameter given by index is mutable"},
+    {"set_param_output",  (PyCFunction) JMethod_set_param_output,  METH_VARARGS, "Sets whether the method parameter given by index is a mere output value (and not read from)"},
+    {"set_param_return",  (PyCFunction) JMethod_set_param_return,  METH_VARARGS, "Sets whether the method parameter given by index is the return value"},
+    {NULL}  /* Sentinel */
+};
+
+/**
+ * Implements the BeamPy_JObjectType class singleton.
+ */
+PyTypeObject JMethod_Type = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "jpy.JMethod",                /* tp_name */
+    sizeof (JPy_JMethod),         /* tp_basicsize */
+    0,                            /* tp_itemsize */
+    (destructor)JMethod_dealloc,  /* tp_dealloc */
+    NULL,                         /* tp_print */
+    NULL,                         /* tp_getattr */
+    NULL,                         /* tp_setattr */
+    NULL,                         /* tp_reserved */
+    (reprfunc)JMethod_repr,       /* tp_repr */
+    NULL,                         /* tp_as_number */
+    NULL,                         /* tp_as_sequence */
+    NULL,                         /* tp_as_mapping */
+    NULL,                         /* tp_hash  */
+    NULL,                         /* tp_call */
+    (reprfunc)JMethod_str,        /* tp_str */
+    NULL,                         /* tp_getattro */
+    NULL,                         /* tp_setattro */
+    NULL,                         /* tp_as_buffer */
+    Py_TPFLAGS_DEFAULT,           /* tp_flags */
+    "Java Method Wrapper",        /* tp_doc */
+    NULL,                         /* tp_traverse */
+    NULL,                         /* tp_clear */
+    NULL,                         /* tp_richcompare */
+    0,                            /* tp_weaklistoffset */
+    NULL,                         /* tp_iter */
+    NULL,                         /* tp_iternext */
+    JMethod_methods,              /* tp_methods */
+    JMethod_members,              /* tp_members */
+    NULL,                         /* tp_getset */
+    NULL,                         /* tp_base */
+    NULL,                         /* tp_dict */
+    NULL,                         /* tp_descr_get */
+    NULL,                         /* tp_descr_set */
+    0,                            /* tp_dictoffset */
+    NULL,                         /* tp_init */
+    NULL,                         /* tp_alloc */
+    NULL,                         /* tp_new */
+};
+
+//////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
+//  JOverloadedMethod
+
+typedef struct JPy_MethodFindResult
+{
+    JPy_JMethod* method;
+    int matchValue;
+    int matchCount;
+}
+JPy_MethodFindResult;
+
+JPy_JMethod* JOverloadedMethod_FindMethod0(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* pyArgs, JPy_MethodFindResult* result)
+{
+    int overloadCount;
+    int argCount;
+    int matchCount;
+    int matchValue;
+    int matchValueMax;
+    JPy_JMethod* currMethod;
+    JPy_JMethod* bestMethod;
+    int i;
+
+    result->method = NULL;
+    result->matchValue = 0;
+    result->matchCount = 0;
+
+    overloadCount = PyList_Size(overloadedMethod->methodList);
+    if (overloadCount <= 0) {
+        PyErr_SetString(PyExc_RuntimeError, "internal error: invalid overloadedMethod->methodList");
+        return NULL;
+    }
+
+    argCount = PyTuple_Size(pyArgs);
+    matchCount = 0;
+    matchValueMax = -1;
+    bestMethod = NULL;
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JOverloadedMethod_FindMethod0: method '%s#%s': overloadCount=%d\n",
+                              overloadedMethod->declaringClass->javaName, JPy_AS_UTF8(overloadedMethod->name), overloadCount);
+
+    for (i = 0; i < overloadCount; i++) {
+        currMethod = (JPy_JMethod*) PyList_GetItem(overloadedMethod->methodList, i);
+        matchValue = JMethod_MatchPyArgs(jenv, currMethod, argCount, pyArgs);
+
+        JPy_DIAG_PRINT(JPy_DIAG_F_METH, "JOverloadedMethod_FindMethod0: methodList[%d]: paramCount=%d, matchValue=%d\n", i,
+                                  currMethod->paramCount, matchValue);
+
+        if (matchValue > 0) {
+            if (matchValue > matchValueMax) {
+                matchValueMax = matchValue;
+                bestMethod = currMethod;
+                matchCount = 1;
+            } else if (matchValue == matchValueMax) {
+                matchCount++;
+            }
+            if (matchValue >= 100 * currMethod->paramCount) {
+                // we can't get any better (if so, we have an internal problem)
+                break;
+            }
+        }
+    }
+
+    if (bestMethod == NULL) {
+        matchValueMax = 0;
+        matchCount = 0;
+    }
+
+    result->method = bestMethod;
+    result->matchValue = matchValueMax;
+    result->matchCount = matchCount;
+
+    return bestMethod;
+}
+
+JPy_JMethod* JOverloadedMethod_FindMethod(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* pyArgs, jboolean visitSuperClass)
+{
+    JPy_JOverloadedMethod* currentOM;
+    JPy_MethodFindResult result;
+    JPy_MethodFindResult bestResult;
+    JPy_JType* superClass;
+    PyObject* superOM;
+
+    if ((JPy_DiagFlags & JPy_DIAG_F_METH) != 0) {
+        int i, argCount = PyTuple_Size(pyArgs);
+        printf("JOverloadedMethod_FindMethod: argCount=%d, visitSuperClass=%d\n", argCount, visitSuperClass);
+        for (i = 0; i < argCount; i++) {
+            PyObject* pyArg = PyTuple_GetItem(pyArgs, i);
+            printf("\tPy_TYPE(pyArgs[%d])->tp_name = %s\n", i, Py_TYPE(pyArg)->tp_name);
+        }
+    }
+
+    bestResult.method = NULL;
+    bestResult.matchValue = 0;
+    bestResult.matchCount = 0;
+
+    currentOM = overloadedMethod;
+    while (1) {
+        if (JOverloadedMethod_FindMethod0(jenv, currentOM, pyArgs, &result) < 0) {
+            // oops, error
+            return NULL;
+        }
+        if (result.method != NULL) {
+            if (result.matchValue >= 100 * result.method->paramCount) {
+                // We can't get any better.
+                return result.method;
+            } else if (result.matchValue > 0 && result.matchValue > bestResult.matchValue) {
+                // We may have better matching methods overloads in the super class (if any)
+                bestResult = result;
+            }
+        }
+
+        if (visitSuperClass) {
+            superClass = currentOM->declaringClass->superType;
+            if (superClass != NULL) {
+                superOM = JType_GetOverloadedMethod(jenv, superClass, currentOM->name, JNI_TRUE);
+            } else {
+                superOM = Py_None;
+            }
+        } else {
+            superOM = Py_None;
+        }
+
+        if (superOM == NULL) {
+            // oops, error
+            return NULL;
+        } else if (superOM == Py_None) {
+            // no overloaded methods found in super class, so return best result found so far
+            if (bestResult.method == NULL) {
+                PyErr_SetString(PyExc_RuntimeError, "no matching Java method overloads found");
+                return NULL;
+            } else if (bestResult.matchCount > 1) {
+                PyErr_SetString(PyExc_RuntimeError, "ambiguous Java method call, too many matching method overloads found");
+                return NULL;
+            } else {
+                return bestResult.method;
+            }
+        } else {
+            // Continue trying with overloads from super type
+            currentOM = (JPy_JOverloadedMethod*) superOM;
+        }
+    }
+
+    // Should never come here
+    PyErr_SetString(PyExc_RuntimeError, "internal error");
+    return NULL;
+}
+
+JPy_JOverloadedMethod* JOverloadedMethod_New(JPy_JType* declaringClass, PyObject* name, JPy_JMethod* method)
+{
+    PyTypeObject* methodType = &JOverloadedMethod_Type;
+    JPy_JOverloadedMethod* overloadedMethod;
+
+    overloadedMethod = (JPy_JOverloadedMethod*) methodType->tp_alloc(methodType, 0);
+    overloadedMethod->declaringClass = declaringClass;
+    overloadedMethod->name = name;
+    overloadedMethod->methodList = PyList_New(0);
+
+    Py_INCREF((PyObject*) overloadedMethod->declaringClass);
+    Py_INCREF((PyObject*) overloadedMethod->name);
+    Py_INCREF((PyObject*) overloadedMethod);
+
+    JOverloadedMethod_AddMethod(overloadedMethod, method);
+
+    return overloadedMethod;
+}
+
+int JOverloadedMethod_AddMethod(JPy_JOverloadedMethod* overloadedMethod, JPy_JMethod* method)
+{
+    return PyList_Append(overloadedMethod->methodList, (PyObject*) method);
+}
+
+/**
+ * The 'JOverloadedMethod' type's tp_dealloc slot.
+ */
+void JOverloadedMethod_dealloc(JPy_JOverloadedMethod* self)
+{
+    Py_DECREF((PyObject*) self->declaringClass);
+    Py_DECREF((PyObject*) self->name);
+    Py_DECREF((PyObject*) self->methodList);
+    Py_TYPE(self)->tp_free((PyObject*) self);
+}
+
+/**
+ * The 'JOverloadedMethod' type's tp_call slot. Makes instances of the 'JOverloadedMethod' type callable.
+ */
+PyObject* JOverloadedMethod_call(JPy_JOverloadedMethod* self, PyObject *args, PyObject *kw)
+{
+    JNIEnv* jenv;
+    JPy_JMethod* method;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
+
+    method = JOverloadedMethod_FindMethod(jenv, self, args, JNI_TRUE);
+    if (method == NULL) {
+        return NULL;
+    }
+
+    return JMethod_InvokeMethod(jenv, method, self->declaringClass, args);
+}
+
+/**
+ * The 'JOverloadedMethod' type's tp_repr slot.
+ */
+PyObject* JOverloadedMethod_repr(JPy_JOverloadedMethod* self)
+{
+    const char* name = JPy_AS_UTF8(self->name);
+    int methodCount = PyList_Size(self->methodList);
+    return JPy_FROM_FORMAT("%s(name='%s', methodCount=%d)",
+                           ((PyObject*)self)->ob_type->tp_name,
+                           name,
+                           methodCount);
+}
+
+static PyMemberDef JOverloadedMethod_members[] =
+{
+    {"name",    T_OBJECT_EX, offsetof(JPy_JOverloadedMethod, name),       READONLY, "Overloaded method name"},
+    {"methods", T_OBJECT_EX, offsetof(JPy_JOverloadedMethod, methodList), READONLY, "List of methods"},
+    {NULL}  /* Sentinel */
+};
+
+/**
+ * The 'JOverloadedMethod' type's tp_str slot.
+ */
+PyObject* JOverloadedMethod_str(JPy_JOverloadedMethod* self)
+{
+    Py_INCREF(self->name);
+    return self->name;
+}
+
+PyTypeObject JOverloadedMethod_Type = {
+    PyVarObject_HEAD_INIT(NULL, 0)
+    "jpy.JOverloadedMethod",                /* tp_name */
+    sizeof (JPy_JOverloadedMethod),         /* tp_basicsize */
+    0,                            /* tp_itemsize */
+    (destructor)JOverloadedMethod_dealloc,  /* tp_dealloc */
+    NULL,                         /* tp_print */
+    NULL,                         /* tp_getattr */
+    NULL,                         /* tp_setattr */
+    NULL,                         /* tp_reserved */
+    (reprfunc)JOverloadedMethod_repr,       /* tp_repr */
+    NULL,                         /* tp_as_number */
+    NULL,                         /* tp_as_sequence */
+    NULL,                         /* tp_as_mapping */
+    NULL,                         /* tp_hash  */
+    (ternaryfunc)JOverloadedMethod_call,    /* tp_call */
+    (reprfunc)JOverloadedMethod_str,        /* tp_str */
+    NULL,                         /* tp_getattro */
+    NULL,                         /* tp_setattro */
+    NULL,                         /* tp_as_buffer */
+    Py_TPFLAGS_DEFAULT,           /* tp_flags */
+    "Java Overloaded Method",     /* tp_doc */
+    NULL,                         /* tp_traverse */
+    NULL,                         /* tp_clear */
+    NULL,                         /* tp_richcompare */
+    0,                            /* tp_weaklistoffset */
+    NULL,                         /* tp_iter */
+    NULL,                         /* tp_iternext */
+    NULL,                         /* tp_methods */
+    JOverloadedMethod_members,    /* tp_members */
+    NULL,                         /* tp_getset */
+    NULL,                         /* tp_base */
+    NULL,                         /* tp_dict */
+    NULL,                         /* tp_descr_get */
+    NULL,                         /* tp_descr_set */
+    0,                            /* tp_dictoffset */
+    NULL,                         /* tp_init */
+    NULL,                         /* tp_alloc */
+    NULL,                         /* tp_new */
+};
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jmethod.h` & `jpy-0.7.5/src/main/c/jpy_jmethod.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,93 +1,94 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_JMETHOD_H
-#define JPY_JMETHOD_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-
-/**
- * Python object representing a Java method. It's type is 'JMethod'.
- */
-typedef struct
-{
-    PyObject_HEAD
-
-    // Method name.
-    PyObject* name;
-    // Method parameter count.
-    int paramCount;
-    // Method is static?
-    char isStatic;
-    // Method parameter types. Will be NULL, if parameter_count == 0.
-    JPy_ParamDescriptor* paramDescriptors;
-    // Method return type. Will be NULL for constructors.
-    JPy_ReturnDescriptor* returnDescriptor;
-    // Method ID retrieved from JNI.
-    jmethodID mid;
-}
-JPy_JMethod;
-
-/**
- * The Python 'JMethod' type singleton.
- */
-extern PyTypeObject JMethod_Type;
-
-/**
- * Python object representing an overloaded Java method. It's type is 'JOverloadedMethod'.
- */
-typedef struct
-{
-    PyObject_HEAD
-
-    // The declaring class.
-    JPy_JType* declaringClass;
-    // Method name.
-    PyObject* name;
-    // List of method overloads (a PyList with items of type JPy_JMethod).
-    PyObject* methodList;
-}
-JPy_JOverloadedMethod;
-
-/**
- * The Python 'JOverloadedMethod' type singleton.
- */
-extern PyTypeObject JOverloadedMethod_Type;
-
-JPy_JMethod*           JOverloadedMethod_FindMethod(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* argTuple, jboolean visitSuperClass);
-JPy_JMethod*           JOverloadedMethod_FindStaticMethod(JPy_JOverloadedMethod* overloadedMethod, PyObject* argTuple);
-JPy_JOverloadedMethod* JOverloadedMethod_New(JPy_JType* declaringClass, PyObject* name, JPy_JMethod* method);
-int                    JOverloadedMethod_AddMethod(JPy_JOverloadedMethod* overloadedMethod, JPy_JMethod* method);
-
-JPy_JMethod* JMethod_New(PyObject* name,
-                         int paramCount,
-                         JPy_ParamDescriptor* paramDescriptors,
-                         JPy_ReturnDescriptor* returnDescriptor,
-                         jboolean isStatic,
-                         jmethodID mid);
-
-void JMethod_Del(JPy_JMethod* method);
-
-int JMethod_ConvertToJavaValues(JNIEnv* jenv, JPy_JMethod* jMethod, int argCount, PyObject* argTuple, jvalue* jArgs);
-
-int  JMethod_CreateJArgs(JNIEnv* jenv, JPy_JMethod* jMethod, PyObject* argTuple, jvalue** jValues, JPy_ArgDisposer** jDisposers);
-void JMethod_DisposeJArgs(JNIEnv* jenv, int paramCount, jvalue* jValues, JPy_ArgDisposer* jDisposers);
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
-
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_JMETHOD_H
+#define JPY_JMETHOD_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+/**
+ * Python object representing a Java method. It's type is 'JMethod'.
+ */
+typedef struct
+{
+    PyObject_HEAD
+
+    // Method name.
+    PyObject* name;
+    // Method parameter count.
+    int paramCount;
+    // Method is static?
+    char isStatic;
+    // Method parameter types. Will be NULL, if parameter_count == 0.
+    JPy_ParamDescriptor* paramDescriptors;
+    // Method return type. Will be NULL for constructors.
+    JPy_ReturnDescriptor* returnDescriptor;
+    // Method ID retrieved from JNI.
+    jmethodID mid;
+}
+JPy_JMethod;
+
+/**
+ * The Python 'JMethod' type singleton.
+ */
+extern PyTypeObject JMethod_Type;
+
+/**
+ * Python object representing an overloaded Java method. It's type is 'JOverloadedMethod'.
+ */
+typedef struct
+{
+    PyObject_HEAD
+
+    // The declaring class.
+    JPy_JType* declaringClass;
+    // Method name.
+    PyObject* name;
+    // List of method overloads (a PyList with items of type JPy_JMethod).
+    PyObject* methodList;
+}
+JPy_JOverloadedMethod;
+
+/**
+ * The Python 'JOverloadedMethod' type singleton.
+ */
+extern PyTypeObject JOverloadedMethod_Type;
+
+JPy_JMethod*           JOverloadedMethod_FindMethod(JNIEnv* jenv, JPy_JOverloadedMethod* overloadedMethod, PyObject* argTuple, jboolean visitSuperClass);
+JPy_JMethod*           JOverloadedMethod_FindStaticMethod(JPy_JOverloadedMethod* overloadedMethod, PyObject* argTuple);
+JPy_JOverloadedMethod* JOverloadedMethod_New(JPy_JType* declaringClass, PyObject* name, JPy_JMethod* method);
+int                    JOverloadedMethod_AddMethod(JPy_JOverloadedMethod* overloadedMethod, JPy_JMethod* method);
+
+JPy_JMethod* JMethod_New(PyObject* name,
+                         int paramCount,
+                         JPy_ParamDescriptor* paramDescriptors,
+                         JPy_ReturnDescriptor* returnDescriptor,
+                         jboolean isStatic,
+                         jmethodID mid);
+
+void JMethod_Del(JPy_JMethod* method);
+
+int JMethod_ConvertToJavaValues(JNIEnv* jenv, JPy_JMethod* jMethod, int argCount, PyObject* argTuple, jvalue* jArgs);
+
+int  JMethod_CreateJArgs(JNIEnv* jenv, JPy_JMethod* jMethod, PyObject* argTuple, jvalue** jValues, JPy_ArgDisposer** jDisposers);
+void JMethod_DisposeJArgs(JNIEnv* jenv, int paramCount, jvalue* jValues, JPy_ArgDisposer* jDisposers);
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
+
 #endif /* !JPY_JMETHOD_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jobj.c` & `jpy-0.7.5/src/main/c/jpy_jobj.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,776 +1,778 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#include "jpy_module.h"
-#include "jpy_diag.h"
-#include "jpy_jarray.h"
-#include "jpy_jtype.h"
-#include "jpy_jobj.h"
-#include "jpy_jmethod.h"
-#include "jpy_jfield.h"
-#include "jpy_conv.h"
-
-JPy_JObj* JObj_New(JNIEnv* jenv, jobject objectRef)
-{
-    jclass classRef;
-    JPy_JType* type;
-
-    classRef = (*jenv)->GetObjectClass(jenv, objectRef);
-    type = JType_GetType(jenv, classRef, JNI_TRUE);
-    (*jenv)->DeleteLocalRef(jenv, classRef);
-    if (type == NULL) {
-        return NULL;
-    }
-
-    return JObj_FromType(jenv, type, objectRef);
-}
-
-JPy_JObj* JObj_FromType(JNIEnv* jenv, JPy_JType* type, jobject objectRef)
-{
-    JPy_JObj* obj;
-
-    obj = (JPy_JObj*) PyObject_New(JPy_JObj, (PyTypeObject*) type);
-    if (obj == NULL) {
-        return NULL;
-    }
-
-    objectRef = (*jenv)->NewGlobalRef(jenv, objectRef);
-    if (objectRef == NULL) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-
-    obj->objectRef = objectRef;
-
-    // For special treatment of primitive array refer to JType_InitSlots()
-    if (type->componentType != NULL && type->componentType->isPrimitive) {
-        JPy_JArray* array;
-
-        array = (JPy_JArray*) obj;
-        array->bufferExportCount = 0;
-    }
-
-    return obj;
-}
-
-/**
- * The JObj type's tp_init slot. Called when the type is used to create new instances (constructor).
- */
-int JObj_init(JPy_JObj* self, PyObject* args, PyObject* kwds)
-{
-    JNIEnv* jenv;
-    PyTypeObject* type;
-    JPy_JType* jType;
-    PyObject* constructor;
-    JPy_JMethod* jMethod;
-    jobject objectRef;
-    jvalue* jArgs;
-    JPy_ArgDisposer* jDisposers;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
-
-    type = ((PyObject*) self)->ob_type;
-
-    constructor = PyDict_GetItemString(type->tp_dict, JPy_JTYPE_ATTR_NAME_JINIT);
-    if (constructor == NULL) {
-        PyErr_SetString(PyExc_RuntimeError, "no constructor found (missing JType attribute '" JPy_JTYPE_ATTR_NAME_JINIT "')");
-        return -1;
-    }
-
-    if (!PyObject_TypeCheck(constructor, &JOverloadedMethod_Type)) {
-        PyErr_SetString(PyExc_RuntimeError, "invalid JType attribute '"  JPy_JTYPE_ATTR_NAME_JINIT  "': expected type JOverloadedMethod_Type");
-        return -1;
-    }
-
-    jType = (JPy_JType*) type;
-    if (jType->classRef == NULL) {
-        PyErr_SetString(PyExc_RuntimeError, "internal error: Java class reference is NULL");
-        return -1;
-    }
-
-    jMethod = JOverloadedMethod_FindMethod(jenv, (JPy_JOverloadedMethod*) constructor, args, JNI_FALSE);
-    if (jMethod == NULL) {
-        return -1;
-    }
-
-    if (JMethod_CreateJArgs(jenv, jMethod, args, &jArgs, &jDisposers) < 0) {
-        return -1;
-    }
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_init: calling Java constructor %s\n", jType->javaName);
-
-    objectRef = (*jenv)->NewObjectA(jenv, jType->classRef, jMethod->mid, jArgs);
-    JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-
-    if (objectRef == NULL) {
-        PyErr_NoMemory();
-        return -1;
-    }
-
-    if (jMethod->paramCount > 0) {
-        JMethod_DisposeJArgs(jenv, jMethod->paramCount, jArgs, jDisposers);
-    }
-
-    objectRef = (*jenv)->NewGlobalRef(jenv, objectRef);
-    if (objectRef == NULL) {
-        PyErr_NoMemory();
-        return -1;
-    }
-
-    // Note:  __init__ may be called multiple times, so we have to release the old objectRef
-    if (self->objectRef != NULL) {
-        (*jenv)->DeleteGlobalRef(jenv, self->objectRef);
-    }
-
-    self->objectRef = objectRef;
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_init: self->objectRef=%p\n", self->objectRef);
-
-    return 0;
-}
-
-/**
- * The JObj type's tp_dealloc slot. Called when the reference count reaches zero.
- */
-void JObj_dealloc(JPy_JObj* self)
-{
-    JNIEnv* jenv;
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_dealloc: releasing instance of %s, self->objectRef=%p\n", Py_TYPE(self)->tp_name, self->objectRef);
-
-    jenv = JPy_GetJNIEnv();
-    if (jenv != NULL) {
-        if (self->objectRef != NULL) {
-            (*jenv)->DeleteGlobalRef(jenv, self->objectRef);
-        }
-    }
-
-    Py_TYPE(self)->tp_free((PyObject*) self);
-}
-
-int JObj_CompareTo(JNIEnv* jenv, JPy_JObj* obj1, JPy_JObj* obj2)
-{
-    jobject ref1;
-    jobject ref2;
-    int value;
-
-    ref1 = obj1->objectRef;
-    ref2 = obj2->objectRef;
-
-    if (ref1 == ref2 || (*jenv)->IsSameObject(jenv, ref1, ref2)) {
-        return 0;
-    } else if ((*jenv)->IsInstanceOf(jenv, ref1, JPy_Comparable_JClass)) {
-        value = (*jenv)->CallIntMethod(jenv, ref1, JPy_Comparable_CompareTo_MID, ref2);
-        (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
-    } else {
-        value = (char*) ref1 - (char*) ref2;
-    }
-
-    return (value == 0) ? 0 : (value < 0) ? -1 : +1;
-}
-
-int JObj_Equals(JNIEnv* jenv, JPy_JObj* obj1, JPy_JObj* obj2)
-{
-    jobject ref1;
-    jobject ref2;
-    int returnValue;
-
-    ref1 = obj1->objectRef;
-    ref2 = obj2->objectRef;
-
-    if ((*jenv)->IsSameObject(jenv, ref1, ref2)) {
-        returnValue = 1;
-    } else {
-        returnValue = (*jenv)->CallIntMethod(jenv, ref1, JPy_Object_Equals_MID, ref2);
-    }
-    (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
-    return returnValue;
-}
-
-/**
- * The JObj type's tp_richcompare slot. Python: obj1 <opid> obj2
- */
-PyObject* JObj_richcompare(PyObject* obj1, PyObject* obj2, int opid)
-{
-    JNIEnv* jenv;
-
-    if (!JObj_Check(obj1) || !JObj_Check(obj2)) {
-        Py_RETURN_FALSE;
-    }
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL);
-
-    if (opid == Py_LT) {
-        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value == -1) {
-            Py_RETURN_TRUE;
-        } else {
-            Py_RETURN_FALSE;
-        }
-    } else if (opid == Py_LE) {
-        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value == -1 || value == 0) {
-            Py_RETURN_TRUE;
-        } else {
-            Py_RETURN_FALSE;
-        }
-    } else if (opid == Py_GT) {
-        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value == +1) {
-            Py_RETURN_TRUE;
-        } else {
-            Py_RETURN_FALSE;
-        }
-    } else if (opid == Py_GE) {
-        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value == +1 || value == 0) {
-            Py_RETURN_TRUE;
-        } else {
-            Py_RETURN_FALSE;
-        }
-    } else if (opid == Py_EQ) {
-        int value = JObj_Equals(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value) {
-            Py_RETURN_TRUE;
-        } else {
-            Py_RETURN_FALSE;
-        }
-    } else if (opid == Py_NE) {
-        int value = JObj_Equals(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
-        if (value == -2) {
-            return NULL;
-        } else if (value) {
-            Py_RETURN_FALSE;
-        } else {
-            Py_RETURN_TRUE;
-        }
-    } else {
-        PyErr_SetString(PyExc_RuntimeError, "internal error: unrecognized opid");
-        return NULL;
-    }
-}
-
-/**
- * The JObj type's tp_hash slot. Python: hash(obj)
- */
-long JObj_hash(JPy_JObj* self)
-{
-    JNIEnv* jenv;
-    jenv = JPy_GetJNIEnv();
-    if (jenv != NULL) {
-        int returnValue = (*jenv)->CallIntMethod(jenv, self->objectRef, JPy_Object_HashCode_MID);
-        (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
-        return returnValue;
-    }
-    return -1;
-}
-
-
-/**
- * The JObj type's tp_repr slot. Python: repr(obj))
- */
-PyObject* JObj_repr(JPy_JObj* self)
-{
-    return JPy_FROM_FORMAT("%s(objectRef=%p)", Py_TYPE(self)->tp_name, self->objectRef);
-}
-
-/**
- * The JObj type's tp_str slot. Calls Object.toString() on Java Objects. Python: str(obj)
- */
-PyObject* JObj_str(JPy_JObj* self)
-{
-    JNIEnv* jenv;
-    jstring stringRef;
-    PyObject* returnValue;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
-
-    if (self->objectRef == NULL) {
-        return Py_BuildValue("");
-    }
-
-    returnValue = NULL;
-    stringRef = (*jenv)->CallObjectMethod(jenv, self->objectRef, JPy_Object_ToString_MID);
-    JPy_ON_JAVA_EXCEPTION_GOTO(error);
-    returnValue = JPy_FromJString(jenv, stringRef);
-
-error:
-    (*jenv)->DeleteLocalRef(jenv, stringRef);
-
-    return returnValue;
-}
-
-
-/**
- * The JObj type's tp_setattro slot.
- */
-int JObj_setattro(JPy_JObj* self, PyObject* name, PyObject* value)
-{
-    PyObject* oldValue;
-
-    //printf("JObj_setattro: %s.%s\n", Py_TYPE(self)->tp_name, JPy_AS_UTF8(name));
-
-    oldValue = PyObject_GenericGetAttr((PyObject*) self, name);
-    if (oldValue != NULL && PyObject_TypeCheck(oldValue, &JField_Type)) {
-        JNIEnv* jenv;
-        JPy_JField* field;
-        JPy_JType* type;
-
-        field = (JPy_JField*) oldValue;
-        type = field->type;
-
-        JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
-
-        if (type == JPy_JBoolean) {
-            jboolean item = JPy_AS_JBOOLEAN(value);
-            (*jenv)->SetBooleanField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JChar) {
-            jchar item = JPy_AS_JCHAR(value);
-            (*jenv)->SetCharField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JByte) {
-            jbyte item = JPy_AS_JBYTE(value);
-            (*jenv)->SetByteField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JShort) {
-            jshort item = JPy_AS_JSHORT(value);
-            (*jenv)->SetShortField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JInt) {
-            jint item = JPy_AS_JINT(value);
-            (*jenv)->SetIntField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JLong) {
-            jlong item = JPy_AS_JLONG(value);
-            (*jenv)->SetLongField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JFloat) {
-            jfloat item = JPy_AS_JFLOAT(value);
-            (*jenv)->SetFloatField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else if (type == JPy_JDouble) {
-            jdouble item = JPy_AS_JDOUBLE(value);
-            (*jenv)->SetDoubleField(jenv, self->objectRef, field->fid, item);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        } else {
-            jobject objectRef;
-            if (JPy_AsJObjectWithType(jenv, value, &objectRef, field->type) < 0) {
-                return -1;
-            }
-            (*jenv)->SetObjectField(jenv, self->objectRef, field->fid, objectRef);
-            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-        }
-        return 0;
-    } else {
-        return PyObject_GenericSetAttr((PyObject*) self, name, value);
-    }
-}
-
-/**
- * The JObj type's tp_getattro slot.
- * This is important: wrap callable objects of type JOverloadedMethod_Type into python methods so that
- * a method call to an instance x of class X becomes: x.m() --> X.m(x)
- */
-PyObject* JObj_getattro(JPy_JObj* self, PyObject* name)
-{
-    JPy_JType* selfType;
-    PyObject* value;
-
-    //printf("JObj_getattro: %s.%s\n", Py_TYPE(self)->tp_name, JPy_AS_UTF8(name));
-
-    // First make sure that the Java type is resolved, otherwise we won't find any methods at all.
-    selfType = (JPy_JType*) Py_TYPE(self);
-    if (!selfType->isResolved) {
-        JNIEnv* jenv;
-        JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
-        if (JType_ResolveType(jenv, selfType) < 0) {
-            return NULL;
-        }
-    }
-
-    // todo: implement a special lookup: we need to override __getattro__ of JType (--> JType_getattro) as well so that we know if a method
-    // is called on a class rather than on an instance. Using PyObject_GenericGetAttr will also call  JType_getattro,
-    // but then we loose the information that a method is called on an instance and not on a class.
-    value = PyObject_GenericGetAttr((PyObject*) self, name);
-    if (value == NULL) {
-        //printf("JObj_getattro: not found!\n");
-        return NULL;
-    }
-    if (PyObject_TypeCheck(value, &JOverloadedMethod_Type)) {
-        //JPy_JOverloadedMethod* overloadedMethod = (JPy_JOverloadedMethod*) value;
-        //printf("JObj_getattro: wrapping JOverloadedMethod, overloadCount=%d\n", PyList_Size(overloadedMethod->methodList));
-#if PY_MAJOR_VERSION >= 3
-        return PyMethod_New(value, (PyObject*) self);
-#else
-        // todo: py27: 3rd arg must be class of self, check if NULL is ok here
-        return PyMethod_New(value, (PyObject*) self, NULL);
-#endif
-    } else if (PyObject_TypeCheck(value, &JField_Type)) {
-        JNIEnv* jenv;
-        JPy_JField* field;
-        JPy_JType* type;
-
-        field = (JPy_JField*) value;
-        type = field->type;
-
-        JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
-
-        if (type == JPy_JBoolean) {
-            jboolean item = (*jenv)->GetBooleanField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JBOOLEAN(item);
-        } else if (type == JPy_JChar) {
-            jchar item = (*jenv)->GetCharField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JCHAR(item);
-        } else if (type == JPy_JByte) {
-            jbyte item = (*jenv)->GetByteField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JBYTE(item);
-        } else if (type == JPy_JShort) {
-            jshort item = (*jenv)->GetShortField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JSHORT(item);
-        } else if (type == JPy_JInt) {
-            jint item = (*jenv)->GetIntField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JINT(item);
-        } else if (type == JPy_JLong) {
-            jlong item = (*jenv)->GetLongField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JLONG(item);
-        } else if (type == JPy_JFloat) {
-            jfloat item = (*jenv)->GetFloatField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JFLOAT(item);
-        } else if (type == JPy_JDouble) {
-            jdouble item = (*jenv)->GetDoubleField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            return JPy_FROM_JDOUBLE(item);
-        } else {
-            PyObject* returnValue;
-            jobject item = (*jenv)->GetObjectField(jenv, self->objectRef, field->fid);
-            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-            returnValue = JPy_FromJObjectWithType(jenv, item, field->type);
-            (*jenv)->DeleteLocalRef(jenv, item);
-            return returnValue;
-        }
-    } else {
-        //printf("JObj_getattro: passing through\n");
-    }
-    return value;
-}
-
-/**
- * The JObj type's sq_length field of the tp_as_sequence slot. Called if len(obj) is called.
- * Only used for array types (type->componentType != NULL).
- */
-Py_ssize_t JObj_sq_length(JPy_JObj* self)
-{
-    JNIEnv* jenv;
-    jsize length;
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
-    length = (*jenv)->GetArrayLength(jenv, self->objectRef);
-    //printf("JObj_sq_length: length=%d\n", length);
-    return (Py_ssize_t) length;
-}
-
-/*
- * The JObj type's sq_item field of the tp_as_sequence slot. Called if 'item = obj[index]' is used.
- * Only used for array types (type->componentType != NULL).
- */
-PyObject* JObj_sq_item(JPy_JObj* self, Py_ssize_t index)
-{
-    JNIEnv* jenv;
-    JPy_JType* type;
-    JPy_JType* componentType;
-    jsize length;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
-
-    //printf("JObj_sq_item: index=%d\n", index);
-
-    type = (JPy_JType*) Py_TYPE(self);
-    componentType = type->componentType;
-    if (componentType == NULL) {
-        PyErr_SetString(PyExc_RuntimeError, "internal error: object is not an array");
-        return NULL;
-    }
-
-    // This is annoying and slow in Python 3.3.2: We must have this check, in order to raise an PyExc_IndexError,
-    // otherwise Python functions such as list(jarr) will not succeed.
-    // Tis is really strange, because n = sq_length() will be called and subsequent sq_item(index=0 ... n) calls will be done.
-    length = (*jenv)->GetArrayLength(jenv, self->objectRef);
-    if (index < 0 || index >= length) {
-        PyErr_SetString(PyExc_IndexError, "Java array index out of bounds");
-        return NULL;
-    }
-
-    if (componentType == JPy_JBoolean) {
-        jboolean item;
-        (*jenv)->GetBooleanArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JBOOLEAN(item);
-    } else if (componentType == JPy_JChar) {
-        jchar item;
-        (*jenv)->GetCharArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JCHAR(item);
-    } else if (componentType == JPy_JByte) {
-        jbyte item;
-        (*jenv)->GetByteArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JBYTE(item);
-    } else if (componentType == JPy_JShort) {
-        jshort item;
-        (*jenv)->GetShortArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JSHORT(item);
-    } else if (componentType == JPy_JInt) {
-        jint item;
-        (*jenv)->GetIntArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JINT(item);
-    } else if (componentType == JPy_JLong) {
-        jlong item;
-        (*jenv)->GetLongArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JLONG(item);
-    } else if (componentType == JPy_JFloat) {
-        jfloat item;
-        (*jenv)->GetFloatArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JFLOAT(item);
-    } else if (componentType == JPy_JDouble) {
-        jdouble item;
-        (*jenv)->GetDoubleArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        return JPy_FROM_JDOUBLE(item);
-    } else {
-        PyObject* returnValue;
-        jobject item = (*jenv)->GetObjectArrayElement(jenv, self->objectRef, (jsize) index);
-        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
-        returnValue = JPy_FromJObjectWithType(jenv, item, type->componentType);
-        (*jenv)->DeleteLocalRef(jenv, item);
-        return returnValue;
-    }
-}
-
-/*
- * The JObj type's sq_ass_item field of the tp_as_sequence slot. Called if 'obj[index] = item' is used.
- * Only used for array types (type->componentType != NULL).
- */
-int JObj_sq_ass_item(JPy_JObj* self, Py_ssize_t index, PyObject* pyItem)
-{
-    JNIEnv* jenv;
-    JPy_JType* type;
-    JPy_JType* componentType;
-
-    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
-
-    type = (JPy_JType*) Py_TYPE(self);
-    componentType = type->componentType;
-    if (type->componentType == NULL) {
-        PyErr_SetString(PyExc_RuntimeError, "internal error: object is not an array");
-        return -1;
-    }
-
-    // Note: the following item assignments are not value range checked
-    if (componentType == JPy_JBoolean) {
-        jboolean item = JPy_AS_JBOOLEAN(pyItem);
-        (*jenv)->SetBooleanArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JChar) {
-        jchar item = JPy_AS_JCHAR(pyItem);
-        (*jenv)->SetCharArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JByte) {
-        jbyte item = JPy_AS_JBYTE(pyItem);
-        (*jenv)->SetByteArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JShort) {
-        jshort item = JPy_AS_JSHORT(pyItem);
-        (*jenv)->SetShortArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JInt) {
-        jint item = JPy_AS_JINT(pyItem);
-        (*jenv)->SetIntArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JLong) {
-        jlong item = JPy_AS_JLONG(pyItem);
-        (*jenv)->SetLongArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JFloat) {
-        jfloat item = JPy_AS_JFLOAT(pyItem);
-        (*jenv)->SetFloatArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else if (componentType == JPy_JDouble) {
-        jdouble item = JPy_AS_JDOUBLE(pyItem);
-        (*jenv)->SetDoubleArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    } else {
-        jobject item;
-        if (JPy_AsJObjectWithType(jenv, pyItem, &item, type->componentType) < 0) {
-            return -1;
-        }
-        (*jenv)->SetObjectArrayElement(jenv, self->objectRef, (jsize) index, item);
-        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
-    }
-    return 0;
-}
-
-/**
- * The JObj type's tp_as_sequence slot.
- * Implements the <sequence> interface for array types (type->componentType != NULL).
- */
-static PySequenceMethods JObj_as_sequence = {
-    (lenfunc) JObj_sq_length,            /* sq_length */
-    NULL,   /* sq_concat */
-    NULL,   /* sq_repeat */
-    (ssizeargfunc) JObj_sq_item,         /* sq_item */
-    NULL,   /* was_sq_slice */
-    (ssizeobjargproc) JObj_sq_ass_item,  /* sq_ass_item */
-    NULL,   /* was_sq_ass_slice */
-    NULL,   /* sq_contains */
-    NULL,   /* sq_inplace_concat */
-    NULL,   /* sq_inplace_repeat */
-};
-
-
-int JType_InitSlots(JPy_JType* type)
-{
-    PyTypeObject* typeObj;
-    jboolean isArray;
-    jboolean isPrimitiveArray;
-
-    isArray = type->componentType != NULL;
-    isPrimitiveArray = isArray && type->componentType->isPrimitive;
-
-    typeObj = (PyTypeObject*) type;
-
-    Py_REFCNT(typeObj) = 1;
-    Py_TYPE(typeObj) = NULL;
-    Py_SIZE(typeObj) = 0;
-    // todo: The following lines are actually correct, but setting Py_TYPE(type) = &JType_Type results in an interpreter crash. Why?
-    // This is still a problem because all the JType slots are actually never called (especially JType_getattro is
-    // needed to resolve unresolved JTypes and to recognize static field and methods access)
-    //Py_INCREF(&JType_Type);
-    //Py_TYPE(type) = &JType_Type;
-    //Py_SIZE(type) = sizeof (JPy_JType);
-
-    typeObj->tp_basicsize = isPrimitiveArray ? sizeof (JPy_JArray) : sizeof (JPy_JObj);
-    typeObj->tp_itemsize = 0;
-    typeObj->tp_base = type->superType != NULL ? (PyTypeObject*) type->superType : &JType_Type;
-    //typeObj->tp_base = (PyTypeObject*) type->superType;
-    typeObj->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE;
-    // If I uncomment the following line, I get (unpredictable) interpreter crashes
-    // (see also http://stackoverflow.com/questions/8066438/how-to-dynamically-create-a-derived-type-in-the-python-c-api)
-    //typeObj->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
-
-    #if PY_MAJOR_VERSION < 3
-    if (isPrimitiveArray) {
-        typeObj->tp_flags |= Py_TPFLAGS_HAVE_NEWBUFFER;
-    }
-    #endif
-
-    typeObj->tp_getattro = (getattrofunc) JObj_getattro;
-    typeObj->tp_setattro = (setattrofunc) JObj_setattro;
-
-    // Note: we may later want to add  <sequence> protocol to 'java.lang.String' and 'java.util.List' types.
-    // However, we cannot check directly against these global variable 'JPy_JString' and 'JPy_JList' here because
-    // the current function (JType_InitSlots) is called to compute the actual values for the global
-    // 'JPy_JString' and 'JPy_JList' variables!
-    // So we actually have to check against the Java Object types in order to create and assign slots for the
-    // Python protocols: java.lang.String --> sequence, java.util.Map --> dict, java.util.List --> list, java.util.Set --> set.
-
-
-    // If this type is an array type, add support for the <sequence> protocol
-    if (isArray) {
-        typeObj->tp_as_sequence = &JObj_as_sequence;
-    }
-
-    if (isPrimitiveArray) {
-        const char* componentTypeName = type->componentType->javaName;
-        if (strcmp(componentTypeName, "boolean") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_boolean;
-        } else if (strcmp(componentTypeName, "char") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_char;
-        } else if (strcmp(componentTypeName, "byte") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_byte;
-        } else if (strcmp(componentTypeName, "short") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_short;
-        } else if (strcmp(componentTypeName, "int") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_int;
-        } else if (strcmp(componentTypeName, "long") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_long;
-        } else if (strcmp(componentTypeName, "float") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_float;
-        } else if (strcmp(componentTypeName, "double") == 0) {
-            typeObj->tp_as_buffer = &JArray_as_buffer_double;
-        }
-    }
-
-    //printf("JType_InitSlots: typeObj->tp_as_buffer=%p\n", typeObj->tp_as_buffer);
-
-    typeObj->tp_alloc = PyType_GenericAlloc;
-    typeObj->tp_new = PyType_GenericNew;
-    typeObj->tp_init = (initproc) JObj_init;
-    typeObj->tp_richcompare = (richcmpfunc) JObj_richcompare;
-    typeObj->tp_hash = (hashfunc) JObj_hash;
-    typeObj->tp_repr = (reprfunc) JObj_repr;
-    typeObj->tp_str = (reprfunc) JObj_str;
-    typeObj->tp_dealloc = (destructor) JObj_dealloc;
-
-    // Check if we should set type.__module__ to the to the first part (up to the last dot) of the tp_name.
-    // See http://docs.python.org/3/c-api/exceptions.html?highlight=pyerr_newexception#PyErr_NewException
-
-    // Note that PyType_Ready() will set our typeObj->ob_type to &PyType_Type, while JType_New() created
-    // the typeObj with an typeObj->ob_type set to &JType_Type.
-    if (PyType_Ready(typeObj) < 0) {
-        JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JType_InitSlots: INTERNAL ERROR: PyType_Ready() failed\n");
-        return -1;
-    }
-
-    //printf("+++++++++++++++++++++++++++++++++++++++++ typeObj->ob_type=%p\n", ((PyObject*)typeObj)->ob_type);
-
-    JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JType_InitSlots: typeObj=%p, Py_TYPE(typeObj)=%p, typeObj->tp_name=\"%s\", typeObj->tp_base=%p, typeObj->tp_init=%p, &JType_Type=%p, &PyType_Type=%p, JObj_init=%p\n",
-                   typeObj, Py_TYPE(typeObj), typeObj->tp_name, typeObj->tp_base, typeObj->tp_init, &JType_Type, &PyType_Type, JObj_init);
-
-    return 0;
-}
-
-// This is only a good test as long JObj_init() is not used in other types
-#define JPY_IS_JTYPE(T)  (((PyTypeObject*) T)->tp_init == (initproc) JObj_init)
-
-
-int JObj_Check(PyObject* arg)
-{
-    return JPY_IS_JTYPE(Py_TYPE(arg));
-}
-
-int JType_Check(PyObject* arg)
-{
-    return PyType_Check(arg) && JPY_IS_JTYPE(arg);
-}
-
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#include "jpy_module.h"
+#include "jpy_diag.h"
+#include "jpy_jarray.h"
+#include "jpy_jtype.h"
+#include "jpy_jobj.h"
+#include "jpy_jmethod.h"
+#include "jpy_jfield.h"
+#include "jpy_conv.h"
+
+JPy_JObj* JObj_New(JNIEnv* jenv, jobject objectRef)
+{
+    jclass classRef;
+    JPy_JType* type;
+
+    classRef = (*jenv)->GetObjectClass(jenv, objectRef);
+    type = JType_GetType(jenv, classRef, JNI_TRUE);
+    (*jenv)->DeleteLocalRef(jenv, classRef);
+    if (type == NULL) {
+        return NULL;
+    }
+
+    return JObj_FromType(jenv, type, objectRef);
+}
+
+JPy_JObj* JObj_FromType(JNIEnv* jenv, JPy_JType* type, jobject objectRef)
+{
+    JPy_JObj* obj;
+
+    obj = (JPy_JObj*) PyObject_New(JPy_JObj, (PyTypeObject*) type);
+    if (obj == NULL) {
+        return NULL;
+    }
+
+    objectRef = (*jenv)->NewGlobalRef(jenv, objectRef);
+    if (objectRef == NULL) {
+        PyErr_NoMemory();
+        return NULL;
+    }
+
+    obj->objectRef = objectRef;
+
+    // For special treatment of primitive array refer to JType_InitSlots()
+    if (type->componentType != NULL && type->componentType->isPrimitive) {
+        JPy_JArray* array;
+
+        array = (JPy_JArray*) obj;
+        array->bufferExportCount = 0;
+    }
+
+    return obj;
+}
+
+/**
+ * The JObj type's tp_init slot. Called when the type is used to create new instances (constructor).
+ */
+int JObj_init(JPy_JObj* self, PyObject* args, PyObject* kwds)
+{
+    JNIEnv* jenv;
+    PyTypeObject* type;
+    JPy_JType* jType;
+    PyObject* constructor;
+    JPy_JMethod* jMethod;
+    jobject objectRef;
+    jvalue* jArgs;
+    JPy_ArgDisposer* jDisposers;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
+
+    type = ((PyObject*) self)->ob_type;
+
+    constructor = PyDict_GetItemString(type->tp_dict, JPy_JTYPE_ATTR_NAME_JINIT);
+    if (constructor == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "no constructor found (missing JType attribute '" JPy_JTYPE_ATTR_NAME_JINIT "')");
+        return -1;
+    }
+
+    if (!PyObject_TypeCheck(constructor, &JOverloadedMethod_Type)) {
+        PyErr_SetString(PyExc_RuntimeError, "invalid JType attribute '"  JPy_JTYPE_ATTR_NAME_JINIT  "': expected type JOverloadedMethod_Type");
+        return -1;
+    }
+
+    jType = (JPy_JType*) type;
+    if (jType->classRef == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "internal error: Java class reference is NULL");
+        return -1;
+    }
+
+    jMethod = JOverloadedMethod_FindMethod(jenv, (JPy_JOverloadedMethod*) constructor, args, JNI_FALSE);
+    if (jMethod == NULL) {
+        return -1;
+    }
+
+    if (JMethod_CreateJArgs(jenv, jMethod, args, &jArgs, &jDisposers) < 0) {
+        return -1;
+    }
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_init: calling Java constructor %s\n", jType->javaName);
+
+    objectRef = (*jenv)->NewObjectA(jenv, jType->classRef, jMethod->mid, jArgs);
+    JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+
+    if (objectRef == NULL) {
+        PyErr_NoMemory();
+        return -1;
+    }
+
+    if (jMethod->paramCount > 0) {
+        JMethod_DisposeJArgs(jenv, jMethod->paramCount, jArgs, jDisposers);
+    }
+
+    objectRef = (*jenv)->NewGlobalRef(jenv, objectRef);
+    if (objectRef == NULL) {
+        PyErr_NoMemory();
+        return -1;
+    }
+
+    // Note:  __init__ may be called multiple times, so we have to release the old objectRef
+    if (self->objectRef != NULL) {
+        (*jenv)->DeleteGlobalRef(jenv, self->objectRef);
+    }
+
+    self->objectRef = objectRef;
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_init: self->objectRef=%p\n", self->objectRef);
+
+    return 0;
+}
+
+/**
+ * The JObj type's tp_dealloc slot. Called when the reference count reaches zero.
+ */
+void JObj_dealloc(JPy_JObj* self)
+{
+    JNIEnv* jenv;
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_MEM, "JObj_dealloc: releasing instance of %s, self->objectRef=%p\n", Py_TYPE(self)->tp_name, self->objectRef);
+
+    jenv = JPy_GetJNIEnv();
+    if (jenv != NULL) {
+        if (self->objectRef != NULL) {
+            (*jenv)->DeleteGlobalRef(jenv, self->objectRef);
+        }
+    }
+
+    Py_TYPE(self)->tp_free((PyObject*) self);
+}
+
+int JObj_CompareTo(JNIEnv* jenv, JPy_JObj* obj1, JPy_JObj* obj2)
+{
+    jobject ref1;
+    jobject ref2;
+    int value;
+
+    ref1 = obj1->objectRef;
+    ref2 = obj2->objectRef;
+
+    if (ref1 == ref2 || (*jenv)->IsSameObject(jenv, ref1, ref2)) {
+        return 0;
+    } else if ((*jenv)->IsInstanceOf(jenv, ref1, JPy_Comparable_JClass)) {
+        value = (*jenv)->CallIntMethod(jenv, ref1, JPy_Comparable_CompareTo_MID, ref2);
+        (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
+    } else {
+        value = (char*) ref1 - (char*) ref2;
+    }
+
+    return (value == 0) ? 0 : (value < 0) ? -1 : +1;
+}
+
+int JObj_Equals(JNIEnv* jenv, JPy_JObj* obj1, JPy_JObj* obj2)
+{
+    jobject ref1;
+    jobject ref2;
+    int returnValue;
+
+    ref1 = obj1->objectRef;
+    ref2 = obj2->objectRef;
+
+    if ((*jenv)->IsSameObject(jenv, ref1, ref2)) {
+        returnValue = 1;
+    } else {
+        returnValue = (*jenv)->CallIntMethod(jenv, ref1, JPy_Object_Equals_MID, ref2);
+    }
+    (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
+    return returnValue;
+}
+
+/**
+ * The JObj type's tp_richcompare slot. Python: obj1 <opid> obj2
+ */
+PyObject* JObj_richcompare(PyObject* obj1, PyObject* obj2, int opid)
+{
+    JNIEnv* jenv;
+
+    if (!JObj_Check(obj1) || !JObj_Check(obj2)) {
+        Py_RETURN_FALSE;
+    }
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL);
+
+    if (opid == Py_LT) {
+        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value == -1) {
+            Py_RETURN_TRUE;
+        } else {
+            Py_RETURN_FALSE;
+        }
+    } else if (opid == Py_LE) {
+        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value == -1 || value == 0) {
+            Py_RETURN_TRUE;
+        } else {
+            Py_RETURN_FALSE;
+        }
+    } else if (opid == Py_GT) {
+        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value == +1) {
+            Py_RETURN_TRUE;
+        } else {
+            Py_RETURN_FALSE;
+        }
+    } else if (opid == Py_GE) {
+        int value = JObj_CompareTo(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value == +1 || value == 0) {
+            Py_RETURN_TRUE;
+        } else {
+            Py_RETURN_FALSE;
+        }
+    } else if (opid == Py_EQ) {
+        int value = JObj_Equals(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value) {
+            Py_RETURN_TRUE;
+        } else {
+            Py_RETURN_FALSE;
+        }
+    } else if (opid == Py_NE) {
+        int value = JObj_Equals(jenv, (JPy_JObj*) obj1, (JPy_JObj*) obj2);
+        if (value == -2) {
+            return NULL;
+        } else if (value) {
+            Py_RETURN_FALSE;
+        } else {
+            Py_RETURN_TRUE;
+        }
+    } else {
+        PyErr_SetString(PyExc_RuntimeError, "internal error: unrecognized opid");
+        return NULL;
+    }
+}
+
+/**
+ * The JObj type's tp_hash slot. Python: hash(obj)
+ */
+long JObj_hash(JPy_JObj* self)
+{
+    JNIEnv* jenv;
+    jenv = JPy_GetJNIEnv();
+    if (jenv != NULL) {
+        int returnValue = (*jenv)->CallIntMethod(jenv, self->objectRef, JPy_Object_HashCode_MID);
+        (*jenv)->ExceptionClear(jenv); // we can't deal with exceptions here, so clear any
+        return returnValue;
+    }
+    return -1;
+}
+
+
+/**
+ * The JObj type's tp_repr slot. Python: repr(obj))
+ */
+PyObject* JObj_repr(JPy_JObj* self)
+{
+    return JPy_FROM_FORMAT("%s(objectRef=%p)", Py_TYPE(self)->tp_name, self->objectRef);
+}
+
+/**
+ * The JObj type's tp_str slot. Calls Object.toString() on Java Objects. Python: str(obj)
+ */
+PyObject* JObj_str(JPy_JObj* self)
+{
+    JNIEnv* jenv;
+    jstring stringRef;
+    PyObject* returnValue;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
+
+    if (self->objectRef == NULL) {
+        return Py_BuildValue("");
+    }
+
+    returnValue = NULL;
+    stringRef = (*jenv)->CallObjectMethod(jenv, self->objectRef, JPy_Object_ToString_MID);
+    JPy_ON_JAVA_EXCEPTION_GOTO(error);
+    returnValue = JPy_FromJString(jenv, stringRef);
+
+error:
+    (*jenv)->DeleteLocalRef(jenv, stringRef);
+
+    return returnValue;
+}
+
+
+/**
+ * The JObj type's tp_setattro slot.
+ */
+int JObj_setattro(JPy_JObj* self, PyObject* name, PyObject* value)
+{
+    PyObject* oldValue;
+
+    //printf("JObj_setattro: %s.%s\n", Py_TYPE(self)->tp_name, JPy_AS_UTF8(name));
+
+    oldValue = PyObject_GenericGetAttr((PyObject*) self, name);
+    if (oldValue != NULL && PyObject_TypeCheck(oldValue, &JField_Type)) {
+        JNIEnv* jenv;
+        JPy_JField* field;
+        JPy_JType* type;
+
+        field = (JPy_JField*) oldValue;
+        type = field->type;
+
+        JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
+
+        if (type == JPy_JBoolean) {
+            jboolean item = JPy_AS_JBOOLEAN(value);
+            (*jenv)->SetBooleanField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JChar) {
+            jchar item = JPy_AS_JCHAR(value);
+            (*jenv)->SetCharField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JByte) {
+            jbyte item = JPy_AS_JBYTE(value);
+            (*jenv)->SetByteField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JShort) {
+            jshort item = JPy_AS_JSHORT(value);
+            (*jenv)->SetShortField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JInt) {
+            jint item = JPy_AS_JINT(value);
+            (*jenv)->SetIntField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JLong) {
+            jlong item = JPy_AS_JLONG(value);
+            (*jenv)->SetLongField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JFloat) {
+            jfloat item = JPy_AS_JFLOAT(value);
+            (*jenv)->SetFloatField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else if (type == JPy_JDouble) {
+            jdouble item = JPy_AS_JDOUBLE(value);
+            (*jenv)->SetDoubleField(jenv, self->objectRef, field->fid, item);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        } else {
+            jobject objectRef;
+            if (JPy_AsJObjectWithType(jenv, value, &objectRef, field->type) < 0) {
+                return -1;
+            }
+            (*jenv)->SetObjectField(jenv, self->objectRef, field->fid, objectRef);
+            JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+        }
+        return 0;
+    } else {
+        return PyObject_GenericSetAttr((PyObject*) self, name, value);
+    }
+}
+
+/**
+ * The JObj type's tp_getattro slot.
+ * This is important: wrap callable objects of type JOverloadedMethod_Type into python methods so that
+ * a method call to an instance x of class X becomes: x.m() --> X.m(x)
+ */
+PyObject* JObj_getattro(JPy_JObj* self, PyObject* name)
+{
+    JPy_JType* selfType;
+    PyObject* value;
+
+    //printf("JObj_getattro: %s.%s\n", Py_TYPE(self)->tp_name, JPy_AS_UTF8(name));
+
+    // First make sure that the Java type is resolved, otherwise we won't find any methods at all.
+    selfType = (JPy_JType*) Py_TYPE(self);
+    if (!selfType->isResolved) {
+        JNIEnv* jenv;
+        JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
+        if (JType_ResolveType(jenv, selfType) < 0) {
+            return NULL;
+        }
+    }
+
+    // todo: implement a special lookup: we need to override __getattro__ of JType (--> JType_getattro) as well so that we know if a method
+    // is called on a class rather than on an instance. Using PyObject_GenericGetAttr will also call  JType_getattro,
+    // but then we loose the information that a method is called on an instance and not on a class.
+    value = PyObject_GenericGetAttr((PyObject*) self, name);
+    if (value == NULL) {
+        //printf("JObj_getattro: not found!\n");
+        return NULL;
+    }
+    if (PyObject_TypeCheck(value, &JOverloadedMethod_Type)) {
+        //JPy_JOverloadedMethod* overloadedMethod = (JPy_JOverloadedMethod*) value;
+        //printf("JObj_getattro: wrapping JOverloadedMethod, overloadCount=%d\n", PyList_Size(overloadedMethod->methodList));
+#if defined(JPY_COMPAT_33P)
+        return PyMethod_New(value, (PyObject*) self);
+#elif defined(JPY_COMPAT_27)
+        // todo: py27: 3rd arg must be class of self, check if NULL is ok here
+        return PyMethod_New(value, (PyObject*) self, NULL);
+#else
+#error JPY_VERSION_ERROR
+#endif
+    } else if (PyObject_TypeCheck(value, &JField_Type)) {
+        JNIEnv* jenv;
+        JPy_JField* field;
+        JPy_JType* type;
+
+        field = (JPy_JField*) value;
+        type = field->type;
+
+        JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
+
+        if (type == JPy_JBoolean) {
+            jboolean item = (*jenv)->GetBooleanField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JBOOLEAN(item);
+        } else if (type == JPy_JChar) {
+            jchar item = (*jenv)->GetCharField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JCHAR(item);
+        } else if (type == JPy_JByte) {
+            jbyte item = (*jenv)->GetByteField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JBYTE(item);
+        } else if (type == JPy_JShort) {
+            jshort item = (*jenv)->GetShortField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JSHORT(item);
+        } else if (type == JPy_JInt) {
+            jint item = (*jenv)->GetIntField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JINT(item);
+        } else if (type == JPy_JLong) {
+            jlong item = (*jenv)->GetLongField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JLONG(item);
+        } else if (type == JPy_JFloat) {
+            jfloat item = (*jenv)->GetFloatField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JFLOAT(item);
+        } else if (type == JPy_JDouble) {
+            jdouble item = (*jenv)->GetDoubleField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            return JPy_FROM_JDOUBLE(item);
+        } else {
+            PyObject* returnValue;
+            jobject item = (*jenv)->GetObjectField(jenv, self->objectRef, field->fid);
+            JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+            returnValue = JPy_FromJObjectWithType(jenv, item, field->type);
+            (*jenv)->DeleteLocalRef(jenv, item);
+            return returnValue;
+        }
+    } else {
+        //printf("JObj_getattro: passing through\n");
+    }
+    return value;
+}
+
+/**
+ * The JObj type's sq_length field of the tp_as_sequence slot. Called if len(obj) is called.
+ * Only used for array types (type->componentType != NULL).
+ */
+Py_ssize_t JObj_sq_length(JPy_JObj* self)
+{
+    JNIEnv* jenv;
+    jsize length;
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
+    length = (*jenv)->GetArrayLength(jenv, self->objectRef);
+    //printf("JObj_sq_length: length=%d\n", length);
+    return (Py_ssize_t) length;
+}
+
+/*
+ * The JObj type's sq_item field of the tp_as_sequence slot. Called if 'item = obj[index]' is used.
+ * Only used for array types (type->componentType != NULL).
+ */
+PyObject* JObj_sq_item(JPy_JObj* self, Py_ssize_t index)
+{
+    JNIEnv* jenv;
+    JPy_JType* type;
+    JPy_JType* componentType;
+    jsize length;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, NULL)
+
+    //printf("JObj_sq_item: index=%d\n", index);
+
+    type = (JPy_JType*) Py_TYPE(self);
+    componentType = type->componentType;
+    if (componentType == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "internal error: object is not an array");
+        return NULL;
+    }
+
+    // This is annoying and slow in Python 3.3.2: We must have this check, in order to raise an PyExc_IndexError,
+    // otherwise Python functions such as list(jarr) will not succeed.
+    // Tis is really strange, because n = sq_length() will be called and subsequent sq_item(index=0 ... n) calls will be done.
+    length = (*jenv)->GetArrayLength(jenv, self->objectRef);
+    if (index < 0 || index >= length) {
+        PyErr_SetString(PyExc_IndexError, "Java array index out of bounds");
+        return NULL;
+    }
+
+    if (componentType == JPy_JBoolean) {
+        jboolean item;
+        (*jenv)->GetBooleanArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JBOOLEAN(item);
+    } else if (componentType == JPy_JChar) {
+        jchar item;
+        (*jenv)->GetCharArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JCHAR(item);
+    } else if (componentType == JPy_JByte) {
+        jbyte item;
+        (*jenv)->GetByteArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JBYTE(item);
+    } else if (componentType == JPy_JShort) {
+        jshort item;
+        (*jenv)->GetShortArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JSHORT(item);
+    } else if (componentType == JPy_JInt) {
+        jint item;
+        (*jenv)->GetIntArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JINT(item);
+    } else if (componentType == JPy_JLong) {
+        jlong item;
+        (*jenv)->GetLongArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JLONG(item);
+    } else if (componentType == JPy_JFloat) {
+        jfloat item;
+        (*jenv)->GetFloatArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JFLOAT(item);
+    } else if (componentType == JPy_JDouble) {
+        jdouble item;
+        (*jenv)->GetDoubleArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        return JPy_FROM_JDOUBLE(item);
+    } else {
+        PyObject* returnValue;
+        jobject item = (*jenv)->GetObjectArrayElement(jenv, self->objectRef, (jsize) index);
+        JPy_ON_JAVA_EXCEPTION_RETURN(NULL);
+        returnValue = JPy_FromJObjectWithType(jenv, item, type->componentType);
+        (*jenv)->DeleteLocalRef(jenv, item);
+        return returnValue;
+    }
+}
+
+/*
+ * The JObj type's sq_ass_item field of the tp_as_sequence slot. Called if 'obj[index] = item' is used.
+ * Only used for array types (type->componentType != NULL).
+ */
+int JObj_sq_ass_item(JPy_JObj* self, Py_ssize_t index, PyObject* pyItem)
+{
+    JNIEnv* jenv;
+    JPy_JType* type;
+    JPy_JType* componentType;
+
+    JPy_GET_JNI_ENV_OR_RETURN(jenv, -1)
+
+    type = (JPy_JType*) Py_TYPE(self);
+    componentType = type->componentType;
+    if (type->componentType == NULL) {
+        PyErr_SetString(PyExc_RuntimeError, "internal error: object is not an array");
+        return -1;
+    }
+
+    // Note: the following item assignments are not value range checked
+    if (componentType == JPy_JBoolean) {
+        jboolean item = JPy_AS_JBOOLEAN(pyItem);
+        (*jenv)->SetBooleanArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JChar) {
+        jchar item = JPy_AS_JCHAR(pyItem);
+        (*jenv)->SetCharArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JByte) {
+        jbyte item = JPy_AS_JBYTE(pyItem);
+        (*jenv)->SetByteArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JShort) {
+        jshort item = JPy_AS_JSHORT(pyItem);
+        (*jenv)->SetShortArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JInt) {
+        jint item = JPy_AS_JINT(pyItem);
+        (*jenv)->SetIntArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JLong) {
+        jlong item = JPy_AS_JLONG(pyItem);
+        (*jenv)->SetLongArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JFloat) {
+        jfloat item = JPy_AS_JFLOAT(pyItem);
+        (*jenv)->SetFloatArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else if (componentType == JPy_JDouble) {
+        jdouble item = JPy_AS_JDOUBLE(pyItem);
+        (*jenv)->SetDoubleArrayRegion(jenv, self->objectRef, (jsize) index, 1, &item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    } else {
+        jobject item;
+        if (JPy_AsJObjectWithType(jenv, pyItem, &item, type->componentType) < 0) {
+            return -1;
+        }
+        (*jenv)->SetObjectArrayElement(jenv, self->objectRef, (jsize) index, item);
+        JPy_ON_JAVA_EXCEPTION_RETURN(-1);
+    }
+    return 0;
+}
+
+/**
+ * The JObj type's tp_as_sequence slot.
+ * Implements the <sequence> interface for array types (type->componentType != NULL).
+ */
+static PySequenceMethods JObj_as_sequence = {
+    (lenfunc) JObj_sq_length,            /* sq_length */
+    NULL,   /* sq_concat */
+    NULL,   /* sq_repeat */
+    (ssizeargfunc) JObj_sq_item,         /* sq_item */
+    NULL,   /* was_sq_slice */
+    (ssizeobjargproc) JObj_sq_ass_item,  /* sq_ass_item */
+    NULL,   /* was_sq_ass_slice */
+    NULL,   /* sq_contains */
+    NULL,   /* sq_inplace_concat */
+    NULL,   /* sq_inplace_repeat */
+};
+
+
+int JType_InitSlots(JPy_JType* type)
+{
+    PyTypeObject* typeObj;
+    jboolean isArray;
+    jboolean isPrimitiveArray;
+
+    isArray = type->componentType != NULL;
+    isPrimitiveArray = isArray && type->componentType->isPrimitive;
+
+    typeObj = (PyTypeObject*) type;
+
+    Py_REFCNT(typeObj) = 1;
+    Py_TYPE(typeObj) = NULL;
+    Py_SIZE(typeObj) = 0;
+    // todo: The following lines are actually correct, but setting Py_TYPE(type) = &JType_Type results in an interpreter crash. Why?
+    // This is still a problem because all the JType slots are actually never called (especially JType_getattro is
+    // needed to resolve unresolved JTypes and to recognize static field and methods access)
+    //Py_INCREF(&JType_Type);
+    //Py_TYPE(type) = &JType_Type;
+    //Py_SIZE(type) = sizeof (JPy_JType);
+
+    typeObj->tp_basicsize = isPrimitiveArray ? sizeof (JPy_JArray) : sizeof (JPy_JObj);
+    typeObj->tp_itemsize = 0;
+    typeObj->tp_base = type->superType != NULL ? (PyTypeObject*) type->superType : &JType_Type;
+    //typeObj->tp_base = (PyTypeObject*) type->superType;
+    typeObj->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE;
+    // If I uncomment the following line, I get (unpredictable) interpreter crashes
+    // (see also http://stackoverflow.com/questions/8066438/how-to-dynamically-create-a-derived-type-in-the-python-c-api)
+    //typeObj->tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE | Py_TPFLAGS_HEAPTYPE;
+
+    #if defined(JPY_COMPAT_27)
+    if (isPrimitiveArray) {
+        typeObj->tp_flags |= Py_TPFLAGS_HAVE_NEWBUFFER;
+    }
+    #endif
+
+    typeObj->tp_getattro = (getattrofunc) JObj_getattro;
+    typeObj->tp_setattro = (setattrofunc) JObj_setattro;
+
+    // Note: we may later want to add  <sequence> protocol to 'java.lang.String' and 'java.util.List' types.
+    // However, we cannot check directly against these global variable 'JPy_JString' and 'JPy_JList' here because
+    // the current function (JType_InitSlots) is called to compute the actual values for the global
+    // 'JPy_JString' and 'JPy_JList' variables!
+    // So we actually have to check against the Java Object types in order to create and assign slots for the
+    // Python protocols: java.lang.String --> sequence, java.util.Map --> dict, java.util.List --> list, java.util.Set --> set.
+
+
+    // If this type is an array type, add support for the <sequence> protocol
+    if (isArray) {
+        typeObj->tp_as_sequence = &JObj_as_sequence;
+    }
+
+    if (isPrimitiveArray) {
+        const char* componentTypeName = type->componentType->javaName;
+        if (strcmp(componentTypeName, "boolean") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_boolean;
+        } else if (strcmp(componentTypeName, "char") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_char;
+        } else if (strcmp(componentTypeName, "byte") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_byte;
+        } else if (strcmp(componentTypeName, "short") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_short;
+        } else if (strcmp(componentTypeName, "int") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_int;
+        } else if (strcmp(componentTypeName, "long") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_long;
+        } else if (strcmp(componentTypeName, "float") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_float;
+        } else if (strcmp(componentTypeName, "double") == 0) {
+            typeObj->tp_as_buffer = &JArray_as_buffer_double;
+        }
+    }
+
+    //printf("JType_InitSlots: typeObj->tp_as_buffer=%p\n", typeObj->tp_as_buffer);
+
+    typeObj->tp_alloc = PyType_GenericAlloc;
+    typeObj->tp_new = PyType_GenericNew;
+    typeObj->tp_init = (initproc) JObj_init;
+    typeObj->tp_richcompare = (richcmpfunc) JObj_richcompare;
+    typeObj->tp_hash = (hashfunc) JObj_hash;
+    typeObj->tp_repr = (reprfunc) JObj_repr;
+    typeObj->tp_str = (reprfunc) JObj_str;
+    typeObj->tp_dealloc = (destructor) JObj_dealloc;
+
+    // Check if we should set type.__module__ to the to the first part (up to the last dot) of the tp_name.
+    // See http://docs.python.org/3/c-api/exceptions.html?highlight=pyerr_newexception#PyErr_NewException
+
+    // Note that PyType_Ready() will set our typeObj->ob_type to &PyType_Type, while JType_New() created
+    // the typeObj with an typeObj->ob_type set to &JType_Type.
+    if (PyType_Ready(typeObj) < 0) {
+        JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JType_InitSlots: INTERNAL ERROR: PyType_Ready() failed\n");
+        return -1;
+    }
+
+    //printf("+++++++++++++++++++++++++++++++++++++++++ typeObj->ob_type=%p\n", ((PyObject*)typeObj)->ob_type);
+
+    JPy_DIAG_PRINT(JPy_DIAG_F_TYPE, "JType_InitSlots: typeObj=%p, Py_TYPE(typeObj)=%p, typeObj->tp_name=\"%s\", typeObj->tp_base=%p, typeObj->tp_init=%p, &JType_Type=%p, &PyType_Type=%p, JObj_init=%p\n",
+                   typeObj, Py_TYPE(typeObj), typeObj->tp_name, typeObj->tp_base, typeObj->tp_init, &JType_Type, &PyType_Type, JObj_init);
+
+    return 0;
+}
+
+// This is only a good test as long JObj_init() is not used in other types
+#define JPY_IS_JTYPE(T)  (((PyTypeObject*) T)->tp_init == (initproc) JObj_init)
+
+
+int JObj_Check(PyObject* arg)
+{
+    return JPY_IS_JTYPE(Py_TYPE(arg));
+}
+
+int JType_Check(PyObject* arg)
+{
+    return PyType_Check(arg) && JPY_IS_JTYPE(arg);
+}
+
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jobj.h` & `jpy-0.7.5/src/main/c/jpy_jobj.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,46 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_JOBJ_H
-#define JPY_JOBJ_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-///////////////////////////////////////////////////////////////////////////////////////////////////////////////////////
-// JClass
-
-/**
- * The Java Object representation in Python.
- * @see JPy_JArray
- */
-typedef struct JPy_JObj
-{
-    PyObject_HEAD
-    jobject objectRef;
-}
-JPy_JObj;
-
-
-int JObj_Check(PyObject* arg);
-
-JPy_JObj* JObj_New(JNIEnv* jenv, jobject objectRef);
-JPy_JObj* JObj_FromType(JNIEnv* jenv, JPy_JType* type, jobject objectRef);
-
-int JObj_InitTypeSlots(PyTypeObject* type, const char* typeName, PyTypeObject* superType);
-
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_JOBJ_H
+#define JPY_JOBJ_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+/**
+ * The Java Object representation in Python.
+ * @see JPy_JArray
+ */
+typedef struct JPy_JObj
+{
+    PyObject_HEAD
+    jobject objectRef;
+}
+JPy_JObj;
+
+
+int JObj_Check(PyObject* arg);
+
+JPy_JObj* JObj_New(JNIEnv* jenv, jobject objectRef);
+JPy_JObj* JObj_FromType(JNIEnv* jenv, JPy_JType* type, jobject objectRef);
+
+int JObj_InitTypeSlots(PyTypeObject* type, const char* typeName, PyTypeObject* superType);
+
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
 #endif /* !JPY_JOBJ_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_jtype.c` & `jpy-0.7.5/src/main/c/jpy_jtype.c`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/c/jpy_jtype.h` & `jpy-0.7.5/src/main/c/jpy_jtype.h`

 * *Files 16% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_JTYPE_H
-#define JPY_JTYPE_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-
-
-/**
- * The Python type 'JType' representing a Java type.
- */
-typedef struct JPy_JType
-{
-    // Since this is a type object, inherit everything from from PyTypeObject.
-    // It is absolutely essential that this is the first struct member!
-    // typeObj.tp_name is this type's fully qualified Java name (same as 'javaName field').
-    PyTypeObject typeObj;
-    // The Java type name.
-    char* javaName;
-    // The JNI class reference (global reference).
-    jclass classRef;
-    // The super type of this type. This will be NULL for primitive types, 'void' and 'java.lang.Object'.
-    struct JPy_JType* superType;
-    // If component type of this type if this type is an array, NULL otherwise.
-    struct JPy_JType* componentType;
-    // If TRUE, 'classRef' refers to a primitive type (or 'void').
-    char isPrimitive;
-    // If TRUE, the type is currently being resolved.
-    char isResolving;
-    // If TRUE, all the class constructors and methods have already been resolved.
-    char isResolved;
-}
-JPy_JType;
-
-/**
- * The 'JType' singleton.
- */
-extern PyTypeObject JType_Type;
-
-typedef void (*JPy_DisposeArg)(JNIEnv*, jvalue* value, void* data);
-
-/**
- * ArgDisposers are used to dispose arguments after invocation of Java methods.
- * We need to dispose those arguments which have been created as local references,
- * e.g. jenv->NewString(), jenv->NewObjectArray(), jenv->New<Type>Array().
- */
-typedef struct JPy_ArgDisposer
-{
-    void* data;
-    JPy_DisposeArg DisposeArg;
-}
-JPy_ArgDisposer;
-
-
-struct JPy_ParamDescriptor;
-
-typedef int (*JPy_MatchPyArg)(JNIEnv*, struct JPy_ParamDescriptor*, PyObject*);
-typedef int (*JPy_ConvertPyArg)(JNIEnv*, struct JPy_ParamDescriptor*, PyObject*, jvalue*, JPy_ArgDisposer*);
-
-/**
- * Method return value descriptor.
- */
-typedef struct JPy_ReturnDescriptor
-{
-    /**
-     * The return type.
-     */
-    JPy_JType* type;
-    /**
-     * If JPy_ParamDescriptor.isReturnIndex == TRUE the index of the parameter, whose argument will serve as return value.
-     * If JPy_ParamDescriptor.isReturnIndex == FALSE it will be -1.
-     */
-    jint paramIndex;
-}
-JPy_ReturnDescriptor;
-
-/**
- * Method parameter descriptor.
- */
-typedef struct JPy_ParamDescriptor
-{
-    JPy_JType* type;
-    jboolean isMutable;
-    jboolean isOutput;
-    jboolean isReturn;
-    JPy_MatchPyArg MatchPyArg;
-    JPy_ConvertPyArg ConvertPyArg;
-}
-JPy_ParamDescriptor;
-
-
-int JType_Check(PyObject* obj);
-
-JPy_JType* JType_GetTypeForObject(JNIEnv* jenv, jobject objectRef);
-JPy_JType* JType_GetTypeForName(JNIEnv* jenv, const char* typeName, jboolean resolve);
-JPy_JType* JType_GetType(JNIEnv* jenv, jclass classRef, jboolean resolve);
-
-PyObject* JType_ConvertJavaToPythonObject(JNIEnv* jenv, JPy_JType* type, jobject objectRef);
-int       JType_ConvertPythonToJavaObject(JNIEnv* jenv, JPy_JType* type, PyObject* arg, jobject* objectRef);
-
-PyObject* JType_GetOverloadedMethod(JNIEnv* jenv, JPy_JType* type, PyObject* methodName, jboolean useSuperClass);
-
-int JType_CreateJavaArray(JNIEnv* jenv, JPy_JType* componentType, PyObject* pyArg, jobject* objectRef);
-
-// Non-API. Defined in jpy_jobj.c
-int JType_InitSlots(JPy_JType* type);
-// Non-API. Defined in jpy_jtype.c
-int JType_ResolveType(JNIEnv* jenv, JPy_JType* type);
-
-#ifdef __cplusplus
-}  /* extern "C" */
-#endif
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_JTYPE_H
+#define JPY_JTYPE_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include "jpy_compat.h"
+
+/**
+ * The Python type 'JType' representing a Java type.
+ */
+typedef struct JPy_JType
+{
+    // Since this is a type object, inherit everything from from PyTypeObject.
+    // It is absolutely essential that this is the first struct member!
+    // typeObj.tp_name is this type's fully qualified Java name (same as 'javaName field').
+    PyTypeObject typeObj;
+    // The Java type name.
+    char* javaName;
+    // The JNI class reference (global reference).
+    jclass classRef;
+    // The super type of this type. This will be NULL for primitive types, 'void' and 'java.lang.Object'.
+    struct JPy_JType* superType;
+    // If component type of this type if this type is an array, NULL otherwise.
+    struct JPy_JType* componentType;
+    // If TRUE, 'classRef' refers to a primitive type (or 'void').
+    char isPrimitive;
+    // If TRUE, the type is currently being resolved.
+    char isResolving;
+    // If TRUE, all the class constructors and methods have already been resolved.
+    char isResolved;
+}
+JPy_JType;
+
+/**
+ * The 'JType' singleton.
+ */
+extern PyTypeObject JType_Type;
+
+typedef void (*JPy_DisposeArg)(JNIEnv*, jvalue* value, void* data);
+
+/**
+ * ArgDisposers are used to dispose arguments after invocation of Java methods.
+ * We need to dispose those arguments which have been created as local references,
+ * e.g. jenv->NewString(), jenv->NewObjectArray(), jenv->New<Type>Array().
+ */
+typedef struct JPy_ArgDisposer
+{
+    void* data;
+    JPy_DisposeArg DisposeArg;
+}
+JPy_ArgDisposer;
+
+
+struct JPy_ParamDescriptor;
+
+typedef int (*JPy_MatchPyArg)(JNIEnv*, struct JPy_ParamDescriptor*, PyObject*);
+typedef int (*JPy_ConvertPyArg)(JNIEnv*, struct JPy_ParamDescriptor*, PyObject*, jvalue*, JPy_ArgDisposer*);
+
+/**
+ * Method return value descriptor.
+ */
+typedef struct JPy_ReturnDescriptor
+{
+    /**
+     * The return type.
+     */
+    JPy_JType* type;
+    /**
+     * If JPy_ParamDescriptor.isReturnIndex == TRUE the index of the parameter, whose argument will serve as return value.
+     * If JPy_ParamDescriptor.isReturnIndex == FALSE it will be -1.
+     */
+    jint paramIndex;
+}
+JPy_ReturnDescriptor;
+
+/**
+ * Method parameter descriptor.
+ */
+typedef struct JPy_ParamDescriptor
+{
+    JPy_JType* type;
+    jboolean isMutable;
+    jboolean isOutput;
+    jboolean isReturn;
+    JPy_MatchPyArg MatchPyArg;
+    JPy_ConvertPyArg ConvertPyArg;
+}
+JPy_ParamDescriptor;
+
+
+int JType_Check(PyObject* obj);
+
+JPy_JType* JType_GetTypeForObject(JNIEnv* jenv, jobject objectRef);
+JPy_JType* JType_GetTypeForName(JNIEnv* jenv, const char* typeName, jboolean resolve);
+JPy_JType* JType_GetType(JNIEnv* jenv, jclass classRef, jboolean resolve);
+
+PyObject* JType_ConvertJavaToPythonObject(JNIEnv* jenv, JPy_JType* type, jobject objectRef);
+int       JType_ConvertPythonToJavaObject(JNIEnv* jenv, JPy_JType* type, PyObject* arg, jobject* objectRef);
+
+PyObject* JType_GetOverloadedMethod(JNIEnv* jenv, JPy_JType* type, PyObject* methodName, jboolean useSuperClass);
+
+int JType_CreateJavaArray(JNIEnv* jenv, JPy_JType* componentType, PyObject* pyArg, jobject* objectRef);
+
+// Non-API. Defined in jpy_jobj.c
+int JType_InitSlots(JPy_JType* type);
+// Non-API. Defined in jpy_jtype.c
+int JType_ResolveType(JNIEnv* jenv, JPy_JType* type);
+
+#ifdef __cplusplus
+}  /* extern "C" */
+#endif
 #endif /* !JPY_JTYPE_H */
```

## Comparing `jpy-0.7.4/src/main/c/jpy_module.c` & `jpy-0.7.5/src/main/c/jpy_module.c`

 * *Files 1% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 };
 
 void JPy_free(void* unused);
 
 #define JPY_MODULE_NAME "jpy"
 #define JPY_MODULE_DOC  "Bi-directional Python-Java Bridge"
 
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
 static struct PyModuleDef JPy_ModuleDef =
 {
     PyModuleDef_HEAD_INIT,
     JPY_MODULE_NAME,   /* Name of the Python JPy_Module */
     JPY_MODULE_DOC,    /* Module documentation */
     -1,                /* Size of per-interpreter state of the JPy_Module, or -1 if the JPy_Module keeps state in global variables. */
     JPy_Functions,     /* Structure containing global jpy-functions */
@@ -229,41 +229,45 @@
     } else {
         JPy_DIAG_PRINT(JPy_DIAG_F_JVM + JPy_DIAG_F_ERR, "JPy_GetJNIEnv: Received unhandled status code from JVM GetEnv(): status=%d\n", status);
     }
 
     return jenv;
 }
 
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
 #define JPY_RETURN(V) return V
 #define JPY_MODULE_INIT_FUNC PyInit_jpy
-#else
+#elif defined(JPY_COMPAT_27)
 #define JPY_RETURN(V) return
 #define JPY_MODULE_INIT_FUNC initjpy
+#else
+#error JPY_VERSION_ERROR
 #endif
 
 /**
  * Called by the Python interpreter's import machinery, e.g. using 'import jpy'.
  */
 PyMODINIT_FUNC JPY_MODULE_INIT_FUNC(void)
 {
     //printf("PyInit_jpy: JPy_JVM=%p\n", JPy_JVM);
 
     /////////////////////////////////////////////////////////////////////////
 
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
     JPy_Module = PyModule_Create(&JPy_ModuleDef);
     if (JPy_Module == NULL) {
         JPY_RETURN(NULL);
     }
-#else
+#elif defined(JPY_COMPAT_27)
     JPy_Module = Py_InitModule3(JPY_MODULE_NAME, JPy_Functions, JPY_MODULE_DOC);
     if (JPy_Module == NULL) {
         JPY_RETURN(NULL);
     }
+#else
+    #error JPY_VERSION_ERROR
 #endif
 
     /////////////////////////////////////////////////////////////////////////
 
     if (PyType_Ready(&JType_Type) < 0) {
         JPY_RETURN(NULL);
     }
```

## Comparing `jpy-0.7.4/src/main/c/jpy_module.h` & `jpy-0.7.5/src/main/c/jpy_module.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,185 +1,187 @@
-/*
- * Copyright (C) 2014 Brockmann Consult GmbH
- *
- * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
- * General Public License as published by the Free Software Foundation; either version 3 of the License,
- * or (at your option) any later version. This program is distributed in the hope that it will be useful,
- * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
- * PARTICULAR PURPOSE. See the GNU General Public License for more details.
- *
- * You should have received a copy of the GNU General Public License along with this program; if not, see
- * http://www.gnu.org/licenses/
- */
-
-#ifndef JPY_MODULE_H
-#define JPY_MODULE_H
-
-#ifdef __cplusplus
-extern "C" {
-#endif
-
-#include <Python.h>
-#include <structmember.h>
-#include <jni.h>
-
-#define JPY_JNI_VERSION JNI_VERSION_1_6
-
-extern PyObject* JPy_Module;
-extern PyObject* JPy_Types;
-extern PyObject* JPy_Type_Callbacks;
-extern PyObject* JException_Type;
-
-extern JavaVM* JPy_JVM;
-extern jboolean JPy_MustDestroyJVM;
-
-
-#define JPy_JTYPE_ATTR_NAME_JINIT "__jinit__"
-
-#define JPy_MODULE_ATTR_NAME_TYPES "types"
-#define JPy_MODULE_ATTR_NAME_TYPE_CALLBACKS "type_callbacks"
-
-
-/**
- * Gets the current JNI environment pointer.
- * Returns NULL, if the JVM is down.
- *
- * General jpy design guideline: Use the JPy_GetJNIEnv function only in entry points from Python calls into C.
- * Add a JNIEnv* as first parameter to all functions that require it.
- */
-JNIEnv* JPy_GetJNIEnv(void);
-
-int JPy_InitGlobalVars(JNIEnv* jenv);
-void JPy_ClearGlobalVars(JNIEnv* jenv);
-
-/**
- * Gets the current JNI environment pointer JENV. If this is NULL, it returns the given RET_VALUE.
- * Warning: This method may immediately return, so make sure there will be no memory leaks in this case.
- *
- * General jpy design guideline: Use the JPy_GET_JNI_ENV_OR_RETURN macro only in entry points from Python calls into C.
- * Add a JNIEnv* as first parameter to all functions that require it.
- */
-#define JPy_GET_JNI_ENV_OR_RETURN(JENV, RET_VALUE) \
-    if ((JENV = JPy_GetJNIEnv()) == NULL) { \
-        return (RET_VALUE); \
-    } else { \
-    }
-
-
-/**
- * Fetches the last Java exception occurred and raises a new Python exception.
- */
-void JPy_HandleJavaException(JNIEnv* jenv);
-
-
-#define JPy_ON_JAVA_EXCEPTION_GOTO(LABEL) \
-    if ((*jenv)->ExceptionCheck(jenv)) { \
-        JPy_HandleJavaException(jenv); \
-        goto LABEL; \
-    }
-
-#define JPy_ON_JAVA_EXCEPTION_RETURN(VALUE) \
-    if ((*jenv)->ExceptionCheck(jenv)) { \
-        JPy_HandleJavaException(jenv); \
-        return VALUE; \
-    }
-
-
-struct JPy_JType;
-
-extern struct JPy_JType* JPy_JBoolean;
-extern struct JPy_JType* JPy_JChar;
-extern struct JPy_JType* JPy_JByte;
-extern struct JPy_JType* JPy_JShort;
-extern struct JPy_JType* JPy_JInt;
-extern struct JPy_JType* JPy_JLong;
-extern struct JPy_JType* JPy_JFloat;
-extern struct JPy_JType* JPy_JDouble;
-extern struct JPy_JType* JPy_JVoid;
-extern struct JPy_JType* JPy_JBooleanObj;
-extern struct JPy_JType* JPy_JCharacterObj;
-extern struct JPy_JType* JPy_JByteObj;
-extern struct JPy_JType* JPy_JShortObj;
-extern struct JPy_JType* JPy_JIntegerObj;
-extern struct JPy_JType* JPy_JLongObj;
-extern struct JPy_JType* JPy_JFloatObj;
-extern struct JPy_JType* JPy_JDoubleObj;
-extern struct JPy_JType* JPy_JObject;
-extern struct JPy_JType* JPy_JString;
-extern struct JPy_JType* JPy_JPyObject;
-extern struct JPy_JType* JPy_JPyModule;
-
-// java.lang.Comparable
-extern jclass JPy_Comparable_JClass;
-extern jmethodID JPy_Comparable_CompareTo_MID;
-// java.lang.Object
-extern jclass JPy_Object_JClass;
-extern jmethodID JPy_Object_ToString_MID;
-extern jmethodID JPy_Object_HashCode_MID;
-extern jmethodID JPy_Object_Equals_MID;
-// java.lang.Class
-extern jclass JPy_Class_JClass;
-extern jmethodID JPy_Class_GetName_MID;
-extern jmethodID JPy_Class_GetDeclaredConstructors_MID;
-extern jmethodID JPy_Class_GetDeclaredFields_MID;
-extern jmethodID JPy_Class_GetDeclaredMethods_MID;
-extern jmethodID JPy_Class_GetComponentType_MID;
-extern jmethodID JPy_Class_IsPrimitive_MID;
-// java.lang.reflect.Constructor
-extern jclass JPy_Constructor_JClass;
-extern jmethodID JPy_Constructor_GetModifiers_MID;
-extern jmethodID JPy_Constructor_GetParameterTypes_MID;
-// java.lang.reflect.Method
-extern jclass JPy_Method_JClass;
-extern jmethodID JPy_Method_GetName_MID;
-extern jmethodID JPy_Method_GetModifiers_MID;
-extern jmethodID JPy_Method_GetParameterTypes_MID;
-extern jmethodID JPy_Method_GetReturnType_MID;
-// java.lang.reflect.Field
-extern jclass JPy_Field_JClass;
-extern jmethodID JPy_Field_GetName_MID;
-extern jmethodID JPy_Field_GetModifiers_MID;
-extern jmethodID JPy_Field_GetType_MID;
-
-extern jclass JPy_RuntimeException_JClass;
-
-extern jclass JPy_Boolean_JClass;
-extern jmethodID JPy_Boolean_Init_MID;
-extern jmethodID JPy_Boolean_BooleanValue_MID;
-
-extern jclass JPy_Character_JClass;
-extern jmethodID JPy_Character_Init_MID;
-extern jmethodID JPy_Character_CharValue_MID;
-
-extern jclass JPy_Byte_JClass;
-extern jmethodID JPy_Byte_Init_MID;
-
-extern jclass JPy_Short_JClass;
-extern jmethodID JPy_Short_Init_MID;
-
-extern jclass JPy_Integer_JClass;
-extern jmethodID JPy_Integer_Init_MID;
-
-extern jclass JPy_Long_JClass;
-extern jmethodID JPy_Long_Init_MID;
-
-extern jclass JPy_Float_JClass;
-extern jmethodID JPy_Float_Init_MID;
-
-extern jclass JPy_Double_JClass;
-extern jmethodID JPy_Double_Init_MID;
-
-extern jclass JPy_Number_JClass;
-extern jmethodID JPy_Number_IntValue_MID;
-extern jmethodID JPy_Number_LongValue_MID;
-extern jmethodID JPy_Number_DoubleValue_MID;
-
-extern jclass JPy_String_JClass;
-extern jclass JPy_Void_JClass;
-
-extern jmethodID JPy_PyObject_GetPointer_MID;
-extern jmethodID JPy_PyObject_Init_MID;
-
-#ifdef __cplusplus
-} /* extern "C" */
-#endif
+/*
+ * Copyright (C) 2014 Brockmann Consult GmbH
+ *
+ * This program is free software; you can redistribute it and/or modify it under the terms of the GNU
+ * General Public License as published by the Free Software Foundation; either version 3 of the License,
+ * or (at your option) any later version. This program is distributed in the hope that it will be useful,
+ * but WITHOUT ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS FOR A
+ * PARTICULAR PURPOSE. See the GNU General Public License for more details.
+ *
+ * You should have received a copy of the GNU General Public License along with this program; if not, see
+ * http://www.gnu.org/licenses/
+ */
+
+#ifndef JPY_MODULE_H
+#define JPY_MODULE_H
+
+#ifdef __cplusplus
+extern "C" {
+#endif
+
+#include <Python.h>
+#include <structmember.h>
+#include <jni.h>
+
+#include "jpy_compat.h"
+
+#define JPY_JNI_VERSION JNI_VERSION_1_6
+
+extern PyObject* JPy_Module;
+extern PyObject* JPy_Types;
+extern PyObject* JPy_Type_Callbacks;
+extern PyObject* JException_Type;
+
+extern JavaVM* JPy_JVM;
+extern jboolean JPy_MustDestroyJVM;
+
+
+#define JPy_JTYPE_ATTR_NAME_JINIT "__jinit__"
+
+#define JPy_MODULE_ATTR_NAME_TYPES "types"
+#define JPy_MODULE_ATTR_NAME_TYPE_CALLBACKS "type_callbacks"
+
+
+/**
+ * Gets the current JNI environment pointer.
+ * Returns NULL, if the JVM is down.
+ *
+ * General jpy design guideline: Use the JPy_GetJNIEnv function only in entry points from Python calls into C.
+ * Add a JNIEnv* as first parameter to all functions that require it.
+ */
+JNIEnv* JPy_GetJNIEnv(void);
+
+int JPy_InitGlobalVars(JNIEnv* jenv);
+void JPy_ClearGlobalVars(JNIEnv* jenv);
+
+/**
+ * Gets the current JNI environment pointer JENV. If this is NULL, it returns the given RET_VALUE.
+ * Warning: This method may immediately return, so make sure there will be no memory leaks in this case.
+ *
+ * General jpy design guideline: Use the JPy_GET_JNI_ENV_OR_RETURN macro only in entry points from Python calls into C.
+ * Add a JNIEnv* as first parameter to all functions that require it.
+ */
+#define JPy_GET_JNI_ENV_OR_RETURN(JENV, RET_VALUE) \
+    if ((JENV = JPy_GetJNIEnv()) == NULL) { \
+        return (RET_VALUE); \
+    } else { \
+    }
+
+
+/**
+ * Fetches the last Java exception occurred and raises a new Python exception.
+ */
+void JPy_HandleJavaException(JNIEnv* jenv);
+
+
+#define JPy_ON_JAVA_EXCEPTION_GOTO(LABEL) \
+    if ((*jenv)->ExceptionCheck(jenv)) { \
+        JPy_HandleJavaException(jenv); \
+        goto LABEL; \
+    }
+
+#define JPy_ON_JAVA_EXCEPTION_RETURN(VALUE) \
+    if ((*jenv)->ExceptionCheck(jenv)) { \
+        JPy_HandleJavaException(jenv); \
+        return VALUE; \
+    }
+
+
+struct JPy_JType;
+
+extern struct JPy_JType* JPy_JBoolean;
+extern struct JPy_JType* JPy_JChar;
+extern struct JPy_JType* JPy_JByte;
+extern struct JPy_JType* JPy_JShort;
+extern struct JPy_JType* JPy_JInt;
+extern struct JPy_JType* JPy_JLong;
+extern struct JPy_JType* JPy_JFloat;
+extern struct JPy_JType* JPy_JDouble;
+extern struct JPy_JType* JPy_JVoid;
+extern struct JPy_JType* JPy_JBooleanObj;
+extern struct JPy_JType* JPy_JCharacterObj;
+extern struct JPy_JType* JPy_JByteObj;
+extern struct JPy_JType* JPy_JShortObj;
+extern struct JPy_JType* JPy_JIntegerObj;
+extern struct JPy_JType* JPy_JLongObj;
+extern struct JPy_JType* JPy_JFloatObj;
+extern struct JPy_JType* JPy_JDoubleObj;
+extern struct JPy_JType* JPy_JObject;
+extern struct JPy_JType* JPy_JString;
+extern struct JPy_JType* JPy_JPyObject;
+extern struct JPy_JType* JPy_JPyModule;
+
+// java.lang.Comparable
+extern jclass JPy_Comparable_JClass;
+extern jmethodID JPy_Comparable_CompareTo_MID;
+// java.lang.Object
+extern jclass JPy_Object_JClass;
+extern jmethodID JPy_Object_ToString_MID;
+extern jmethodID JPy_Object_HashCode_MID;
+extern jmethodID JPy_Object_Equals_MID;
+// java.lang.Class
+extern jclass JPy_Class_JClass;
+extern jmethodID JPy_Class_GetName_MID;
+extern jmethodID JPy_Class_GetDeclaredConstructors_MID;
+extern jmethodID JPy_Class_GetDeclaredFields_MID;
+extern jmethodID JPy_Class_GetDeclaredMethods_MID;
+extern jmethodID JPy_Class_GetComponentType_MID;
+extern jmethodID JPy_Class_IsPrimitive_MID;
+// java.lang.reflect.Constructor
+extern jclass JPy_Constructor_JClass;
+extern jmethodID JPy_Constructor_GetModifiers_MID;
+extern jmethodID JPy_Constructor_GetParameterTypes_MID;
+// java.lang.reflect.Method
+extern jclass JPy_Method_JClass;
+extern jmethodID JPy_Method_GetName_MID;
+extern jmethodID JPy_Method_GetModifiers_MID;
+extern jmethodID JPy_Method_GetParameterTypes_MID;
+extern jmethodID JPy_Method_GetReturnType_MID;
+// java.lang.reflect.Field
+extern jclass JPy_Field_JClass;
+extern jmethodID JPy_Field_GetName_MID;
+extern jmethodID JPy_Field_GetModifiers_MID;
+extern jmethodID JPy_Field_GetType_MID;
+
+extern jclass JPy_RuntimeException_JClass;
+
+extern jclass JPy_Boolean_JClass;
+extern jmethodID JPy_Boolean_Init_MID;
+extern jmethodID JPy_Boolean_BooleanValue_MID;
+
+extern jclass JPy_Character_JClass;
+extern jmethodID JPy_Character_Init_MID;
+extern jmethodID JPy_Character_CharValue_MID;
+
+extern jclass JPy_Byte_JClass;
+extern jmethodID JPy_Byte_Init_MID;
+
+extern jclass JPy_Short_JClass;
+extern jmethodID JPy_Short_Init_MID;
+
+extern jclass JPy_Integer_JClass;
+extern jmethodID JPy_Integer_Init_MID;
+
+extern jclass JPy_Long_JClass;
+extern jmethodID JPy_Long_Init_MID;
+
+extern jclass JPy_Float_JClass;
+extern jmethodID JPy_Float_Init_MID;
+
+extern jclass JPy_Double_JClass;
+extern jmethodID JPy_Double_Init_MID;
+
+extern jclass JPy_Number_JClass;
+extern jmethodID JPy_Number_IntValue_MID;
+extern jmethodID JPy_Number_LongValue_MID;
+extern jmethodID JPy_Number_DoubleValue_MID;
+
+extern jclass JPy_String_JClass;
+extern jclass JPy_Void_JClass;
+
+extern jmethodID JPy_PyObject_GetPointer_MID;
+extern jmethodID JPy_PyObject_Init_MID;
+
+#ifdef __cplusplus
+} /* extern "C" */
+#endif
 #endif /* !JPY_MODULE_H */
```

## Comparing `jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.c` & `jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.c`

 * *Files 2% similar despite different names*

```diff
@@ -118,18 +118,20 @@
 JNIEXPORT void JNICALL Java_org_jpy_PyLib_startPython
   (JNIEnv* jenv, jclass jLibClass, jobjectArray options)
 {
 
     JPy_DIAG_PRINT(JPy_DIAG_F_ALL, "PyLib_startPython: entered: jenv=%p, JPy_Module=%p\n", jenv, JPy_Module);
 
     if (!Py_IsInitialized()) {
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
         Py_SetProgramName(L"java");
-#else
+#elif defined(JPY_COMPAT_27)
         Py_SetProgramName("java");
+#else
+        #error JPY_VERSION_ERROR
 #endif
         Py_Initialize();
         PyLib_RedirectStdOut();
     }
 
     // if JPy_Module is still NULL, then the 'jpy' module has not been imported yet.
     //
@@ -776,48 +778,52 @@
     (*jenv)->ReleaseStringUTFChars(jenv, jName, nameChars);
     Py_XDECREF(pyCallable);
     Py_XDECREF(pyArgs);
 
     return pyReturnValue;
 }
 
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
 
 char* PyLib_ObjToChars(PyObject* pyObj, PyObject** pyNewRef)
 {
     char* chars = NULL;
     if (pyObj != NULL) {
         PyObject* pyObjStr = PyObject_Str(pyObj);
         if (pyObjStr != NULL) {
             PyObject* pyObjUtf8 = PyUnicode_AsEncodedString(pyObjStr, "utf-8", "replace");
             if (pyObjUtf8 != NULL) {
-                chars = PyBytes_AsString(*pyObjUtf8);
+                chars = PyBytes_AsString(pyObjUtf8);
                 *pyNewRef = pyObjUtf8;
             }
             Py_XDECREF(pyObjStr);
         }
     }
     return chars;
 }
 
-#else
+#elif defined(JPY_COMPAT_27)
 
 char* PyLib_ObjToChars(PyObject* pyObj, PyObject** pyNewRef)
 {
     char* chars = NULL;
     if (pyObj != NULL) {
         PyObject* pyObjStr = PyObject_Str(pyObj);
         if (pyObjStr != NULL) {
             chars = PyBytes_AsString(pyObjStr);
             *pyNewRef = pyObjStr;
         }
     }
     return chars;
 }
 
+#else
+
+#error JPY_VERSION_ERROR
+
 #endif
 
 #define JPY_NOT_AVAILABLE_MSG "<not available>"
 #define JPY_NOT_AVAILABLE_MSG_LEN strlen(JPY_NOT_AVAILABLE_MSG)
 #define JPY_ERR_BASE_MSG "Error in Python interpreter"
 #define JPY_NO_INFO_MSG JPY_ERR_BASE_MSG ", no information available"
 #define JPY_INFO_ALLOC_FAILED_MSG JPY_ERR_BASE_MSG ", failed to allocate information text"
@@ -948,15 +954,15 @@
 
     {NULL, NULL, 0, NULL} /*Sentinel*/
 };
 
 #define JPY_STDOUT_MODULE_NAME "jpy_stdout"
 #define JPY_STDOUT_MODULE_DOC  "Redirect 'stdout' to the console in embedded mode"
 
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
 static struct PyModuleDef JPrint_ModuleDef =
 {
     PyModuleDef_HEAD_INIT,
     JPY_STDOUT_MODULE_NAME, /* Name of the Python JPy_Module */
     JPY_STDOUT_MODULE_DOC,  /* Module documentation */
     -1,                 /* Size of per-interpreter state of the JPy_Module, or -1 if the JPy_Module keeps state in global variables. */
     JPrint_Functions,    /* Structure containing global jpy-functions */
@@ -966,18 +972,20 @@
     NULL      // m_free
 };
 #endif
 
 void PyLib_RedirectStdOut(void)
 {
     PyObject* module;
-#if PY_MAJOR_VERSION >= 3
+#if defined(JPY_COMPAT_33P)
     module = PyModule_Create(&JPrint_ModuleDef);
-#else
+#elif defined(JPY_COMPAT_27)
     module = Py_InitModule3(JPY_STDOUT_MODULE_NAME, JPrint_Functions, JPY_STDOUT_MODULE_DOC);
+#else
+    #error JPY_VERSION_ERROR
 #endif
     PySys_SetObject("stdout", module);
     PySys_SetObject("stderr", module);
 }
```

## Comparing `jpy-0.7.4/src/main/c/jni/org_jpy_PyLib.h` & `jpy-0.7.5/src/main/c/jni/org_jpy_PyLib.h`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/c/jni/org_jpy_PyLib_Diag.h` & `jpy-0.7.5/src/main/c/jni/org_jpy_PyLib_Diag.h`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/package-info.java` & `jpy-0.7.5/src/main/java/org/jpy/package-info.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/PyLib.java` & `jpy-0.7.5/src/main/java/org/jpy/PyLib.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/PyLibConfig.java` & `jpy-0.7.5/src/main/java/org/jpy/PyLibConfig.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/PyModule.java` & `jpy-0.7.5/src/main/java/org/jpy/PyModule.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/PyObject.java` & `jpy-0.7.5/src/main/java/org/jpy/PyObject.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/PyProxyHandler.java` & `jpy-0.7.5/src/main/java/org/jpy/PyProxyHandler.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/annotations/Mutable.java` & `jpy-0.7.5/src/main/java/org/jpy/annotations/Mutable.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/annotations/Output.java` & `jpy-0.7.5/src/main/java/org/jpy/annotations/Output.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/main/java/org/jpy/annotations/Return.java` & `jpy-0.7.5/src/main/java/org/jpy/annotations/Return.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/JavaReflectionTest.java` & `jpy-0.7.5/src/test/java/org/jpy/JavaReflectionTest.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/PyLibTest.java` & `jpy-0.7.5/src/test/java/org/jpy/PyLibTest.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/PyModuleTest.java` & `jpy-0.7.5/src/test/java/org/jpy/PyModuleTest.java`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     @BeforeClass
     public static void setUp() throws Exception {
         System.out.println("PyModuleTest: Current thread: " + Thread.currentThread());
 
         PyLib.startPython();
         assertEquals(true, PyLib.isPythonRunning());
 
-        PyLib.Diag.setFlags(PyLib.Diag.F_METH);
+        //PyLib.Diag.setFlags(PyLib.Diag.F_METH);
     }
 
     @AfterClass
     public static void tearDown() throws Exception {
         PyLib.Diag.setFlags(PyLib.Diag.F_OFF);
         //PyLib.stopPython();
     }
```

## Comparing `jpy-0.7.4/src/test/java/org/jpy/PyObjectTest.java` & `jpy-0.7.5/src/test/java/org/jpy/PyObjectTest.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/UseCases.java` & `jpy-0.7.5/src/test/java/org/jpy/UseCases.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/ConstructorOverloadTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/ExceptionTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/FieldTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/FieldTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodOverloadTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/MethodReturnValueTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/ModifyAndReturnParametersTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/Processor.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/Processor.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/Thing.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/Thing.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeConversionTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java` & `jpy-0.7.5/src/test/java/org/jpy/fixtures/TypeResolutionTestFixture.java`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_array_test.py` & `jpy-0.7.5/src/test/python/jpy_array_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_diag_test.py` & `jpy-0.7.5/src/test/python/jpy_diag_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_exception_test.py` & `jpy-0.7.5/src/test/python/jpy_exception_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_field_test.py` & `jpy-0.7.5/src/test/python/jpy_field_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_gettype_test.py` & `jpy-0.7.5/src/test/python/jpy_gettype_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_modretparam_test.py` & `jpy-0.7.5/src/test/python/jpy_modretparam_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_mt_test.py` & `jpy-0.7.5/src/test/python/jpy_mt_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_overload_test.py` & `jpy-0.7.5/src/test/python/jpy_overload_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_perf_test.py` & `jpy-0.7.5/src/test/python/jpy_perf_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_retval_test.py` & `jpy-0.7.5/src/test/python/jpy_retval_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_rt_test.py` & `jpy-0.7.5/src/test/python/jpy_rt_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_typeconv_test.py` & `jpy-0.7.5/src/test/python/jpy_typeconv_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/jpy_typeres_test.py` & `jpy-0.7.5/src/test/python/jpy_typeres_test.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/imp/import_ex1.py` & `jpy-0.7.5/src/test/python/imp/import_ex1.py`

 * *Files identical despite different names*

## Comparing `jpy-0.7.4/src/test/python/imp/import_ex2.py` & `jpy-0.7.5/src/test/python/imp/import_ex2.py`

 * *Files identical despite different names*

