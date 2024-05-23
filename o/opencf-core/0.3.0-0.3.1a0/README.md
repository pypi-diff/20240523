# Comparing `tmp/opencf_core-0.3.0.tar.gz` & `tmp/opencf_core-0.3.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf_core-0.3.0.tar", max compression
+gzip compressed data, was "opencf_core-0.3.1a0.tar", max compression
```

## Comparing `opencf_core-0.3.0.tar` & `opencf_core-0.3.1a0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     7078 2024-05-03 17:07:50.871608 opencf_core-0.3.0/README.md
--rw-r--r--   0        0        0        0 2024-05-03 17:07:50.875608 opencf_core-0.3.0/opencf_core/__init__.py
--rw-r--r--   0        0        0    19442 2024-05-03 17:31:07.238604 opencf_core-0.3.0/opencf_core/base_converter.py
--rw-r--r--   0        0        0     6210 2024-05-03 17:33:26.276403 opencf_core-0.3.0/opencf_core/converter_app.py
--rw-r--r--   0        0        0    15473 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/filetypes.py
--rw-r--r--   0        0        0     5891 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/io_handler.py
--rw-r--r--   0        0        0     3441 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/logging_config.py
--rw-r--r--   0        0        0     2014 2024-05-03 17:07:50.879608 opencf_core-0.3.0/opencf_core/mimes.py
--rw-r--r--   0        0        0     1108 2024-05-08 08:25:59.106994 opencf_core-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8273 1970-01-01 00:00:00.000000 opencf_core-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     7078 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/opencf_core/__init__.py
+-rw-r--r--   0        0        0    19862 2024-05-23 17:47:40.073650 opencf_core-0.3.1a0/opencf_core/base_converter.py
+-rw-r--r--   0        0        0     6430 2024-05-23 17:47:40.073650 opencf_core-0.3.1a0/opencf_core/converter_app.py
+-rw-r--r--   0        0        0     1109 2024-05-23 17:46:59.309102 opencf_core-0.3.1a0/opencf_core/exceptions.py
+-rw-r--r--   0        0        0    16054 2024-05-23 17:47:40.077650 opencf_core-0.3.1a0/opencf_core/filetypes.py
+-rw-r--r--   0        0        0     5891 2024-05-08 14:58:19.894394 opencf_core-0.3.1a0/opencf_core/io_handler.py
+-rw-r--r--   0        0        0     3566 2024-05-23 09:27:20.464956 opencf_core-0.3.1a0/opencf_core/logging_config.py
+-rw-r--r--   0        0        0     2030 2024-05-23 10:30:58.320136 opencf_core-0.3.1a0/opencf_core/mimes.py
+-rw-r--r--   0        0        0      543 2024-05-23 17:46:59.309102 opencf_core-0.3.1a0/opencf_core/utils.py
+-rw-r--r--   0        0        0     1110 2024-05-23 17:52:49.677591 opencf_core-0.3.1a0/pyproject.toml
+-rw-r--r--   0        0        0     8275 1970-01-01 00:00:00.000000 opencf_core-0.3.1a0/PKG-INFO
```

### Comparing `opencf_core-0.3.0/README.md` & `opencf_core-0.3.1a0/README.md`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.0/opencf_core/base_converter.py` & `opencf_core-0.3.1a0/opencf_core/base_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,18 +12,19 @@
 
 Exceptions:
 - ValueError: Raised when file paths or types are incompatible or unsupported.
 - AssertionError: Ensured for internal consistency checks, confirming that file types match expected values.
 """
 
 from abc import ABC, abstractmethod
+from enum import Enum
 from pathlib import Path
-from typing import Any, Iterable, List, Optional, Tuple, Union
+from typing import Any, Iterable, List, Optional, Tuple, Type, Union
 
-from .filetypes import EmptySuffixError, FileType
+from .filetypes import BaseFileType, EmptySuffixError, FileType
 from .io_handler import FileReader, FileWriter, SamePathReader
 from .logging_config import logger
 
 
 class ResolvedInputFile:
     """
     Handles resolving the file type of a given file or folder, managing path adjustments and optional content reading.
@@ -33,29 +34,35 @@
         self,
         path: Union[str, Path],
         is_dir: Optional[bool] = None,
         should_exist: bool = True,
         file_type: Optional[str] = None,
         add_suffix: bool = False,
         read_content: bool = False,
+        filetype_class: Optional[Type[BaseFileType]] = FileType,
     ):
         """
         Initializes an instance of ResolvedInputFile with options for type resolution and path modification.
 
         Args:
             path (str): The path to the file or folder.
             is_dir (bool, optional): Specifies if the path is a directory. If None, inferred using pathlib. Defaults to None.
             should_exist (bool, optional): Specifies if the existence of the path is required. Defaults to True.
-            file_type (str, optional): The explicit type of the file. If None, attempts to resolve to a FileType object based on the path or content.
+            file_type (str, optional): The explicit type of the file. If None, attempts to resolve to a filetype object based on the path or content.
             add_suffix (bool, optional): Whether to append the resolved file type's suffix to the file path. Defaults to False.
             read_content (bool, optional): Whether to read the file's content to assist in type resolution. Defaults to False.
         """
         # Convert path to Path object
         self.path = Path(path)
 
+        if filetype_class is None:
+            filetype_class = FileType
+        assert issubclass(filetype_class, Enum)
+        self.filetype_class = filetype_class
+
         self._check_existence(should_exist)
 
         # Infer if the path is a directory
         if is_dir is None:
             is_dir = self._resolve_path_type(file_type=file_type)
 
         # Resolve the file type
@@ -122,27 +129,27 @@
         """
         if self.path.is_file():
             raise ValueError(
                 f"The specified path '{self.path}' is a file, not a directory."
             )
         # Create directory if it doesn't exist
         self.path.mkdir(exist_ok=True)
-        resolved_file_type = FileType.from_suffix(file_type, raise_err=True)
+        resolved_file_type = self.filetype_class.from_suffix(file_type, raise_err=True)
         assert resolved_file_type.is_true_filetype()
         suffix = resolved_file_type.get_suffix()
         return resolved_file_type, suffix
 
     def _resolve_file_type(
         self, file_type: Optional[str], read_content: bool, add_suffix: bool
     ):
         """
         Resolves the file type based on given parameters.
 
         Args:
-            file_type (FileType or str, optional): An explicit file type or extension.
+            file_type (BaseFileType or str, optional): An explicit file type or extension.
             read_content (bool): Indicates if file content should be used to help resolve the file type.
             add_suffix (bool): Whether to append the resolved file type's suffix to the file path.
         """
         resolved_file_type = self.__resolve_filetype__(
             file_type, self.path, read_content
         )
         assert resolved_file_type.is_true_filetype()
@@ -154,37 +161,37 @@
         if add_suffix:
             self.path = self.path.with_suffix(suffix)
 
         return resolved_file_type, suffix
 
     def __resolve_filetype__(
         self, file_type: Optional[str], file_path: Path, read_content: bool
-    ) -> FileType:
+    ) -> BaseFileType:
         """
         Determines the file type, utilizing the provided type, file path, or content as needed.
 
         Args:
-            file_type (FileType or str, optional): An explicit file type or extension.
+            file_type (BaseFileType or str, optional): An explicit file type or extension.
             file_path (str): The path to the file, used if file_type is not provided.
             read_content (bool): Indicates if file content should be used to help resolve the file type.
 
         Returns:
-            FileType: The resolved file type.
+            BaseFileType: The resolved file type.
         """
         if not file_type:
             try:
-                return FileType.from_path(
+                return self.filetype_class.from_path(
                     file_path, read_content=read_content, raise_err=True
                 )
             except EmptySuffixError:
                 raise ValueError("filepath suffix is emtpy but file_type not set")
 
-        resolved_file_type = FileType.from_suffix(file_type, raise_err=True)
+        resolved_file_type = self.filetype_class.from_suffix(file_type, raise_err=True)
 
-        file_type_from_path = FileType.from_path(
+        file_type_from_path = self.filetype_class.from_path(
             file_path, read_content=read_content, raise_err=False
         )
 
         if file_type_from_path.is_true_filetype():
             assert file_type_from_path == resolved_file_type
 
         return resolved_file_type
@@ -380,76 +387,78 @@
         return cls.get_supported_input_types()
 
     @classmethod
     def get_output_types(cls):
         return cls.get_supported_output_types()
 
     @classmethod
-    def get_supported_input_types(cls) -> Tuple[FileType, ...]:
+    def get_supported_input_types(cls) -> Tuple[BaseFileType, ...]:
         """
         Defines the supported input file types for this converter.
 
         Returns:
-            Tuple[FileType]: The file types supported for input.
+            Tuple[BaseFileType]: The file types supported for input.
         """
         input_types = cls._get_supported_input_types()
 
-        # Check if input_types is a single FileType instance
-        if isinstance(input_types, FileType):
+        # Check if input_types is a single BaseFileType instance
+        if isinstance(input_types, BaseFileType):
             return (input_types,)  # Convert single instance to tuple
 
-        # Check if input_types is an iterable of FileType instances
+        # Check if input_types is an iterable of BaseFileType instances
         input_types = tuple(input_types)
-        if not all(isinstance(input_type, FileType) for input_type in input_types):
+        if not all(isinstance(input_type, BaseFileType) for input_type in input_types):
             raise ValueError("Invalid supported input file type")
 
         return input_types
 
     @classmethod
-    def get_supported_output_types(cls) -> Tuple[FileType, ...]:
+    def get_supported_output_types(cls) -> Tuple[BaseFileType, ...]:
         """
         Defines the supported output file types for this converter.
 
         Returns:
-            Tuple[FileType]: The file types supported for output.
+            Tuple[BaseFileType]: The file types supported for output.
         """
         output_types = cls._get_supported_output_types()
 
-        # Check if output_types is a single FileType instance
-        if isinstance(output_types, FileType):
+        # Check if output_types is a single BaseFileType instance
+        if isinstance(output_types, BaseFileType):
             return (output_types,)  # Convert single instance to tuple
 
-        # Check if output_types is an iterable of FileType instances
+        # Check if output_types is an iterable of BaseFileType instances
         output_types = tuple(output_types)
-        if not all(isinstance(output_type, FileType) for output_type in output_types):
+        if not all(
+            isinstance(output_type, BaseFileType) for output_type in output_types
+        ):
             raise ValueError("Invalid supported output file type")
 
         return output_types
 
     @classmethod
     @abstractmethod
-    def _get_supported_input_types(cls) -> Iterable[FileType]:
+    def _get_supported_input_types(cls) -> Iterable[BaseFileType]:
         """
         Abstract method to define the supported input file types by the converter.
 
         Returns:
-            Iterable[FileType]: The supported input file type.
+            Iterable[BaseFileType]: The supported input file type.
         """
         raise NotImplementedError(
             f"{cls.__name__}._get_supported_input_typess() must be implemented by subclasses."
         )
 
     @classmethod
     @abstractmethod
-    def _get_supported_output_types(cls) -> Iterable[FileType]:
+    def _get_supported_output_types(cls) -> Iterable[BaseFileType]:
         """
         Abstract method to define the supported output file types by the converter.
 
         Returns:
-            Iterable[FileType]: The supported output file type.
+            Iterable[BaseFileType]: The supported output file type.
         """
         raise NotImplementedError(
             f"{cls.__name__}._get_supported_output_typess() must be implemented by subclasses."
         )
 
     @abstractmethod
     def _convert(
```

### Comparing `opencf_core-0.3.0/opencf_core/converter_app.py` & `opencf_core-0.3.1a0/opencf_core/converter_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,43 +6,45 @@
 
 from collections import defaultdict
 from itertools import product
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Type
 
 from .base_converter import BaseConverter, ResolvedInputFile
-from .filetypes import FileType
+from .filetypes import BaseFileType, FileType
 from .logging_config import logger
 
 
 class BaseConverterApp:
     """
     Main application class responsible for managing file conversions.
     """
 
     converters: List[Type[BaseConverter]] = []
+    filetype_class: Type[BaseFileType] = FileType
 
     def __init__(
         self,
         input_file_paths: List[str],
         input_file_type: Optional[str] = None,
         output_file_path: Optional[str] = None,
         output_file_type: Optional[str] = None,
     ):
         """
         Initializes the BaseConverterApp instance.
 
         Args:
             input_file_paths (List[str]): List of paths to the input files.
-            input_file_type (FileType, optional): The type of the input file. Defaults to None.
+            input_file_type (BaseFileType, optional): The type of the input file. Defaults to None.
             output_file_path (str, optional): The path to the output file. Defaults to None.
-            output_file_type (FileType, optional): The type of the output file. Defaults to None.
+            output_file_type (BaseFileType, optional): The type of the output file. Defaults to None.
         """
+
         self._converter_map: Dict[
-            Tuple[FileType, FileType], List[Type[BaseConverter]]
+            Tuple[BaseFileType, BaseFileType], List[Type[BaseConverter]]
         ] = defaultdict(list)
 
         if not isinstance(input_file_paths, list):
             raise TypeError("input_file_paths sould be a list")
         if len(input_file_paths) == 0:
             raise ValueError("input_file_paths should not be a empty list")
 
@@ -50,14 +52,15 @@
             ResolvedInputFile(
                 input_file_path,
                 is_dir=False,
                 should_exist=True,
                 file_type=input_file_type,
                 add_suffix=False,
                 read_content=True,
+                filetype_class=self.filetype_class,
             )
             for input_file_path in input_file_paths
         ]
 
         self.input_file_type = self.input_files[0].file_type
         assert self.input_file_type.is_true_filetype()
 
@@ -73,14 +76,15 @@
         self.output_file = ResolvedInputFile(
             output_file_path,
             is_dir=None,
             should_exist=False,
             file_type=output_file_type,
             add_suffix=add_suffix_to_output_path,
             read_content=False,
+            filetype_class=self.filetype_class,
         )
         self.output_file_type = self.output_file.file_type
 
         for _conv_class in self.converters:
             self.add_converter_pair(_conv_class)
 
     def add_converter_pair(self, converter_class):
@@ -104,34 +108,36 @@
         output_types = converter_class.get_output_types()
 
         # Add the converter pair to the converter map
         for input_type, output_type in product(input_types, output_types):
             self._converter_map[(input_type, output_type)].append(converter_class)
 
     def get_converters_for_conversion(
-        self, input_type: FileType, output_type: FileType
+        self, input_type: BaseFileType, output_type: BaseFileType
     ) -> List[Type[BaseConverter]]:
         """
         Returns a list of converter classes for a given input-output type pair.
 
         Args:
             input_type (str): The input type.
             output_type (str): The output type.
 
         Returns:
             List[Type[BaseConverter]]: List of converter classes if found, else an empty list.
         """
         return self._converter_map[(input_type, output_type)]
 
-    def get_supported_conversions(self) -> Tuple[Tuple[FileType, FileType], ...]:
+    def get_supported_conversions(
+        self,
+    ) -> Tuple[Tuple[BaseFileType, BaseFileType], ...]:
         """
         Retrieves the supported conversions.
 
         Returns:
-            Tuple[Tuple[FileType, FileType]]: A tuple of tuples representing supported conversions.
+            Tuple[Tuple[BaseFileType, BaseFileType]]: A tuple of tuples representing supported conversions.
         """
         return tuple(self._converter_map.keys())
 
     def run(self):
         """
         Runs the conversion process.
         """
```

### Comparing `opencf_core-0.3.0/opencf_core/io_handler.py` & `opencf_core-0.3.1a0/opencf_core/io_handler.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.0/opencf_core/logging_config.py` & `opencf_core-0.3.1a0/opencf_core/logging_config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
-import os
 from datetime import datetime
+from pathlib import Path
 from typing import Optional
 
 
 class ColoredFormatter(logging.Formatter):
     """
     - original code from [Sergey Pleshakov, stackoverflow](https://stackoverflow.com/a/56944256/16668046)
     """
@@ -31,15 +31,15 @@
         formatter = logging.Formatter(log_fmt)
         return formatter.format(record)
 
 
 class LoggerConfig:
     def __init__(self) -> None:
         self.logger: logging.Logger = logging.Logger("_")
-        self.log_file: Optional[str] = None
+        self.log_file: Optional[Path] = None
         self.log_level: int = logging.INFO
 
     def setup_logger(
         self, name: str, log_file: Optional[str] = None, level: int = logging.INFO
     ) -> None:
         """Set up logger.
 
@@ -71,19 +71,21 @@
 
         Args:
             log_file (str): Path to the log file.
         """
         if log_file == "default":
             # Save log file in user's home directory with a timestamp
             timestamp = datetime.now().strftime("%Y%m%d_%H%M%S")
-            user_home = os.path.expanduser("~")
-            self.log_file = os.path.join(user_home, f"openconv-core_{timestamp}.log")
+            log_directory = Path.home() / ".cache" / "openconv-core"
+            # Create directory if it doesn't exist
+            log_directory.mkdir(parents=True, exist_ok=True)
+            self.log_file = log_directory / f"{timestamp}.log"
         else:
             # Use the provided log file path
-            self.log_file = os.path.expanduser(log_file)
+            self.log_file = Path(log_file).expanduser()
 
         file_handler = logging.FileHandler(self.log_file)
         formatter = logging.Formatter(
             "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
         )
         file_handler.setFormatter(formatter)
         self.logger.addHandler(file_handler)
```

### Comparing `opencf_core-0.3.0/opencf_core/mimes.py` & `opencf_core-0.3.1a0/opencf_core/mimes.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 This module provides a singleton class for guessing MIME types from file paths using the python-magic library.
 """
 
 try:
     import magic  # pip install python-magic
 except ImportError:
-    magic = None
+    magic = None  # type: ignore
 
 
 class MimeGuesser:
     """
     Singleton class for guessing MIME types from file paths using the python-magic library.
     """
```

### Comparing `opencf_core-0.3.0/pyproject.toml` & `opencf_core-0.3.1a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "opencf-core"
 packages = [
     {include = "opencf_core"}
 ]
-version = "0.3.0"
+version = "0.3.1a0"
 description = "A robust framework for handling file conversion tasks in Python"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `opencf_core-0.3.0/PKG-INFO` & `opencf_core-0.3.1a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf-core
-Version: 0.3.0
+Version: 0.3.1a0
 Summary: A robust framework for handling file conversion tasks in Python
 Home-page: https://github.com/Hermann-web/opencf-core
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
```

