# Comparing `tmp/glue_utils-0.5.0.tar.gz` & `tmp/glue_utils-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.5.0.tar", max compression
+gzip compressed data, was "glue_utils-0.5.1.tar", max compression
```

## Comparing `glue_utils-0.5.0.tar` & `glue_utils-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.5.0/LICENSE
--rw-r--r--   0        0        0     2221 2024-05-19 23:47:08.494209 glue_utils-0.5.0/README.md
--rw-r--r--   0        0        0     4142 2024-05-20 00:27:25.073298 glue_utils-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       89 2024-05-20 00:27:25.074725 glue_utils-0.5.0/src/glue_utils/__init__.py
--rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.5.0/src/glue_utils/options.py
--rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.5.0/src/glue_utils/py.typed
--rw-r--r--   0        0        0      950 2024-05-19 23:47:08.495182 glue_utils-0.5.0/src/glue_utils/pyspark/__init__.py
--rw-r--r--   0        0        0     8542 2024-05-19 23:47:08.495829 glue_utils-0.5.0/src/glue_utils/pyspark/connection_options.py
--rw-r--r--   0        0        0      919 2024-05-19 23:47:08.496480 glue_utils-0.5.0/src/glue_utils/pyspark/connection_types.py
--rw-r--r--   0        0        0      897 2024-05-19 23:47:08.496994 glue_utils-0.5.0/src/glue_utils/pyspark/context/__init__.py
--rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.497455 glue_utils-0.5.0/src/glue_utils/pyspark/context/documentdb.py
--rw-r--r--   0        0        0     2154 2024-05-19 23:47:08.497854 glue_utils-0.5.0/src/glue_utils/pyspark/context/dynamodb.py
--rw-r--r--   0        0        0    10415 2024-05-19 23:47:08.498336 glue_utils-0.5.0/src/glue_utils/pyspark/context/jdbc.py
--rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.498764 glue_utils-0.5.0/src/glue_utils/pyspark/context/kinesis.py
--rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.499372 glue_utils-0.5.0/src/glue_utils/pyspark/context/mongodb.py
--rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.499825 glue_utils-0.5.0/src/glue_utils/pyspark/context/opensearch.py
--rw-r--r--   0        0        0    10403 2024-05-19 23:47:08.500298 glue_utils-0.5.0/src/glue_utils/pyspark/context/s3.py
--rw-r--r--   0        0        0     2007 2024-05-19 23:47:08.500797 glue_utils-0.5.0/src/glue_utils/pyspark/format_options.py
--rw-r--r--   0        0        0      259 2024-05-19 23:47:08.501108 glue_utils-0.5.0/src/glue_utils/pyspark/formats.py
--rw-r--r--   0        0        0     6123 2024-05-20 00:26:10.700994 glue_utils-0.5.0/src/glue_utils/pyspark/job.py
--rw-r--r--   0        0        0     3333 1970-01-01 00:00:00.000000 glue_utils-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.5.1/LICENSE
+-rw-r--r--   0        0        0     2215 2024-05-23 00:48:09.013585 glue_utils-0.5.1/README.md
+-rw-r--r--   0        0        0     4165 2024-05-23 00:52:29.441391 glue_utils-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0       89 2024-05-23 00:52:29.443646 glue_utils-0.5.1/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0     1050 2024-05-10 09:44:26.756369 glue_utils-0.5.1/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-03 09:02:47.986990 glue_utils-0.5.1/src/glue_utils/py.typed
+-rw-r--r--   0        0        0      950 2024-05-19 23:47:08.495182 glue_utils-0.5.1/src/glue_utils/pyspark/__init__.py
+-rw-r--r--   0        0        0    10402 2024-05-23 00:48:09.018342 glue_utils-0.5.1/src/glue_utils/pyspark/connection_options.py
+-rw-r--r--   0        0        0      907 2024-05-22 10:21:48.665732 glue_utils-0.5.1/src/glue_utils/pyspark/connection_types.py
+-rw-r--r--   0        0        0      943 2024-05-22 10:21:48.666042 glue_utils-0.5.1/src/glue_utils/pyspark/context/__init__.py
+-rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.497455 glue_utils-0.5.1/src/glue_utils/pyspark/context/documentdb.py
+-rw-r--r--   0        0        0     2154 2024-05-19 23:47:08.497854 glue_utils-0.5.1/src/glue_utils/pyspark/context/dynamodb.py
+-rw-r--r--   0        0        0    10415 2024-05-19 23:47:08.498336 glue_utils-0.5.1/src/glue_utils/pyspark/context/jdbc.py
+-rw-r--r--   0        0        0     2103 2024-05-22 10:21:48.666259 glue_utils-0.5.1/src/glue_utils/pyspark/context/kafka.py
+-rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.498764 glue_utils-0.5.1/src/glue_utils/pyspark/context/kinesis.py
+-rw-r--r--   0        0        0     2137 2024-05-19 23:47:08.499372 glue_utils-0.5.1/src/glue_utils/pyspark/context/mongodb.py
+-rw-r--r--   0        0        0     2188 2024-05-19 23:47:08.499825 glue_utils-0.5.1/src/glue_utils/pyspark/context/opensearch.py
+-rw-r--r--   0        0        0    10403 2024-05-19 23:47:08.500298 glue_utils-0.5.1/src/glue_utils/pyspark/context/s3.py
+-rw-r--r--   0        0        0     2079 2024-05-22 10:21:48.666547 glue_utils-0.5.1/src/glue_utils/pyspark/format_options.py
+-rw-r--r--   0        0        0      287 2024-05-22 10:21:48.666826 glue_utils-0.5.1/src/glue_utils/pyspark/formats.py
+-rw-r--r--   0        0        0     6123 2024-05-20 00:26:10.700994 glue_utils-0.5.1/src/glue_utils/pyspark/job.py
+-rw-r--r--   0        0        0     3327 1970-01-01 00:00:00.000000 glue_utils-0.5.1/PKG-INFO
```

### Comparing `glue_utils-0.5.0/LICENSE` & `glue_utils-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/README.md` & `glue_utils-0.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,28 +18,28 @@
 
 ```sh
 pip install glue-utils
 ```
 
 ### For development...
 
-This library does not include `pyspark` and `aws-glue-libs` as 
-dependencies as they are already pre-installed in Glue's runtime 
+This library does not include `pyspark` and `aws-glue-libs` as
+dependencies as they are already pre-installed in Glue's runtime
 environment.
 
-To help in developing your Glue jobs locally in your IDE, it is helpful 
-to install `pyspark` and `aws-glue-libs`. Unfortunately, `aws-glue-libs` 
-is not available through PyPI so we can only install it from its git 
+To help in developing your Glue jobs locally in your IDE, it is helpful
+to install `pyspark` and `aws-glue-libs`. Unfortunately, `aws-glue-libs`
+is not available through PyPI so we can only install it from its git
 repository.
 
 ```sh
 pip install pyspark==3.3.0
 pip install git+https://github.com/awslabs/aws-glue-libs.git@master
 ```
 
-To make your local environment as close to Glue's runtime as possible, 
+To make your local environment as close to Glue's runtime as possible,
 use the versions specified in [this document](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-libraries.html#glue-modules-provided).
 
 ## Documentation
 
-For more details on what you can use this library for, check out the 
-[project wiki](https://github.com/dashmug/glue-utils/wiki).
+For more details on what you can use this library for, check out the
+[project wiki](https://github.com/dashmug/glue-utils/wiki).
```

### Comparing `glue_utils-0.5.0/pyproject.toml` & `glue_utils-0.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.5.0"
+version = "0.5.1"
 package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
@@ -34,23 +34,24 @@
 pytest-randomly = "^3.15.0"
 pytest-cov = "^5.0.0"
 mypy = "^1.10.0"
 bumpver = "^2023.1129"
 import-linter = "^2.0"
 ruff = "^0.4.4"
 pytest = "^8.2.1"
+pre-commit = "^3.7.1"
 
 [tool.poetry.group.local.dependencies]
-# The "local" dependency group refers to dependencies that already 
+# The "local" dependency group refers to dependencies that already
 # exist in AWS Glue's runtime. We don't need to install these in the
-# container. We only need them for local (non-container) development to 
+# container. We only need them for local (non-container) development to
 # aid the IDE in providing code completion and type checking.
-# 
-# It is best to keep the dependencies here in sync with what's on Glue's 
-# documentation. 
+#
+# It is best to keep the dependencies here in sync with what's on Glue's
+# documentation.
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-libraries.html#glue-modules-provided
 aws-glue-libs = { git = "https://github.com/awslabs/aws-glue-libs.git", rev = "master" }
 pyspark = "3.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
@@ -101,29 +102,30 @@
 
 [[tool.mypy.overrides]]
 module = "test.*"
 disallow_incomplete_defs = false
 disallow_untyped_defs = false
 
 [tool.pytest.ini_options]
-addopts = "--cov=glue_utils --cov-report=term --cov-report=html --cov-report=xml"
+addopts = "-p no:cacheprovider --cov=glue_utils --cov-report=term"
 filterwarnings = [
     "ignore::FutureWarning:pyspark.sql.context",
 ]
 
 [tool.coverage.run]
 relative_files = true
 branch = true
 omit = ["**/test_*.py"]
 
 [tool.coverage.paths]
 source = ["src/glue_utils", "*/site-packages/glue_utils"]
 
 [tool.coverage.report]
 skip_empty = true
+show_missing = true
 exclude_also = [
     "def __repr__",
     "if self.debug:",
     "if settings.DEBUG",
     "raise AssertionError",
     "raise NotImplementedError",
     "if 0:",
@@ -134,15 +136,15 @@
     "@overload",
 ]
 
 [tool.coverage.xml]
 output = "coverage/results.xml"
 
 [tool.bumpver]
-current_version = "0.5.0"
+current_version = "0.5.1"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "release: Bump version {old_version} -> {new_version}"
 commit = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
@@ -157,8 +159,8 @@
 
 [tool.importlinter]
 root_package = "glue_utils"
 
 [[tool.importlinter.contracts]]
 name = "Generic code should not import specific code"
 type = "layers"
-layers = ["glue_utils.pyspark", "glue_utils.options"]
+layers = ["glue_utils.pyspark", "glue_utils.options"]
```

### Comparing `glue_utils-0.5.0/src/glue_utils/options.py` & `glue_utils-0.5.1/src/glue_utils/options.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/__init__.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/connection_options.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/connection_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Literal, TypedDict  # noqa: D100
+"""Module containing dictionary structures for handling different connection types."""
+
+from typing import Literal, TypedDict
 
 
 class BookmarkConnectionOptions(TypedDict, total=False):
     """TypedDict class representing general connection options.
 
     Reference
     ---------
@@ -28,30 +30,30 @@
     databaseName: str
     url: str
     dbtable: str
     user: str
     password: str
     customJdbcDriverS3Path: str
     customJdbcDriverClassName: str
-    bulkSize: int
+    bulkSize: str
     hashfield: str
     hashexpression: str
-    hashpartitions: int
+    hashpartitions: str
     sampleQuery: str
-    enablePartitioningForSampleQuery: bool
-    sampleSize: int
+    enablePartitioningForSampleQuery: Literal["true", "false"]
+    sampleSize: str
 
 
 # Redshift has a connection option with a dot in it, so we need to use
 # this form of TypedDict to define the connection options.
 RedshiftOptions = TypedDict(
     "RedshiftOptions",
     {
-        "autopushdown": bool,
-        "autopushdown.s3_result_cache": bool,
+        "autopushdown": Literal["true", "false"],
+        "autopushdown.s3_result_cache": Literal["true", "false"],
         "aws_iam_role": str,
         "csvnullstring": str,
         "DbUser": str,
         "extracopyoptions": str,
         "redshiftTmpDir": str,
         "sse_kms_key": str,
         "unload_s3_format": Literal["TEXT", "PARQUET"],
@@ -83,21 +85,21 @@
     """
 
     paths: list[str]
     exclusions: str
     compressionType: Literal["gzip", "bzip2"]
     groupFiles: Literal["inPartition", "none"]
     groupSize: str
-    recurse: bool
-    maxBand: int
-    maxFilesInBand: int
-    isFailFast: bool
+    recurse: Literal["true", "false"]
+    maxBand: str
+    maxFilesInBand: str
+    isFailFast: Literal["true", "false"]
     catalogPartitionPredicate: str
     excludeStorageClasses: list[str]
-    useS3ListImplementation: bool
+    useS3ListImplementation: Literal["true", "false"]
 
 
 class S3SinkConnectionOptions(BookmarkConnectionOptions, total=False):
     """Connection options for writing data to an S3 sink."""
 
     path: str
     compression: Literal["gzip", "bzip2"]
@@ -105,38 +107,38 @@
 
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-dynamodb-home.html
 DynamoDBSourceConnectionOptions = TypedDict(
     "DynamoDBSourceConnectionOptions",
     {
         "dynamodb.input.tableName": str,
-        "dynamodb.throughput.read.percent": float,
-        "dynamodb.splits": int,
+        "dynamodb.throughput.read.percent": str,
+        "dynamodb.splits": str,
         "dynamodb.sts.roleArn": str,
         "dynamodb.sts.roleSessionName": str,
         "dynamodb.sts.region": str,
         "dynamodb.export": Literal["ddb", "s3"],
         "dynamodb.tableArn": str,
         "dynamodb.s3.bucket": str,
         "dynamodb.s3.prefix": str,
         "dynamodb.s3.bucketOwner": str,
-        "dynamodb.simplifyDDBJson": bool,
+        "dynamodb.simplifyDDBJson": Literal["true", "false"],
         "dynamodb.exportTime": str,
     },
     total=False,
 )
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-dynamodb-home.html
 DynamoDBSinkConnectionOptions = TypedDict(
     "DynamoDBSinkConnectionOptions",
     {
         "dynamodb.output.tableName": str,
-        "dynamodb.throughput.write.percent": float,
-        "dynamodb.output.numParallelTasks": int,
-        "dynamodb.output.retry": int,
+        "dynamodb.throughput.write.percent": str,
+        "dynamodb.output.numParallelTasks": str,
+        "dynamodb.output.retry": str,
         "dynamodb.sts.roleArn": str,
         "dynamodb.sts.roleSessionName": str,
     },
     total=False,
 )
 
 
@@ -146,70 +148,70 @@
     Reference
     ---------
     - https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-kinesis-home.html
 
     """
 
     streamARN: str
-    failOnDataLoss: bool
+    failOnDataLoss: Literal["true", "false"]
     awsSTSRoleArn: str
     awsSTSSessionName: str
-    awsSTSEndpoint: str
+    awsSTSEndpostr: str
 
 
 class KinesisSourceConnectionOptions(KinesisConnectionOptions, total=False):
     """Connection options to read from Kinesis."""
 
     classification: str
     streamName: str
-    endpointUrl: str
+    endpostrUrl: str
     delimiter: str
     startingPosition: str
-    maxFetchTimeInMs: int
-    maxFetchRecordsPerShard: int
-    maxRecordPerRead: int
-    addIdleTimeBetweenReads: bool
-    idleTimeBetweenReadsInMs: int
-    describeShardInterval: str
-    numRetries: int
-    retryIntervalMs: int
-    maxRetryIntervalMs: int
-    avoidEmptyBatches: bool
+    maxFetchTimeInMs: str
+    maxFetchRecordsPerShard: str
+    maxRecordPerRead: str
+    addIdleTimeBetweenReads: Literal["true", "false"]
+    idleTimeBetweenReadsInMs: str
+    describeShardStrerval: str
+    numRetries: str
+    retryStrervalMs: str
+    maxRetryStrervalMs: str
+    avoidEmptyBatches: Literal["true", "false"]
     schema: str
-    inferSchema: bool
-    addRecordTimestamp: bool
-    emitConsumerLagMetrics: bool
+    inferSchema: Literal["true", "false"]
+    addRecordTimestamp: Literal["true", "false"]
+    emitConsumerLagMetrics: Literal["true", "false"]
     fanoutConsumerARN: str
 
 
 class KinesisSinkConnectionOptions(KinesisConnectionOptions, total=False):
     """Connection options for writing to Kinesis."""
 
     partitionKey: str
-    recordMaxBufferedTime: int
-    aggregationEnabled: bool
-    aggregationMaxSize: int
-    aggregationMaxCount: int
-    producerRateLimit: int
-    collectionMaxCount: int
-    collectionMaxSize: int
+    recordMaxBufferedTime: str
+    aggregationEnabled: Literal["true", "false"]
+    aggregationMaxSize: str
+    aggregationMaxCount: str
+    producerRateLimit: str
+    collectionMaxCount: str
+    collectionMaxSize: str
 
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-documentdb-home.html
 DocumentDBSourceConnectionOptions = TypedDict(
     "DocumentDBSourceConnectionOptions",
     {
         "uri": str,
         "database": str,
         "collection": str,
         "username": str,
         "password": str,
-        "ssl": bool,
-        "ssl.domain_match": bool,
-        "batchSize": int,
+        "ssl": str,
+        "ssl.domain_match": str,
+        "batchSize": str,
         "partitioner": str,
         "partitionerOptions.partitionKey": str,
         "partitionerOptions.partitionSizeMB": str,
         "partitionerOptions.samplesPerPartition": str,
         "partitionerOptions.shardKey": str,
         "partitionerOptions.numberOfPartitions": str,
     },
@@ -225,35 +227,35 @@
     """
 
     uri: str
     database: str
     collection: str
     username: str
     password: str
-    extendedBSONTypes: bool
-    replaceDocument: bool
-    maxBatchSize: int
-    retryWrites: bool
+    extendedBSONTypes: str
+    replaceDocument: str
+    maxBatchSize: str
+    retryWrites: str
 
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-mongodb-home.html
 MongoDBSourceConnectionOptions = TypedDict(
     "MongoDBSourceConnectionOptions",
     {
         "connectionName": str,
         "uri": str,
         "connection.uri": str,
         "username": str,
         "password": str,
         "database": str,
         "collection": str,
-        "ssl": bool,
-        "ssl.domain_match": bool,
-        "disableUpdateUri": bool,
-        "batchSize": int,
+        "ssl": Literal["true", "false"],
+        "ssl.domain_match": Literal["true", "false"],
+        "disableUpdateUri": Literal["true", "false"],
+        "batchSize": str,
         "partitioner": str,
         "partitionerOptions.partitionKey": str,
         "partitionerOptions.partitionSizeMB": str,
         "partitionerOptions.samplesPerPartition": str,
         "partitionerOptions.shardKey": str,
         "partitionerOptions.numberOfPartitions": str,
     },
@@ -267,40 +269,83 @@
         "connectionName": str,
         "uri": str,
         "connection.uri": str,
         "username": str,
         "password": str,
         "database": str,
         "collection": str,
-        "ssl": bool,
-        "ssl.domain_match": bool,
-        "disableUpdateUri": bool,
-        "extendedBSONTypes": bool,
-        "replaceDocument": bool,
-        "maxBatchSize": int,
-        "retryWrites": bool,
+        "ssl": Literal["true", "false"],
+        "ssl.domain_match": Literal["true", "false"],
+        "disableUpdateUri": Literal["true", "false"],
+        "extendedBSONTypes": Literal["true", "false"],
+        "replaceDocument": Literal["true", "false"],
+        "maxBatchSize": str,
+        "retryWrites": Literal["true", "false"],
     },
     total=False,
 )
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-opensearch-home.html
 OpenSearchSourceConnectionOptions = TypedDict(
     "OpenSearchSourceConnectionOptions",
     {
         "connectionName": str,
         "opensearch.resource": str,
         "opensearch.query": str,
-        "pushdown": bool,
+        "pushdown": Literal["true", "false"],
         "opensearch.read.field.as.array.include": str,
     },
     total=False,
 )
 
 # https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-opensearch-home.html
 OpenSearchSinkConnectionOptions = TypedDict(
     "OpenSearchSinkConnectionOptions",
     {
         "connectionName": str,
         "opensearch.resource": str,
     },
     total=False,
 )
+
+# https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-kafka-home.html
+KafkaSourceConnectionOptions = TypedDict(
+    "KafkaSourceConnectionOptions",
+    {
+        "connectionName": str,
+        "bootstrap.servers": str,
+        "security.protocol": Literal["SSL", "PLAINTEXT"],
+        "topicName": str,
+        "assign": str,
+        "subscribePattern": str,
+        "classification": str,
+        "delimiter": str,
+        "startingOffsets": Literal["earliest", "latest"],
+        "startingTimestamp": str,
+        "endingOffsets": str,
+        "pollTimeoutMs": str,
+        "numRetries": str,
+        "retryStrervalMs": str,
+        "maxOffsetsPerTrigger": str,
+        "minPartitions": str,
+        "includeHeaders": Literal["true", "false"],
+        "schema": str,
+        "inferSchema": Literal["true", "false"],
+        "addRecordTimestamp": Literal["true", "false"],
+        "emitConsumerLagMetrics": Literal["true", "false"],
+    },
+    total=False,
+)
+
+
+class KafkaSinkConnectionOptions(TypedDict, total=False):
+    """Connection options for writing to Kafka.
+
+    Reference:
+    - https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-etl-connect-kafka-home.html
+    """
+
+    connectionName: str
+    topicName: str
+    partition: str
+    key: str
+    classification: str
```

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/connection_types.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/connection_types.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Module containing classes and types for handling different connection types."""
+"""Module containing types for handling different connection types."""
 
 from enum import Enum
 
 
 class ConnectionType(Enum):
     """Enum class representing different types of connections."""
```

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/__init__.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 from __future__ import annotations
 
 from awsglue.context import GlueContext
 
 from .documentdb import DocumentDBMixin
 from .dynamodb import DynamoDBMixin
 from .jdbc import JDBCMixin
+from .kafka import KafkaMixin
 from .kinesis import KinesisMixin
 from .mongodb import MongoDBMixin
 from .opensearch import OpenSearchMixin
 from .s3 import S3Mixin
 
 
 class GluePySparkContext(
     DocumentDBMixin,
     DynamoDBMixin,
     JDBCMixin,
+    KafkaMixin,
     KinesisMixin,
     MongoDBMixin,
     OpenSearchMixin,
     S3Mixin,
     # awsglue has no typings yet
     GlueContext,  # type: ignore[misc]
 ):
```

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/documentdb.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/documentdb.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/dynamodb.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/dynamodb.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/jdbc.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/jdbc.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/kinesis.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/kinesis.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/mongodb.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/mongodb.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/opensearch.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/opensearch.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/context/s3.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/context/s3.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/format_options.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/format_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-from typing import Literal, TypedDict  # noqa: D100
+"""Module containing dictionary structures for handling different format options."""
+
+from typing import Literal, TypedDict
 
 
 class S3FormatOptions(TypedDict, total=False):
     """Common format options for S3."""
 
     attachFilename: str
     attachTimestamp: str
```

### Comparing `glue_utils-0.5.0/src/glue_utils/pyspark/job.py` & `glue_utils-0.5.1/src/glue_utils/pyspark/job.py`

 * *Files identical despite different names*

### Comparing `glue_utils-0.5.0/PKG-INFO` & `glue_utils-0.5.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.5.0
+Version: 0.5.1
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -44,28 +44,29 @@
 
 ```sh
 pip install glue-utils
 ```
 
 ### For development...
 
-This library does not include `pyspark` and `aws-glue-libs` as 
-dependencies as they are already pre-installed in Glue's runtime 
+This library does not include `pyspark` and `aws-glue-libs` as
+dependencies as they are already pre-installed in Glue's runtime
 environment.
 
-To help in developing your Glue jobs locally in your IDE, it is helpful 
-to install `pyspark` and `aws-glue-libs`. Unfortunately, `aws-glue-libs` 
-is not available through PyPI so we can only install it from its git 
+To help in developing your Glue jobs locally in your IDE, it is helpful
+to install `pyspark` and `aws-glue-libs`. Unfortunately, `aws-glue-libs`
+is not available through PyPI so we can only install it from its git
 repository.
 
 ```sh
 pip install pyspark==3.3.0
 pip install git+https://github.com/awslabs/aws-glue-libs.git@master
 ```
 
-To make your local environment as close to Glue's runtime as possible, 
+To make your local environment as close to Glue's runtime as possible,
 use the versions specified in [this document](https://docs.aws.amazon.com/glue/latest/dg/aws-glue-programming-python-libraries.html#glue-modules-provided).
 
 ## Documentation
 
-For more details on what you can use this library for, check out the 
+For more details on what you can use this library for, check out the
 [project wiki](https://github.com/dashmug/glue-utils/wiki).
+
```

