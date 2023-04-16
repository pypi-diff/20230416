# Comparing `tmp/ach-file-0.1.5b0.tar.gz` & `tmp/ach-file-0.1.6b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ach-file-0.1.5b0.tar", last modified: Sat Nov 12 22:33:57 2022, max compression
+gzip compressed data, was "ach-file-0.1.6b0.tar", last modified: Sun Apr 16 06:22:01 2023, max compression
```

## Comparing `ach-file-0.1.5b0.tar` & `ach-file-0.1.6b0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/
--rw-r--r--   0 molly     (1000) molly     (1000)     1065 2022-11-11 00:19:34.000000 ach-file-0.1.5b0/LICENSE
--rw-r--r--   0 molly     (1000) molly     (1000)     6056 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/PKG-INFO
--rw-r--r--   0 molly     (1000) molly     (1000)     5565 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/README.md
-drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/ach/
--rw-r--r--   0 molly     (1000) molly     (1000)      126 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/__init__.py
--rw-r--r--   0 molly     (1000) molly     (1000)     3923 2022-11-12 22:33:32.000000 ach-file-0.1.5b0/ach/constants.py
-drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/ach/files/
--rw-r--r--   0 molly     (1000) molly     (1000)      279 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/files/__init__.py
--rw-r--r--   0 molly     (1000) molly     (1000)     9622 2022-11-12 22:33:32.000000 ach-file-0.1.5b0/ach/files/file_builder.py
--rw-r--r--   0 molly     (1000) molly     (1000)     6716 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/files/file_parser.py
--rw-r--r--   0 molly     (1000) molly     (1000)    14342 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/files/file_structure.py
-drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/ach/record_types/
--rw-r--r--   0 molly     (1000) molly     (1000)      762 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/__init__.py
--rw-r--r--   0 molly     (1000) molly     (1000)     1471 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/addenda.py
--rw-r--r--   0 molly     (1000) molly     (1000)     1734 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/batch_control.py
--rw-r--r--   0 molly     (1000) molly     (1000)     2832 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/batch_header.py
--rw-r--r--   0 molly     (1000) molly     (1000)     2599 2022-11-12 21:57:10.000000 ach-file-0.1.5b0/ach/record_types/entry_detail.py
--rw-r--r--   0 molly     (1000) molly     (1000)     1269 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/file_control.py
--rw-r--r--   0 molly     (1000) molly     (1000)     2851 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/file_header.py
--rw-r--r--   0 molly     (1000) molly     (1000)    13816 2022-11-12 21:22:32.000000 ach-file-0.1.5b0/ach/record_types/record_fields.py
--rw-r--r--   0 molly     (1000) molly     (1000)     7371 2022-11-12 19:51:05.000000 ach-file-0.1.5b0/ach/record_types/record_type_base.py
-drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/ach_file.egg-info/
--rw-r--r--   0 molly     (1000) molly     (1000)     6056 2022-11-12 22:33:57.000000 ach-file-0.1.5b0/ach_file.egg-info/PKG-INFO
--rw-r--r--   0 molly     (1000) molly     (1000)      581 2022-11-12 22:33:57.000000 ach-file-0.1.5b0/ach_file.egg-info/SOURCES.txt
--rw-r--r--   0 molly     (1000) molly     (1000)        1 2022-11-12 22:33:57.000000 ach-file-0.1.5b0/ach_file.egg-info/dependency_links.txt
--rw-r--r--   0 molly     (1000) molly     (1000)        4 2022-11-12 22:33:57.000000 ach-file-0.1.5b0/ach_file.egg-info/top_level.txt
--rw-r--r--   0 molly     (1000) molly     (1000)       38 2022-11-12 22:33:57.586938 ach-file-0.1.5b0/setup.cfg
--rw-r--r--   0 molly     (1000) molly     (1000)      702 2022-11-12 21:57:10.000000 ach-file-0.1.5b0/setup.py
+drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2023-04-16 06:22:01.415766 ach-file-0.1.6b0/
+-rw-r--r--   0 molly     (1000) molly     (1000)     1065 2022-11-11 00:19:34.000000 ach-file-0.1.6b0/LICENSE
+-rw-r--r--   0 molly     (1000) molly     (1000)     6056 2023-04-16 06:22:01.415766 ach-file-0.1.6b0/PKG-INFO
+-rw-r--r--   0 molly     (1000) molly     (1000)     5565 2022-11-12 19:51:05.000000 ach-file-0.1.6b0/README.md
+drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2023-04-16 06:22:01.405766 ach-file-0.1.6b0/ach/
+-rw-r--r--   0 molly     (1000) molly     (1000)      126 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/__init__.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     3927 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/constants.py
+drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2023-04-16 06:22:01.405766 ach-file-0.1.6b0/ach/files/
+-rw-r--r--   0 molly     (1000) molly     (1000)      279 2022-11-12 19:51:05.000000 ach-file-0.1.6b0/ach/files/__init__.py
+-rw-r--r--   0 molly     (1000) molly     (1000)    10468 2023-04-16 05:43:06.000000 ach-file-0.1.6b0/ach/files/file_builder.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     6898 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/files/file_parser.py
+-rw-r--r--   0 molly     (1000) molly     (1000)    14260 2023-04-16 04:35:59.000000 ach-file-0.1.6b0/ach/files/file_structure.py
+drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2023-04-16 06:22:01.415766 ach-file-0.1.6b0/ach/record_types/
+-rw-r--r--   0 molly     (1000) molly     (1000)      788 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/__init__.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     1679 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/addenda.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     1979 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/batch_control.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     3361 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/batch_header.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     2948 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/entry_detail.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     1402 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/file_control.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     3411 2023-04-16 04:48:47.000000 ach-file-0.1.6b0/ach/record_types/file_header.py
+-rw-r--r--   0 molly     (1000) molly     (1000)    14238 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/record_fields.py
+-rw-r--r--   0 molly     (1000) molly     (1000)     7585 2023-02-15 06:29:46.000000 ach-file-0.1.6b0/ach/record_types/record_type_base.py
+drwxr-xr-x   0 molly     (1000) molly     (1000)        0 2023-04-16 06:22:01.415766 ach-file-0.1.6b0/ach_file.egg-info/
+-rw-r--r--   0 molly     (1000) molly     (1000)     6056 2023-04-16 06:22:01.000000 ach-file-0.1.6b0/ach_file.egg-info/PKG-INFO
+-rw-r--r--   0 molly     (1000) molly     (1000)      581 2023-04-16 06:22:01.000000 ach-file-0.1.6b0/ach_file.egg-info/SOURCES.txt
+-rw-r--r--   0 molly     (1000) molly     (1000)        1 2023-04-16 06:22:01.000000 ach-file-0.1.6b0/ach_file.egg-info/dependency_links.txt
+-rw-r--r--   0 molly     (1000) molly     (1000)        4 2023-04-16 06:22:01.000000 ach-file-0.1.6b0/ach_file.egg-info/top_level.txt
+-rw-r--r--   0 molly     (1000) molly     (1000)       38 2023-04-16 06:22:01.415766 ach-file-0.1.6b0/setup.cfg
+-rw-r--r--   0 molly     (1000) molly     (1000)      702 2023-04-16 06:21:48.000000 ach-file-0.1.6b0/setup.py
```

### Comparing `ach-file-0.1.5b0/LICENSE` & `ach-file-0.1.6b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ach-file-0.1.5b0/PKG-INFO` & `ach-file-0.1.6b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ach-file
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: Highly configurable and permissive library to generate ACH files
 Home-page: https://github.com/freemish/ach-file
 Author: Molly Gouletas
 Author-email: molly.gouletas@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ach-file-0.1.5b0/README.md` & `ach-file-0.1.6b0/README.md`

 * *Files identical despite different names*

### Comparing `ach-file-0.1.5b0/ach/constants.py` & `ach-file-0.1.6b0/ach/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 class BatchServiceClassCode(enum.IntEnum):
     """
     Represents whether a batch contains only credits,
     only debits, or both.
     """
+
     MIXED = 200
     CREDITS = 220
     DEBITS = 225
 
     def __str__(self) -> str:
         return str(self.value)
 
@@ -19,14 +20,15 @@
 class TransactionCode(enum.IntEnum):
     """
     Represents type of transaction:
         - target is savings or checking account
         - action is crediting the account or debiting the account
         - whether is a dry-run (prenote) or is immediately effective
     """
+
     CHECKING_CREDIT = 22
     CHECKING_CREDIT_PRENOTE = 23
     CHECKING_DEBIT = 27
     CHECKING_DEBIT_PRENOTE = 28
     SAVINGS_CREDIT = 32
     SAVINGS_CREDIT_PRENOTE = 33
     SAVINGS_DEBIT = 37
@@ -38,15 +40,15 @@
 
     # pylint: disable=attribute-defined-outside-init
     @classmethod
     def _create_pseudo_member_(cls, value):
         pseudo_member = cls._value2member_map_.get(value, None)
         if pseudo_member is None:
             new_member = int.__new__(cls, value)
-            new_member._name_ = f'UNKNOWN_{value}'
+            new_member._name_ = f"UNKNOWN_{value}"
             new_member._value_ = value
             pseudo_member = cls._value2member_map_.setdefault(value, new_member)
         return pseudo_member
 
     def __str__(self) -> str:
         return str(self.value)
 
@@ -73,14 +75,15 @@
 
 class BatchStandardEntryClassCode(enum.Enum):
     """
     Represents one of several common SEC codes.
     See this site for more details:
     https://achdevguide.nacha.org/ach-file-details
     """
+
     PPD = enum.auto()
     ARC = enum.auto()
     BOC = enum.auto()
     CCD = enum.auto()
     CIE = enum.auto()
     CTX = enum.auto()
     IAT = enum.auto()
@@ -100,14 +103,15 @@
 
 class AutoDateInput(enum.Enum):
     """
     If values "NOW" or "TOMORROW"
     are put into a DateFieldType or TimeFieldType Field,
     the Field will autogenerate a date given today's datetime.
     """
+
     NOW = enum.auto()
     TOMORROW = enum.auto()
 
     # pylint: disable=invalid-overridden-method
     @property
     def value(self) -> str:
         return self.name
@@ -116,15 +120,15 @@
         return self.name
 
 
 RECORD_SIZE = 94
 
 FILE_HEADER_RECORD_TYPE_CODE = 1
 FILE_HEADER_PRIORITY_CODE = 1
-FILE_HEADER_DEFAULT_FILE_ID_MODIFIER = 'A'
+FILE_HEADER_DEFAULT_FILE_ID_MODIFIER = "A"
 FILE_HEADER_BLOCKING_FACTOR = 10
 FILE_HEADER_FORMAT_CODE = 1
 
 BATCH_HEADER_RECORD_TYPE_CODE = 5
 BATCH_DEFAULT_SERVICE_CLASS_CODE = BatchServiceClassCode.MIXED
 BATCH_HEADER_DEFAULT_STANDARD_ENTRY_CLASS_CODE = BatchStandardEntryClassCode.PPD
 BATCH_HEADER_DEFAULT_ORIGINATOR_STATUS_CODE = 1
```

### Comparing `ach-file-0.1.5b0/ach/files/file_builder.py` & `ach-file-0.1.6b0/ach/files/file_builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 """Defines an ACH file builder."""
 
 from typing import Any, Dict, List, Tuple
 
 from ..record_types import (
-    AddendaRecordType, BatchHeaderRecordType,
-    EntryDetailRecordType, FieldDefinition,
-    FileHeaderRecordType
+    AddendaRecordType,
+    BatchHeaderRecordType,
+    EntryDetailRecordType,
+    FieldDefinition,
+    FileHeaderRecordType,
 )
 from .file_structure import ACHBatch, ACHFileContents, ACHTransactionEntry
 
 
 class NoBatchForTransactionError(Exception):
     """
     Raise when no batches have been added before adding
     a transaction entry to the ACHFileBuilder.
     """
 
 
 class ACHFileBuilder:
     """Builds an ACHFileContents object."""
 
+    ach_file_contents_class = ACHFileContents
+    ach_batch_class = ACHBatch
+    ach_transaction_entry_class = ACHTransactionEntry
+    file_header_record_type_class = FileHeaderRecordType
+    batch_header_record_type_class = BatchHeaderRecordType
+    entry_detail_record_type_class = EntryDetailRecordType
+    addenda_record_type_class = AddendaRecordType
+
     def __init__(self, **file_settings):
         """
         Accepts a dict of file settings.
         Run cls.get_file_setting_fields to see all key options.
 
         Examples:
 
@@ -39,38 +49,45 @@
             ACHFileBuilder(
                 destination_routing='012345678',
                 origin_routing='102345678',
                 destination_name='YOUR BANK',
                 origin_name='YOUR FINANCIAL INSTITUTION',
             )
         """
-        self.ach_file_contents: ACHFileContents = ACHFileContents(
-            FileHeaderRecordType(**file_settings))
-        self.default_odfi_identification: str = file_settings.get('origin_routing', '').lstrip()[:8]
+        self.ach_file_contents: ACHFileContents = self.ach_file_contents_class(
+            self.file_header_record_type_class(**file_settings)
+        )
+        self.default_odfi_identification: str = file_settings.get(
+            "origin_routing", ""
+        ).lstrip()[:8]
 
-    def render(self, line_break: str = '\n', end: str = '\n') -> str:
+    def render(self, line_break: str = "\n", end: str = "\n") -> str:
         """Renders ACH flat file contents as a string."""
-        return self.ach_file_contents.render_file_contents(line_break=line_break, end=end)
+        return self.ach_file_contents.render_file_contents(
+            line_break=line_break, end=end
+        )
 
-    def add_batch(self, **batch_settings: Dict[str, Any]) -> 'ACHFileBuilder':
+    def add_batch(self, **batch_settings: Dict[str, Any]) -> "ACHFileBuilder":
         """
         Accepts a dict of batch settings.
         See cls.get_batch_fields to see all options.
 
         Example:
             b.add_batch(
                 company_name='YOUR COMPANY',
                 company_identification='1234567890',
                 standard_entry_class_code='CCD',
                 company_entry_description='Bonus',
                 effective_entry_date='NOW',
             )
         """
         self._update_batch_settings(batch_settings)
-        self.ach_file_contents.add_batch(ACHBatch(BatchHeaderRecordType(**batch_settings)))
+        self.ach_file_contents.add_batch(
+            self.ach_batch_class(self.batch_header_record_type_class(**batch_settings))
+        )
         return self
 
     def add_entries_and_addendas(
         self,
         entry_dict_list: List[Dict[str, Any]],
         batch_index: int = -1,
         raise_exc: bool = True,
@@ -119,15 +136,17 @@
                 self.add_entry_and_addenda(batch_index=batch_index, **entry_dict)
             except Exception as exc:
                 if raise_exc:
                     raise exc from exc
                 failed_entry_dicts_and_excs.append((entry_dict, exc))
         return failed_entry_dicts_and_excs
 
-    def add_entry_and_addenda(self, batch_index: int = -1, **entry_details) -> 'ACHFileBuilder':
+    def add_entry_and_addenda(
+        self, batch_index: int = -1, **entry_details
+    ) -> "ACHFileBuilder":
         """
         Adds single entry and its addenda(s) to a batch.
         Raises NoBatchForTransactionError or IndexError if batch index specified does not exist.
 
         Example:
             b.add_entry_and_addenda(
                 transaction_code=22,
@@ -135,118 +154,136 @@
                 rdfi_account_number='45454545',
                 amount=2000,
                 individual_name='Tester Testerson',
                 addendas=[{'payment_related_information': 'This is a memo'}],
             )
         """
         if not self.ach_file_contents.batches:
-            raise NoBatchForTransactionError("Must add batch before adding transaction entries")
+            raise NoBatchForTransactionError(
+                "Must add batch before adding transaction entries"
+            )
 
-        ach_tx_entry = self._convert_entry_detail_kwargs_to_ach_transaction_entry(**entry_details)
+        ach_tx_entry = self._convert_entry_detail_kwargs_to_ach_transaction_entry(
+            **entry_details
+        )
         self.ach_file_contents.batches[batch_index].add_transaction(ach_tx_entry)
         return self
 
     def _update_batch_settings(self, batch_settings: Dict[str, Any]) -> None:
         update_batch_settings = {
-            'odfi_identification': self.default_odfi_identification,
-            'batch_number': len(self.ach_file_contents.batches) + 1,
+            "odfi_identification": self.default_odfi_identification,
+            "batch_number": len(self.ach_file_contents.batches) + 1,
         }
         for k, val in update_batch_settings.items():
             if k not in batch_settings:
                 batch_settings[k] = val
 
     def _convert_entry_detail_kwargs_to_ach_transaction_entry(
-        self,
-        **entry_details
+        self, **entry_details
     ) -> ACHTransactionEntry:
         addenda_list_kwargs = self._update_entry_detail_kwargs(entry_details)
 
-        entry_record = EntryDetailRecordType(**entry_details)
+        entry_record = self.entry_detail_record_type_class(**entry_details)
         addenda_records = []
 
         for i, addenda_kwargs in enumerate(addenda_list_kwargs):
             self._update_addenda_record_kwargs(
                 addenda_kwargs,
-                entry_details.get('trace_sequence_number'),
-                addenda_sequence_num=i+1,
+                entry_details.get("trace_sequence_number"),
+                addenda_sequence_num=i + 1,
             )
-            addenda_records.append(AddendaRecordType(**addenda_kwargs))
+            addenda_records.append(self.addenda_record_type_class(**addenda_kwargs))
 
-        return ACHTransactionEntry(entry_record, addenda_records)
+        return self.ach_transaction_entry_class(entry_record, addenda_records)
 
-    def _update_entry_detail_kwargs(self, entry_details: Dict[str, Any]) -> List[Dict[str, Any]]:
+    def _update_entry_detail_kwargs(
+        self, entry_details: Dict[str, Any]
+    ) -> List[Dict[str, Any]]:
         raw_addendas = []
-        if 'addendas' in entry_details:
-            raw_addendas = entry_details.pop('addendas')
+        if "addendas" in entry_details:
+            raw_addendas = entry_details.pop("addendas")
 
         update_entry = {
-            'addenda_record_indicator': len(raw_addendas),
-            'trace_odfi_identifier': self.default_odfi_identification,
-            'trace_sequence_number': len(
-                self.ach_file_contents.get_all_transactions()) + 1,
+            "addenda_record_indicator": len(raw_addendas),
+            "trace_odfi_identifier": self.default_odfi_identification,
+            "trace_sequence_number": len(self.ach_file_contents.get_all_transactions())
+            + 1,
         }
         for k, val in update_entry.items():
             if k not in entry_details:
                 entry_details[k] = val
         return raw_addendas
 
     def _update_addenda_record_kwargs(
         self,
         addenda_kwargs: Dict[str, Any],
         entry_detail_sequence_num: int,
         addenda_sequence_num: int,
     ) -> None:
         update_entry = {
-            'entry_detail_sequence_number': entry_detail_sequence_num,
-            'addenda_sequence_number': addenda_sequence_num,
+            "entry_detail_sequence_number": entry_detail_sequence_num,
+            "addenda_sequence_number": addenda_sequence_num,
         }
         for k, val in update_entry.items():
             if k not in addenda_kwargs:
                 addenda_kwargs[k] = val
 
-    @staticmethod
-    def get_file_setting_fields(only_required: bool = False) -> Dict[str, FieldDefinition]:
+    @classmethod
+    def get_file_setting_fields(
+        cls,
+        only_required: bool = False,
+    ) -> Dict[str, FieldDefinition]:
         """
         Returns kwargs to pass into init.
         If only_required, returns only keywords that need to be set.
         """
         if only_required:
-            return FileHeaderRecordType.get_required_kwargs()
-        return FileHeaderRecordType.field_definition_dict
+            return cls.file_header_record_type_class.get_required_kwargs()
+        return cls.file_header_record_type_class.field_definition_dict
 
-    @staticmethod
-    def get_batch_fields(only_required: bool = False) -> Dict[str, FieldDefinition]:
+    @classmethod
+    def get_batch_fields(
+        cls, only_required: bool = False
+    ) -> Dict[str, FieldDefinition]:
         """
         Returns kwargs to pass into init.
         If only_required, returns only keywords that need to be set.
         """
         if only_required:
-            required_kwargs = dict(BatchHeaderRecordType.get_required_kwargs())
-            required_kwargs.pop('odfi_identification')
-            required_kwargs.pop('batch_number')
+            required_kwargs = dict(
+                cls.batch_header_record_type_class.get_required_kwargs()
+            )
+            required_kwargs.pop("odfi_identification")
+            required_kwargs.pop("batch_number")
             return required_kwargs
-        return BatchHeaderRecordType.field_definition_dict
+        return cls.batch_header_record_type_class.field_definition_dict
 
-    @staticmethod
-    def get_entry_fields(only_required: bool = False) -> Dict[str, FieldDefinition]:
+    @classmethod
+    def get_entry_fields(
+        cls, only_required: bool = False
+    ) -> Dict[str, FieldDefinition]:
         """
         Returns kwargs to pass into init.
         If only_required, returns only keywords that need to be set.
         """
         if only_required:
-            required_kwargs = dict(EntryDetailRecordType.get_required_kwargs())
-            required_kwargs.pop('trace_odfi_identifier')
-            required_kwargs.pop('trace_sequence_number')
+            required_kwargs = dict(
+                cls.entry_detail_record_type_class.get_required_kwargs()
+            )
+            required_kwargs.pop("trace_odfi_identifier")
+            required_kwargs.pop("trace_sequence_number")
             return required_kwargs
-        return EntryDetailRecordType.field_definition_dict
+        return cls.entry_detail_record_type_class.field_definition_dict
 
-    @staticmethod
-    def get_addenda_fields(only_required: bool = False) -> Dict[str, FieldDefinition]:
+    @classmethod
+    def get_addenda_fields(
+        cls, only_required: bool = False
+    ) -> Dict[str, FieldDefinition]:
         """
         Returns kwargs to pass into init.
         If only_required, returns only keywords that need to be set.
         """
         if only_required:
-            required_kwargs = dict(AddendaRecordType.get_required_kwargs())
-            required_kwargs.pop('entry_detail_sequence_number')
+            required_kwargs = dict(cls.addenda_record_type_class.get_required_kwargs())
+            required_kwargs.pop("entry_detail_sequence_number")
             return required_kwargs
-        return AddendaRecordType.field_definition_dict
+        return cls.addenda_record_type_class.field_definition_dict
```

### Comparing `ach-file-0.1.5b0/ach/files/file_parser.py` & `ach-file-0.1.6b0/ach/files/file_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 """Defines an ACH file parser."""
 
 from typing import Dict, List, Optional, Union
 
 from .file_structure import ACHBatch, ACHFileContents, ACHTransactionEntry
 from ..record_types import (
-    AddendaRecordType, BatchControlRecordType,
-    BatchHeaderRecordType, EntryDetailRecordType,
-    FileControlRecordType, FileHeaderRecordType
+    AddendaRecordType,
+    BatchControlRecordType,
+    BatchHeaderRecordType,
+    EntryDetailRecordType,
+    FileControlRecordType,
+    FileHeaderRecordType,
 )
 from ..record_types.record_type_base import RecordType
 from ..constants import (
     ADDENDA_RECORD_TYPE_CODE,
     BATCH_CONTROL_RECORD_TYPE_CODE,
     BATCH_HEADER_RECORD_TYPE_CODE,
     ENTRY_DETAIL_RECORD_TYPE_CODE,
     FILE_CONTROL_RECORD_TYPE_CODE,
     FILE_HEADER_RECORD_TYPE_CODE,
-    RECORD_SIZE
+    RECORD_SIZE,
 )
 
 
 class ACHFileContentsParser:
     """
     Accepts a raw ACH file as a string.
     Can return a list of RecordType types
     and an ACHFileContents type.
     """
+
     def __init__(self, ach_file_str: str):
         self._raw_str = ach_file_str
 
     def process_records_list(self) -> List[RecordType]:
         """Processes raw ACH file string into a list of RecordTypes in order."""
         return self.convert_file_string_to_records_list(self._raw_str)
 
     def process_ach_file_contents(
         self,
         records_list: Optional[List[RecordType]] = None,
     ) -> ACHFileContents:
         """Processes a list of RecordTypes into an ACHFileContents."""
         return self.convert_records_list_to_ach_file_contents(
-            records_list or self.process_records_list())
+            records_list or self.process_records_list()
+        )
 
     @staticmethod
     def convert_records_list_to_ach_file_contents(
         records_list: List[RecordType],
         recalc_control_records: bool = False,
     ) -> ACHFileContents:
         """Converts list of RecordTypes to ACHFileContents type."""
@@ -62,29 +67,31 @@
     def _convert_sub_records_list_to_ach_batch_list(
         records_list: List[RecordType],
         recalc_batch_control: bool = False,
     ) -> List[ACHBatch]:
         ach_batch_list: List[ACHBatch] = []
         batch_to_records: Dict[
             BatchControlRecordType,
-            List[Union[EntryDetailRecordType, AddendaRecordType]]
+            List[Union[EntryDetailRecordType, AddendaRecordType]],
         ] = {}
         curr_batch_header: Optional[BatchHeaderRecordType] = None
         for record in records_list:
-            if (record.get_field_value('record_type_code')
-                == str(BATCH_HEADER_RECORD_TYPE_CODE)
+            if record.get_field_value("record_type_code") == str(
+                BATCH_HEADER_RECORD_TYPE_CODE
             ):
                 curr_batch_header = record
                 batch_to_records[curr_batch_header] = []
                 continue
-            if (record.get_field_value('record_type_code')
-                == str(BATCH_CONTROL_RECORD_TYPE_CODE)
+            if record.get_field_value("record_type_code") == str(
+                BATCH_CONTROL_RECORD_TYPE_CODE
             ):
                 # pylint: disable=line-too-long
-                tx_entries = ACHFileContentsParser._convert_batch_transaction_record_types_to_ach_transaction_entry_list(batch_to_records[curr_batch_header])
+                tx_entries = ACHFileContentsParser._convert_batch_transaction_record_types_to_ach_transaction_entry_list(
+                    batch_to_records[curr_batch_header]
+                )
                 ach_batch = ACHBatch(curr_batch_header, tx_entries)
                 if not recalc_batch_control:
                     ach_batch.batch_control_record = record
                 ach_batch_list.append(ach_batch)
                 continue
             batch_to_records[curr_batch_header].append(record)
         return ach_batch_list
@@ -93,26 +100,30 @@
     def _convert_batch_transaction_record_types_to_ach_transaction_entry_list(
         records_list: List[Union[EntryDetailRecordType, AddendaRecordType]],
     ) -> List[ACHTransactionEntry]:
         entries: List[ACHTransactionEntry] = []
         curr_entry: Optional[EntryDetailRecordType] = None
         curr_entry_addendas: List[AddendaRecordType] = []
         for record in records_list:
-            if record.get_field_value('record_type_code') == str(ADDENDA_RECORD_TYPE_CODE):
+            if record.get_field_value("record_type_code") == str(
+                ADDENDA_RECORD_TYPE_CODE
+            ):
                 curr_entry_addendas.append(record)
                 continue
             if curr_entry:
                 entries.append(ACHTransactionEntry(curr_entry, curr_entry_addendas))
             curr_entry = record
             curr_entry_addendas = []
 
         entries.append(ACHTransactionEntry(curr_entry, curr_entry_addendas))
         return entries
 
-    def get_record_fields_dict_list(self, records_list: List[RecordType]) -> List[Dict[str, str]]:
+    def get_record_fields_dict_list(
+        self, records_list: List[RecordType]
+    ) -> List[Dict[str, str]]:
         """
         Returns records list as list of dictionaries (field names: clean values).
         """
         dict_list = []
         for record in records_list:
             dict_list.append({x: y.value for x, y in record.fields.items()})
         return dict_list
@@ -132,38 +143,44 @@
             ENTRY_DETAIL_RECORD_TYPE_CODE: EntryDetailRecordType,
             FILE_CONTROL_RECORD_TYPE_CODE: FileControlRecordType,
             FILE_HEADER_RECORD_TYPE_CODE: FileHeaderRecordType,
         }
         return record_type_map.get(int(record_type_code))
 
     @staticmethod
-    def convert_line_to_record_type(line_str: str, record_type_class: RecordType) -> RecordType:
+    def convert_line_to_record_type(
+        line_str: str, record_type_class: RecordType
+    ) -> RecordType:
         """
         Converts a line in an ACH record to a RecordType according to its
         leading record type code.
         """
         str_index = 0
         kwargs = {}
         for key, field_def in record_type_class.field_definition_dict.items():
-            kwargs[key] = line_str[str_index: str_index + field_def.length]
+            kwargs[key] = line_str[str_index : str_index + field_def.length]
             str_index += field_def.length
         return record_type_class(**kwargs)
 
     @staticmethod
     def convert_file_string_to_records_list(
         file_str: str,
-        line_break: str = '\n',
+        line_break: str = "\n",
     ) -> List[RecordType]:
         """
         Splits a file string along line breaks
         and initializes each line as a RecordType.
         Returns list of RecordTypes.
         """
         lines = file_str.split(line_break)
         records = []
         for line in lines:
-            if not line or line == '9' * RECORD_SIZE:
+            if not line or line == "9" * RECORD_SIZE:
                 continue
-            record_type_class = ACHFileContentsParser.get_record_type_from_record_type_code(line[0])
-            record_type = ACHFileContentsParser.convert_line_to_record_type(line, record_type_class)
+            record_type_class = (
+                ACHFileContentsParser.get_record_type_from_record_type_code(line[0])
+            )
+            record_type = ACHFileContentsParser.convert_line_to_record_type(
+                line, record_type_class
+            )
             records.append(record_type)
         return records
```

### Comparing `ach-file-0.1.5b0/ach/files/file_structure.py` & `ach-file-0.1.6b0/ach/files/file_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,109 +1,111 @@
 """Defines ACH file structure and how record types relate."""
 
 from math import ceil
 from typing import Any, Dict, List, Optional, Tuple
 
 from ..constants import FILE_HEADER_BLOCKING_FACTOR, RECORD_SIZE, TransactionCode
 from ..record_types import (
-    AddendaRecordType, BatchControlRecordType,
-    BatchHeaderRecordType, EntryDetailRecordType,
-    FileControlRecordType, FileHeaderRecordType
+    AddendaRecordType,
+    BatchControlRecordType,
+    BatchHeaderRecordType,
+    EntryDetailRecordType,
+    FileControlRecordType,
+    FileHeaderRecordType,
 )
 
 
 class ACHFileContents:
     """
     Contains 1 FileHeaderRecordType, 1 FileControlRecord, and n ACHBatch.
 
     Attributes:
         file_header_record: FileHeaderRecordType
         batches: List[ACHBatch]
         [computed property] file_control_record: FileControlRecordType
     """
+
     def __init__(
         self,
         file_header_record: FileHeaderRecordType,
-        batches: Optional[List['ACHBatch']] = None,
+        batches: Optional[List["ACHBatch"]] = None,
     ):
         self._file_header_record = file_header_record
         self.batches = batches or []
         self._file_control_record = None
         self._recalc_file_control = False
 
     def get_rendered_line_list(self) -> List[str]:
         """Get rendered lines of an ACH file as an unjoined list."""
         record_types_list = [self.file_header_record.render_record_line()]
         for batch in self.batches:
             record_types_list.extend(batch.get_rendered_line_list())
         record_types_list.append(self.file_control_record.render_record_line())
         return record_types_list
 
-    def render_file_contents(self, line_break: str = '\n', end: str = '\n') -> str:
+    def render_file_contents(self, line_break: str = "\n", end: str = "\n") -> str:
         """
         Render all records in ACHFileContents as a single flat-file string.
         """
         rendered_line_list = self.get_rendered_line_list()
         file_contents = line_break.join(rendered_line_list)
 
         block_orphan_count = len(rendered_line_list) % FILE_HEADER_BLOCKING_FACTOR
         if block_orphan_count:
             for _ in range(FILE_HEADER_BLOCKING_FACTOR - block_orphan_count):
-                file_contents += line_break + ('9' * RECORD_SIZE)
+                file_contents += line_break + ("9" * RECORD_SIZE)
 
         return file_contents + end
 
     def render_json_dict(self) -> Dict[str, Any]:
         """
         Render all records as dictionaries of their valid field values.
         """
         file_as_json_dict = {
-            'file_header': self.file_header_record.get_field_values(),
-            'batches': [
-                b.get_json_dict() for b in self.batches
-            ],
-            'file_control': self.file_control_record.get_field_values(),
+            "file_header": self.file_header_record.get_field_values(),
+            "batches": [b.get_json_dict() for b in self.batches],
+            "file_control": self.file_control_record.get_field_values(),
         }
         return file_as_json_dict
 
     @property
     def file_header_record(self) -> FileHeaderRecordType:
         """Get FileHeaderRecordType."""
         return self._file_header_record
 
     @file_header_record.setter
     def file_header_record(self, file_header_record: FileHeaderRecordType) -> None:
         """
         If file header record is changed when file control has already
         been calculated, recalculate file control.
         """
-        self.file_header_record = file_header_record
+        self._file_header_record = file_header_record
         if self._file_control_record:
             self._recalc_file_control = True
 
-    def add_batch(self, batch: 'ACHBatch') -> None:
+    def add_batch(self, batch: "ACHBatch") -> None:
         """
         Add an ACHBatch to ACHFileContents.
         If file control has already been calculated, recalculate.
         """
         self.batches.append(batch)
         if self._file_control_record:
             self._recalc_file_control = True
 
-    def remove_batch_by_index(self, index: int) -> 'ACHBatch':
+    def remove_batch_by_index(self, index: int) -> "ACHBatch":
         """
         Remove an ACHBatch from ACHFileContents.
         If file control has already been calculated, recalculate.
         """
         batch = self.batches.pop(index)
         if self._file_control_record:
             self._recalc_file_control = True
         return batch
 
-    def get_all_transactions(self) -> List['ACHTransactionEntry']:
+    def get_all_transactions(self) -> List["ACHTransactionEntry"]:
         """
         Get all ACHTransactionEntry objects across all batches.
         """
         txs = []
         for batch in self.batches:
             txs.extend(batch.transactions)
         return txs
@@ -137,21 +139,21 @@
             entry_hash=self._compute_entry_hash(),
             total_credit_amount=credit_total,
             total_debit_amount=debit_total,
         )
 
     def _compute_entry_and_addenda_count(self) -> int:
         return sum(
-            int(x.batch_control_record.get_field_value('entry_and_addenda_count'))
+            int(x.batch_control_record.get_field_value("entry_and_addenda_count"))
             for x in self.batches
         )
 
     def _compute_entry_hash(self) -> int:
         return sum(
-            int(x.batch_control_record.get_field_value('entry_hash'))
+            int(x.batch_control_record.get_field_value("entry_hash"))
             for x in self.batches
         )
 
     def _compute_line_count(self, entry_addenda_count: Optional[int] = None) -> int:
         if entry_addenda_count is None:
             entry_addenda_count = self._compute_entry_and_addenda_count()
         return entry_addenda_count + (len(self.batches) * 2) + 2
@@ -159,42 +161,46 @@
     def _compute_block_count(
         self,
         line_count: Optional[int] = None,
         entry_addenda_count: Optional[int] = None,
     ) -> int:
         if line_count is None:
             line_count = self._compute_line_count(entry_addenda_count)
-        return ceil(line_count / float(FILE_HEADER_BLOCKING_FACTOR))
+        return ceil(
+            line_count
+            / float(self.file_header_record.get_field_value("blocking_factor"))
+        )
 
     def _compute_debit_and_credit_totals(self) -> Tuple[int, int]:
         debit_sum, credit_sum = 0, 0
         debit_sum = sum(
-            int(x.batch_control_record.get_field_value('total_debit_amount'))
+            int(x.batch_control_record.get_field_value("total_debit_amount"))
             for x in self.batches
         )
         credit_sum = sum(
-            int(x.batch_control_record.get_field_value('total_credit_amount'))
+            int(x.batch_control_record.get_field_value("total_credit_amount"))
             for x in self.batches
         )
         return debit_sum, credit_sum
 
 
 class ACHBatch:
     """
     Contains 1 BatchHeaderRecordType, 1 BatchControlRecordType, and n ACHTransactionEntry.
 
     Attributes:
         batch_header_record: BatchHeaderRecordType
         transactions: List[ACHTransactionEntry]
         [computed + cached property] batch_control_record: BatchControlRecordType
     """
+
     def __init__(
         self,
         batch_header_record: BatchHeaderRecordType,
-        transactions: Optional[List['ACHTransactionEntry']] = None,
+        transactions: Optional[List["ACHTransactionEntry"]] = None,
     ):
         self._batch_header_record = batch_header_record
         self.transactions = transactions or []
         self._batch_control_record: BatchControlRecordType = None
         self._recalc_batch_control = False
 
     @property
@@ -208,24 +214,24 @@
         Sets a batch header record.
         If batch control has been computed, set to recalculate.
         """
         self._batch_header_record = batch_header_record
         if self._batch_control_record:
             self._recalc_batch_control = True
 
-    def add_transaction(self, transaction: 'ACHTransactionEntry') -> None:
+    def add_transaction(self, transaction: "ACHTransactionEntry") -> None:
         """
         Adds an ACHTransactionEntry to this ACHBatch.
         If batch control has been computed, set to recalculate.
         """
         self.transactions.append(transaction)
         if self._batch_control_record:
             self._recalc_batch_control = True
 
-    def remove_transaction_by_index(self, index: int) -> 'ACHTransactionEntry':
+    def remove_transaction_by_index(self, index: int) -> "ACHTransactionEntry":
         """
         Removes an ACHTransactionEntry by index.
         If batch control has been computed, set to recalculate.
         """
         transaction = self.transactions.pop(index)
         if self._batch_control_record:
             self._recalc_batch_control = True
@@ -236,15 +242,17 @@
         """Get batch control record."""
         if self._batch_control_record and not self._recalc_batch_control:
             return self._batch_control_record
         self._batch_control_record = self._compute_batch_control_record()
         return self._batch_control_record
 
     @batch_control_record.setter
-    def batch_control_record(self, batch_control_record: BatchControlRecordType) -> None:
+    def batch_control_record(
+        self, batch_control_record: BatchControlRecordType
+    ) -> None:
         """For use by file parser."""
         self._batch_control_record = batch_control_record
 
     def get_rendered_line_list(self) -> List[str]:
         """
         Get list of rendered RecordTypes as single-line strings
         contained in this ACHBatch.
@@ -257,37 +265,37 @@
 
     def get_json_dict(self) -> Dict[str, Any]:
         """
         Get JSON dict representing all contained RecordTypes as dicts
         mapped from field names to their valid values.
         """
         batch_dict = {
-            'batch_header': self._batch_header_record.get_field_values(),
-            'transactions': [
-                t.get_json_dict() for t in self.transactions
-            ],
-            'batch_control': self.batch_control_record.get_field_values(),
+            "batch_header": self._batch_header_record.get_field_values(),
+            "transactions": [t.get_json_dict() for t in self.transactions],
+            "batch_control": self.batch_control_record.get_field_values(),
         }
         return batch_dict
 
     def _compute_batch_control_record(self) -> BatchControlRecordType:
         debit_total, credit_total = self._compute_debit_and_credit_totals()
         return BatchControlRecordType(
             entry_and_addenda_count=self._compute_entry_and_addenda_count(),
             entry_hash=self._compute_entry_hash(),
             total_debit_amount=debit_total,
             total_credit_amount=credit_total,
             service_class_code=self._batch_header_record.get_field_value(
-                'service_class_code'),
+                "service_class_code"
+            ),
             company_identification=self._batch_header_record.get_field_value(
-                'company_identification'),
+                "company_identification"
+            ),
             odfi_identification=self._batch_header_record.get_field_value(
-                'odfi_identification'),
-            batch_number=self._batch_header_record.get_field_value(
-                'batch_number'),
+                "odfi_identification"
+            ),
+            batch_number=self._batch_header_record.get_field_value("batch_number"),
         )
 
     def _compute_entry_hash(self) -> int:
         return sum(x.get_entry_hash_int() for x in self.transactions)
 
     def _compute_entry_and_addenda_count(self) -> int:
         return sum(x.get_entry_and_addenda_count() for x in self.transactions)
@@ -302,14 +310,15 @@
     """
     Contains 1 entry detail record and 0-n addendas associated with that record.
 
     Attributes:
         entry: EntryDetailRecordType
         addendas: List[AddendaRecordType]
     """
+
     def __init__(
         self,
         entry: EntryDetailRecordType,
         addendas: Optional[List[AddendaRecordType]] = None,
     ):
         self._entry = entry
         self.addendas = addendas or []
@@ -333,55 +342,44 @@
         """
         return len(self.addendas) + 1
 
     def get_entry_hash_int(self) -> int:
         """
         Return first 8 digits of RDFI routing number converted to int.
         """
-        return int(self._entry.get_field_value('rdfi_routing')[:8])
+        return int(self._entry.get_field_value("rdfi_routing")[:8])
 
     def get_transaction_code_enum(self) -> TransactionCode:
         """Return TransactionCode enum from transaction_code field."""
         return TransactionCode(int(self._entry.get_field_value("transaction_code")))
 
     def get_amount(self) -> int:
         """Return amount (of cents) as int from amount field."""
         return int(self._entry.get_field_value("amount"))
 
     def get_debit_amount(self) -> int:
         """Get amount if amount is a debit else 0."""
-        return (
-            self.get_amount()
-            if self.get_transaction_code_enum().is_debit()
-            else 0
-        )
+        return self.get_amount() if self.get_transaction_code_enum().is_debit() else 0
 
     def get_credit_amount(self) -> int:
         """Get amount if amount is a credit else 0."""
-        return (
-            self.get_amount()
-            if self.get_transaction_code_enum().is_credit()
-            else 0
-        )
+        return self.get_amount() if self.get_transaction_code_enum().is_credit() else 0
 
     def get_rendered_line_list(self) -> List[str]:
         """
         Get list of all contained RecordTypes rendered
         as single-line strings.
         """
-        return (
-            [self._entry.render_record_line()]
-            + [x.render_record_line() for x in self.addendas]
-        )
+        return [self._entry.render_record_line()] + [
+            x.render_record_line() for x in self.addendas
+        ]
 
     def get_json_dict(self) -> Dict[str, Any]:
         """
         Get JSON dict of all contained RecordTypes as
         field names mapped to valid field values.
         """
         tx_dict = {
-            'entry_detail': self._entry.get_field_values(),
-            'addendas': [
-                a.get_field_values() for a in self.addendas
-            ],
+            "entry_detail": self._entry.get_field_values(),
+            "addendas": [a.get_field_values() for a in self.addendas],
         }
         return tx_dict
```

### Comparing `ach-file-0.1.5b0/ach/record_types/__init__.py` & `ach-file-0.1.6b0/ach/record_types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,19 +3,25 @@
 from .addenda import AddendaRecordType
 from .batch_control import BatchControlRecordType
 from .batch_header import BatchHeaderRecordType
 from .entry_detail import EntryDetailRecordType
 from .file_control import FileControlRecordType
 from .file_header import FileHeaderRecordType
 from .record_fields import (
-    Alignment, AlphaNumFieldType,
-    BlankPaddedRoutingNumberFieldType, DateFieldType,
-    EmptyRequiredFieldError, Field, FieldDefinition,
-    FieldType, IntegerFieldType, TimeFieldType,
-    ValueMismatchesFieldTypeError
+    Alignment,
+    AlphaNumFieldType,
+    BlankPaddedRoutingNumberFieldType,
+    DateFieldType,
+    EmptyRequiredFieldError,
+    Field,
+    FieldDefinition,
+    FieldType,
+    IntegerFieldType,
+    TimeFieldType,
+    ValueMismatchesFieldTypeError,
 )
 from .record_type_base import (
     InvalidRecordSizeError,
     InvalidRecordTypeParametersError,
     RecordTypeAggregateFieldCreationError,
-    RecordType
+    RecordType,
 )
```

### Comparing `ach-file-0.1.5b0/ach/record_types/addenda.py` & `ach-file-0.1.6b0/ach/record_types/batch_control.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,50 @@
-"""Defines addenda fields and record type."""
+"""Defines batch control fields and record type."""
 
 from typing import Dict
 
-from ..constants import (
-    ADDENDA_DEFAULT_SEQUENCE_NUMBER,
-    ADDENDA_RECORD_TYPE_CODE,
-    ADDENDA_TYPE_CODE
-)
-from .record_fields import (
-    AlphaNumFieldType,
-    FieldDefinition,
-    IntegerFieldType
-)
+from ..constants import BATCH_CONTROL_RECORD_TYPE_CODE, BATCH_DEFAULT_SERVICE_CLASS_CODE
+from .record_fields import AlphaNumFieldType, FieldDefinition, IntegerFieldType
 from .record_type_base import RecordType
 
 
 # pylint: disable=line-too-long
-class AddendaRecordType(RecordType):
-    """Define all fields of an addenda record line of an ACH file."""
+class BatchControlRecordType(RecordType):
+    """Define all fields of a batch control record line of an ACH file."""
+
     field_definition_dict: Dict[str, FieldDefinition] = {
-        'record_type_code': FieldDefinition('Record Type Code', IntegerFieldType, length=1, default=ADDENDA_RECORD_TYPE_CODE),
-        'addenda_type_code': FieldDefinition('Addenda Type Code', IntegerFieldType, length=2, default=ADDENDA_TYPE_CODE),
-        'payment_related_information': FieldDefinition('Payment Related Information', AlphaNumFieldType, length=80, required=False),
-        'addenda_sequence_number': FieldDefinition('Addenda Sequence Number', IntegerFieldType, length=4, default=ADDENDA_DEFAULT_SEQUENCE_NUMBER),
-        'entry_detail_sequence_number': FieldDefinition('Entry Detail Sequence Number', IntegerFieldType, length=7),
+        "record_type_code": FieldDefinition(
+            "Record Type Code",
+            IntegerFieldType,
+            length=1,
+            default=BATCH_CONTROL_RECORD_TYPE_CODE,
+        ),
+        "service_class_code": FieldDefinition(
+            "Service Class Code",
+            IntegerFieldType,
+            length=3,
+            default=BATCH_DEFAULT_SERVICE_CLASS_CODE,
+        ),
+        "entry_and_addenda_count": FieldDefinition(
+            "Entry and Addenda Count", IntegerFieldType, length=6
+        ),
+        "entry_hash": FieldDefinition("Entry Hash", IntegerFieldType, length=10),
+        "total_debit_amount": FieldDefinition(
+            "Total Debit Amount", IntegerFieldType, length=12
+        ),
+        "total_credit_amount": FieldDefinition(
+            "Total Credit Amount", IntegerFieldType, length=12
+        ),
+        "company_identification": FieldDefinition(
+            "Company Identification", IntegerFieldType, length=10
+        ),
+        "message_authentication_code": FieldDefinition(
+            "Message Authentication Code", AlphaNumFieldType, length=19, required=False
+        ),
+        "reserved": FieldDefinition(
+            "Reserved Space", AlphaNumFieldType, length=6, required=False
+        ),
+        "odfi_identification": FieldDefinition(
+            "ODFI Identification (First 8 of Routing)", IntegerFieldType, length=8
+        ),
+        "batch_number": FieldDefinition("Batch Number", IntegerFieldType, length=7),
     }
-
-    def __init__(self, payment_related_information: str, entry_detail_sequence_number: int, **kwargs):
-        kwargs['payment_related_information'] = payment_related_information
-        kwargs['entry_detail_sequence_number'] = entry_detail_sequence_number
-        super().__init__(**kwargs)
```

### Comparing `ach-file-0.1.5b0/ach/record_types/entry_detail.py` & `ach-file-0.1.6b0/ach/record_types/batch_header.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,51 +1,96 @@
-"""Defines entry detail fields and record type."""
+"""Defines batch header fields and record type."""
 
 from typing import Dict
 
 from ..constants import (
-    ENTRY_DETAIL_DEFAULT_ADDENDA_RECORD_INDICATOR,
-    ENTRY_DETAIL_RECORD_TYPE_CODE
+    AutoDateInput,
+    BATCH_HEADER_DEFAULT_ORIGINATOR_STATUS_CODE,
+    BATCH_DEFAULT_SERVICE_CLASS_CODE,
+    BATCH_HEADER_DEFAULT_STANDARD_ENTRY_CLASS_CODE,
+    BATCH_HEADER_RECORD_TYPE_CODE,
 )
 from .record_fields import (
-    AlphaNumFieldType, FieldDefinition, IntegerFieldType
+    AlphaNumFieldType,
+    DateFieldType,
+    FieldDefinition,
+    IntegerFieldType,
 )
 from .record_type_base import RecordType
 
 
 # pylint: disable=line-too-long
-class EntryDetailRecordType(RecordType):
-    """Define all fields in an entry detail record line of an ACH file."""
+class BatchHeaderRecordType(RecordType):
+    """Define all fields in a batch header record line of an ACH file."""
+
     field_definition_dict: Dict[str, FieldDefinition] = {
-        'record_type_code': FieldDefinition('Record Type Code', IntegerFieldType, length=1, default=ENTRY_DETAIL_RECORD_TYPE_CODE),
-        'transaction_code': FieldDefinition('Transaction Code', IntegerFieldType, length=2),
-        'rdfi_routing': FieldDefinition('RDFI Routing Number', IntegerFieldType, length=9),
-        'rdfi_account_number': FieldDefinition('RDFI Account Number', AlphaNumFieldType, length=17, auto_correct_input=False),
-        'amount': FieldDefinition('Transaction Amount Expressed As Cents', IntegerFieldType, length=10),
-        'individual_identification_number': FieldDefinition('Individual Identification Number (Alphanumeric)', AlphaNumFieldType, length=15, required=False),
-        'individual_name': FieldDefinition('Individual Name', AlphaNumFieldType, length=22),
-        'discretionary_data': FieldDefinition('Discretionary Data', AlphaNumFieldType, length=2, required=False),
-        'addenda_record_indicator': FieldDefinition('Addenda Record Indicator', IntegerFieldType, length=1, default=ENTRY_DETAIL_DEFAULT_ADDENDA_RECORD_INDICATOR),
-        'trace_odfi_identifier': FieldDefinition('Trace Number: ODFI Identifier', IntegerFieldType, length=8),
-        'trace_sequence_number': FieldDefinition('Trace Number: Sequence Number', IntegerFieldType, length=7)
+        "record_type_code": FieldDefinition(
+            "Record Type Code",
+            IntegerFieldType,
+            length=1,
+            default=BATCH_HEADER_RECORD_TYPE_CODE,
+        ),
+        "service_class_code": FieldDefinition(
+            "Service Class Code",
+            IntegerFieldType,
+            length=3,
+            default=BATCH_DEFAULT_SERVICE_CLASS_CODE,
+        ),
+        "company_name": FieldDefinition("Company Name", AlphaNumFieldType, length=16),
+        "company_discretionary_data": FieldDefinition(
+            "Company Discretionary Data", AlphaNumFieldType, length=20, required=False
+        ),
+        "company_identification": FieldDefinition(
+            "Company Identification Number", IntegerFieldType, length=10
+        ),
+        "standard_entry_class_code": FieldDefinition(
+            "Standard Entry Class Code",
+            AlphaNumFieldType,
+            length=3,
+            default=BATCH_HEADER_DEFAULT_STANDARD_ENTRY_CLASS_CODE,
+        ),
+        "company_entry_description": FieldDefinition(
+            "Company Entry Description", AlphaNumFieldType, length=10
+        ),
+        "company_descriptive_date": FieldDefinition(
+            "Company Descriptive Date", DateFieldType, length=6, required=False
+        ),
+        "effective_entry_date": FieldDefinition(
+            "Effective Entry Date",
+            DateFieldType,
+            length=6,
+            default=AutoDateInput.TOMORROW,
+            auto_correct_input=True,
+        ),
+        "settlement_date": FieldDefinition(
+            "Settlement Date", AlphaNumFieldType, length=3, required=False
+        ),
+        "originator_status_code": FieldDefinition(
+            "Originator Status Code",
+            IntegerFieldType,
+            length=1,
+            default=BATCH_HEADER_DEFAULT_ORIGINATOR_STATUS_CODE,
+        ),
+        "odfi_identification": FieldDefinition(
+            "ODFI Identification (Routing Without Final Digit)",
+            IntegerFieldType,
+            length=8,
+        ),
+        "batch_number": FieldDefinition("Batch Number", IntegerFieldType, length=7),
     }
 
     # pylint: disable=too-many-arguments
     def __init__(
-            self,
-            transaction_code: int,
-            rdfi_routing: str,
-            rdfi_account_number: str,
-            amount: int,
-            individual_name: str,
-            trace_number: str = None,
-            **kwargs
-        ):
-        kwargs['transaction_code'] = transaction_code
-        kwargs['rdfi_routing'] = rdfi_routing
-        kwargs['rdfi_account_number'] = rdfi_account_number
-        kwargs['amount'] = amount
-        kwargs['individual_name'] = individual_name
-        if trace_number is not None:
-            kwargs['trace_odfi_identifier'] = str(trace_number)[:8]
-            kwargs['trace_sequence_number'] = str(trace_number)[8:15]
+        self,
+        company_name: str,
+        company_identification: str,
+        company_entry_description: str,
+        odfi_identification: str,
+        batch_number: int,
+        **kwargs
+    ):
+        kwargs["company_name"] = company_name
+        kwargs["company_identification"] = company_identification
+        kwargs["company_entry_description"] = company_entry_description
+        kwargs["odfi_identification"] = odfi_identification
+        kwargs["batch_number"] = batch_number
         super().__init__(**kwargs)
```

### Comparing `ach-file-0.1.5b0/ach/record_types/file_header.py` & `ach-file-0.1.6b0/ach/record_types/file_header.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,53 +5,102 @@
 from ..constants import (
     AutoDateInput,
     FILE_HEADER_BLOCKING_FACTOR,
     FILE_HEADER_DEFAULT_FILE_ID_MODIFIER,
     FILE_HEADER_FORMAT_CODE,
     FILE_HEADER_PRIORITY_CODE,
     FILE_HEADER_RECORD_TYPE_CODE,
-    RECORD_SIZE
+    RECORD_SIZE,
 )
 from .record_fields import (
     AlphaNumFieldType,
     BlankPaddedRoutingNumberFieldType,
     DateFieldType,
     TimeFieldType,
     FieldDefinition,
-    IntegerFieldType
+    IntegerFieldType,
 )
 from .record_type_base import RecordType
 
 
 # pylint: disable=line-too-long
 class FileHeaderRecordType(RecordType):
     """Defines all fields of a file header record line of an ACH file."""
+
     field_definition_dict: Dict[str, FieldDefinition] = {
-        'record_type_code': FieldDefinition('Record Type Code', IntegerFieldType, length=1, default=FILE_HEADER_RECORD_TYPE_CODE),
-        'priority_code': FieldDefinition('Priority Code', IntegerFieldType, length=2, default=FILE_HEADER_PRIORITY_CODE),
-        'destination_routing': FieldDefinition('Immediate Destination Routing', BlankPaddedRoutingNumberFieldType, length=10, auto_correct_input=True),
-        'origin_routing': FieldDefinition('Immediate Origin Routing', BlankPaddedRoutingNumberFieldType, length=10, auto_correct_input=True),
-        'file_creation_date': FieldDefinition('File Creation Date', DateFieldType, length=6, auto_correct_input=True, default=AutoDateInput.NOW),
-        'file_creation_time': FieldDefinition('File Creation Time', TimeFieldType, length=4, required=False),
-        'file_id_modifier': FieldDefinition('File ID Modifier', AlphaNumFieldType, length=1, default=FILE_HEADER_DEFAULT_FILE_ID_MODIFIER),
-        'record size': FieldDefinition('Record Size', IntegerFieldType, length=3, default=RECORD_SIZE),
-        'blocking_factor': FieldDefinition('Blocking Factor', IntegerFieldType, length=2, default=FILE_HEADER_BLOCKING_FACTOR),
-        'format_code': FieldDefinition('Format Code', IntegerFieldType, length=1, default=FILE_HEADER_FORMAT_CODE),
-        'destination_name': FieldDefinition('Destination Financial Institution Name', AlphaNumFieldType, length=23),
-        'origin_name': FieldDefinition('Origin Financial Institution Name', AlphaNumFieldType, length=23),
-        'reference_code': FieldDefinition('Reference Code Or Empty String', AlphaNumFieldType, length=8, default=''),
+        "record_type_code": FieldDefinition(
+            "Record Type Code",
+            IntegerFieldType,
+            length=1,
+            default=FILE_HEADER_RECORD_TYPE_CODE,
+        ),
+        "priority_code": FieldDefinition(
+            "Priority Code",
+            IntegerFieldType,
+            length=2,
+            default=FILE_HEADER_PRIORITY_CODE,
+        ),
+        "destination_routing": FieldDefinition(
+            "Immediate Destination Routing",
+            BlankPaddedRoutingNumberFieldType,
+            length=10,
+            auto_correct_input=True,
+        ),
+        "origin_routing": FieldDefinition(
+            "Immediate Origin Routing",
+            BlankPaddedRoutingNumberFieldType,
+            length=10,
+            auto_correct_input=True,
+        ),
+        "file_creation_date": FieldDefinition(
+            "File Creation Date",
+            DateFieldType,
+            length=6,
+            auto_correct_input=True,
+            default=AutoDateInput.NOW,
+        ),
+        "file_creation_time": FieldDefinition(
+            "File Creation Time", TimeFieldType, length=4, required=False
+        ),
+        "file_id_modifier": FieldDefinition(
+            "File ID Modifier",
+            AlphaNumFieldType,
+            length=1,
+            default=FILE_HEADER_DEFAULT_FILE_ID_MODIFIER,
+        ),
+        "record size": FieldDefinition(
+            "Record Size", IntegerFieldType, length=3, default=RECORD_SIZE
+        ),
+        "blocking_factor": FieldDefinition(
+            "Blocking Factor",
+            IntegerFieldType,
+            length=2,
+            default=FILE_HEADER_BLOCKING_FACTOR,
+        ),
+        "format_code": FieldDefinition(
+            "Format Code", IntegerFieldType, length=1, default=FILE_HEADER_FORMAT_CODE
+        ),
+        "destination_name": FieldDefinition(
+            "Destination Financial Institution Name", AlphaNumFieldType, length=23
+        ),
+        "origin_name": FieldDefinition(
+            "Origin Financial Institution Name", AlphaNumFieldType, length=23
+        ),
+        "reference_code": FieldDefinition(
+            "Reference Code Or Empty String", AlphaNumFieldType, length=8, default=""
+        ),
     }
 
     def __init__(
         self,
         destination_routing: str,
         origin_routing: str,
         destination_name: str,
         origin_name: str,
         **kwargs
     ):
         self.field_definition_dict = self.field_definition_dict
-        kwargs['destination_routing'] = destination_routing
-        kwargs['origin_routing'] = origin_routing
-        kwargs['destination_name'] = destination_name
-        kwargs['origin_name'] = origin_name
+        kwargs["destination_routing"] = destination_routing
+        kwargs["origin_routing"] = origin_routing
+        kwargs["destination_name"] = destination_name
+        kwargs["origin_name"] = origin_name
         super().__init__(**kwargs)
```

### Comparing `ach-file-0.1.5b0/ach/record_types/record_fields.py` & `ach-file-0.1.6b0/ach/record_types/record_fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,16 @@
         msg_format: str -- Message containing "{}" to indicate where string arguments
             can be formatted dynamically on instantiation
         value: str -- Value passed in to be validated as a particular FieldType
         field_type_or_regex: str -- Descriptive string indicating either the regex
             or type of field that the value mismatched
         message: Message displayed when exception is raised
     """
-    msg_format = "Passed-in value \"{}\" mismatches {}"
+
+    msg_format = 'Passed-in value "{}" mismatches {}'
 
     def __init__(self, value: str, field_type_or_regex: str):
         self.value = value
         self.field_type_or_regex = field_type_or_regex
         self.message = self.msg_format.format(self.value, self.field_type_or_regex)
         super().__init__(self.message)
 
@@ -38,24 +39,26 @@
 
     Attributes:
         msg_format: str -- Message containing "{}" to indicate where string arguments
             can be formatted dynamically on instantiation
         field_name: str -- Pretty name of FieldDefinition with missing value
         message: Message displayed when exception is raised
     """
+
     msg_format = "Field {} requires a value and there is no default in its definition"
 
     def __init__(self, field_name: str):
         self.field_name = field_name
         self.message = self.msg_format.format(field_name)
         super().__init__(self.message)
 
 
 class Alignment(Enum):
     """Represents whether a field type should be aligned left or right."""
+
     LEFT = 0
     RIGHT = 1
 
     def align(self, input_string: str, length: int, padding: str) -> str:
         """
         Aligns text to the left or right of a given string length,
         using padding to fill any gaps if input string is shorter than length.
@@ -84,38 +87,47 @@
     Attributes:
         padding: str -- Filler for fixed-width string
         alignment: Alignment -- Original string should be oriented
             either left or right in fixed-width string
         regex: Optional[re.Pattern] -- pattern against which original string
             should be validated
     """
+
     padding: str
     alignment: Alignment
     regex: Optional[re.Pattern]
     auto_correct: bool
 
     @classmethod
     def apply_fixed_length(cls, input_string: str, length: int) -> str:
         """Adds padding for short strings and truncates long ones."""
         input_string = cls.alignment.align(input_string, length, cls.padding)
         return cls.alignment.truncate(input_string, length)
 
     @classmethod
     def should_correct_input(cls, auto_correct_override: Optional[bool]) -> bool:
         """Return True if auto_correct is True, else False if input is not to be changed."""
-        return auto_correct_override if auto_correct_override is not None else cls.auto_correct
+        return (
+            auto_correct_override
+            if auto_correct_override is not None
+            else cls.auto_correct
+        )
 
     # pylint: disable=unused-argument
     @classmethod
-    def correct_input(cls, input_string: str, auto_correct_override: Optional[bool] = None) -> str:
+    def correct_input(
+        cls, input_string: str, auto_correct_override: Optional[bool] = None
+    ) -> str:
         """Correct input to only contain characters that would pass regex check."""
         return input_string
 
     @classmethod
-    def is_valid(cls, input_string: str, *args, raise_exc: bool = False, **kwargs) -> bool:
+    def is_valid(
+        cls, input_string: str, *args, raise_exc: bool = False, **kwargs
+    ) -> bool:
         """
         Returns True if input is valid, else False.
         Raises exc instead of return False if raise_exc.
         """
         exc = None
         try:
             cls.do_validation(input_string, *args, **kwargs)
@@ -131,128 +143,153 @@
     @classmethod
     def do_validation(cls, input_string: str, *args, **kwargs) -> None:
         """
         Validates input string. If invalid, raises exception, else returns None.
         """
         if not cls.regex:
             return
-        is_match = input_string == getattr(re.match(cls.regex, input_string), 'string', '')
+        is_match = input_string == getattr(
+            re.match(cls.regex, input_string), "string", ""
+        )
         if not is_match:
-            raise ValueMismatchesFieldTypeError(input_string, cls.regex.pattern or cls.__name__)
+            raise ValueMismatchesFieldTypeError(
+                input_string, cls.regex.pattern or cls.__name__
+            )
 
 
 class IntegerFieldType(FieldType):
     """Represents an integer field type. Pads number strings with leading 0s."""
-    padding: str = '0'
+
+    padding: str = "0"
     alignment: Alignment = Alignment.RIGHT
-    regex: re.Pattern = re.compile(r'^\d+$')
+    regex: re.Pattern = re.compile(r"^\d+$")
     auto_correct: bool = False
 
 
 class AlphaNumFieldType(FieldType):
     """Represents an alphanumeric field type. Pads strings with trailing spaces."""
-    padding: str = ' '
+
+    padding: str = " "
     alignment: Alignment = Alignment.LEFT
-    regex: re.Pattern = re.compile(r'^[A-Za-z0-9./()&\'\s-]+$')
+    regex: re.Pattern = re.compile(r"^[A-Za-z0-9./()&\'\s-]+$")
     auto_correct: bool = True
 
     @classmethod
-    def correct_input(cls, input_string: str, auto_correct_override: Optional[bool] = None) -> str:
+    def correct_input(
+        cls, input_string: str, auto_correct_override: Optional[bool] = None
+    ) -> str:
         """
         Replaces all characters not present in class's regex pattern with an empty string.
         """
         if not cls.should_correct_input(auto_correct_override):
             return input_string
-        return re.sub( re.compile(r'[^A-Za-z0-9./()&\'\s-]'), '', input_string)
+        return re.sub(re.compile(r"[^A-Za-z0-9./()&\'\s-]"), "", input_string)
 
 
 class BlankPaddedRoutingNumberFieldType(IntegerFieldType):
     """Represents a routing number padded with a leading blank space."""
-    padding: str = ' '
-    regex: re.Pattern = re.compile(r'^\s?\d{9}$')
+
+    padding: str = " "
+    regex: re.Pattern = re.compile(r"^\s?\d{9}$")
     auto_correct: bool = True
 
     @classmethod
-    def correct_input(cls, input_string: str, auto_correct_override: Optional[bool] = None) -> str:
+    def correct_input(
+        cls, input_string: str, auto_correct_override: Optional[bool] = None
+    ) -> str:
         if not cls.should_correct_input(auto_correct_override):
             return input_string
         if not cls.auto_correct:
             return input_string
         if not input_string:
-            return ''
+            return ""
         if cls.is_valid(input_string):
             return input_string
         if input_string.lstrip().isdigit():
-            return Alignment.RIGHT.align(input_string, 9, '0')
+            return Alignment.RIGHT.align(input_string, 9, "0")
         return input_string
 
 
 class DateFieldType(AlphaNumFieldType):
     """
     Accepts 6 digits representing a valid date OR generates a date
     given a datetime.date, a datetime.datetime, or an AutoDateInput string.
     If not required, pads with blanks.
     """
-    regex: re.Pattern = re.compile(r'^\d{6}$')
+
+    regex: re.Pattern = re.compile(r"^\d{6}$")
     auto_correct: bool = True
 
     @classmethod
-    def correct_input(cls, input_string: str, auto_correct_override: Optional[bool] = None) -> str:
-        if not cls.should_correct_input(auto_correct_override) or cls.is_valid(input_string):
+    def correct_input(
+        cls, input_string: str, auto_correct_override: Optional[bool] = None
+    ) -> str:
+        if not cls.should_correct_input(auto_correct_override) or cls.is_valid(
+            input_string
+        ):
             return input_string
 
         if input_string.upper() == AutoDateInput.NOW.value:
-            return datetime.date.today().strftime('%y%m%d')
+            return datetime.date.today().strftime("%y%m%d")
 
         if input_string.upper() == AutoDateInput.TOMORROW.value:
-            return (datetime.date.today() + datetime.timedelta(days=1)).strftime('%y%m%d')
+            return (datetime.date.today() + datetime.timedelta(days=1)).strftime(
+                "%y%m%d"
+            )
 
         with suppress(ValueError):
-            return datetime.datetime.fromisoformat(input_string).strftime('%y%m%d')
+            return datetime.datetime.fromisoformat(input_string).strftime("%y%m%d")
 
         with suppress(ValueError):
-            return datetime.date.fromisoformat(input_string).strftime('%y%m%d')
+            return datetime.date.fromisoformat(input_string).strftime("%y%m%d")
 
         return input_string
 
     @classmethod
     def do_validation(cls, input_string: str, *args, **kwargs) -> None:
         if not input_string or not input_string.strip():
             return
         try:
             super().do_validation(input_string, *args, **kwargs)
         except Exception as exc:
             raise exc from exc
-        datetime.date(2000 + int(input_string[:2]), int(input_string[2:4]), int(input_string[4:6]))
+        datetime.date(
+            2000 + int(input_string[:2]), int(input_string[2:4]), int(input_string[4:6])
+        )
 
 
 class TimeFieldType(AlphaNumFieldType):
     """
     Accepts 4 digits representing military time hours and minutes
     OR generates a time given a datetime.datetime or AutoDateInput string.
     """
-    regex: re.Pattern = re.compile(r'^\d{4}$')
+
+    regex: re.Pattern = re.compile(r"^\d{4}$")
     auto_correct: bool = True
 
     @classmethod
-    def correct_input(cls, input_string: str, auto_correct_override: Optional[bool] = None) -> str:
-        if not cls.should_correct_input(auto_correct_override) or cls.is_valid(input_string):
+    def correct_input(
+        cls, input_string: str, auto_correct_override: Optional[bool] = None
+    ) -> str:
+        if not cls.should_correct_input(auto_correct_override) or cls.is_valid(
+            input_string
+        ):
             return input_string
 
         if input_string.upper() == AutoDateInput.NOW.value:
-            return datetime.datetime.now().strftime('%H%M')
+            return datetime.datetime.now().strftime("%H%M")
 
         if input_string.upper() == AutoDateInput.TOMORROW.value:
-            return (datetime.date.today() + datetime.timedelta(days=1)).strftime('%H%M')
+            return (datetime.date.today() + datetime.timedelta(days=1)).strftime("%H%M")
 
         with suppress(ValueError):
-            return datetime.datetime.fromisoformat(input_string).strftime('%H%M')
+            return datetime.datetime.fromisoformat(input_string).strftime("%H%M")
 
         with suppress(ValueError):
-            return datetime.date.fromisoformat(input_string).strftime('%H%M')
+            return datetime.date.fromisoformat(input_string).strftime("%H%M")
 
         return input_string
 
     @classmethod
     def do_validation(cls, input_string: str, *args, **kwargs) -> None:
         if not input_string or not input_string.strip():
             return
@@ -275,14 +312,15 @@
             accepted in a Field with this given FieldDefinition
         length: int -- length of field
             (when original input is padded, aligned, corrected)
         required: bool -- whether value needs to be non-blank
         default: Optional[str] -- if no value is provided to Field,
             defines what is automatically set as the Field's value
     """
+
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         field_name: str,
         field_type: FieldType,
         length: int,
         required: bool = True,
@@ -294,27 +332,32 @@
         self.length = length
         self.required = required
         self.default = str(default) if default is not None else None
         self.auto_correct_input = auto_correct_input
 
     # pylint: disable=consider-using-f-string
     def __repr__(self) -> str:
-        return '<{}: {} [{}]>'.format(
-            type(self).__name__, self.field_name, self.field_type.__name__)
+        return "<{}: {} [{}]>".format(
+            type(self).__name__, self.field_name, self.field_type.__name__
+        )
 
     def correct_input(self, input_string: str) -> str:
         """Corrects input according to current setting and FieldType default setting."""
         return self.field_type.correct_input(input_string, self.auto_correct_input)
 
-    def is_valid(self, input_string: str, *args, raise_exc: bool = True, **kwargs) -> bool:
+    def is_valid(
+        self, input_string: str, *args, raise_exc: bool = True, **kwargs
+    ) -> bool:
         """
         Returns True if string is valid, else False.
         If raise_exc, raises an exception instead of returning False.
         """
-        return self.field_type.is_valid(input_string, *args, raise_exc=raise_exc, **kwargs)
+        return self.field_type.is_valid(
+            input_string, *args, raise_exc=raise_exc, **kwargs
+        )
 
     def get_fixed_width_value(self, input_string: str) -> str:
         """Convert input string to fixed length according to its FieldType."""
         return self.field_type.apply_fixed_length(input_string, self.length)
 
 
 class Field:
@@ -326,42 +369,52 @@
         field_definition: FieldDefinition -- defines properties of a field
             in a record
         original_value: Optional[str] -- raw value passed into field before
             alignments and corrections
         cleaned_value: str: Setting this attribute interrupts initialization
             if raw input value is invalid
     """
+
     # pylint: disable=too-few-public-methods
     def __init__(self, field_definition: FieldDefinition, value: Optional[str] = None):
         self.field_definition = field_definition
         self.original_value = value
         self.value = value
 
     @property
     def value(self) -> str:
         """Return cleaned value of field (not original value)."""
         return self.cleaned_value
 
     @value.setter
     def value(self, raw_value: str) -> None:
         """Set a new cleaned value on this Field."""
-        self.cleaned_value = Field._create_cleaned_value(self.field_definition, raw_value)
+        self.cleaned_value = Field._create_cleaned_value(
+            self.field_definition, raw_value
+        )
 
     @staticmethod
-    def _create_cleaned_value(field_definition: FieldDefinition, value: Optional[str] = None):
+    def _create_cleaned_value(
+        field_definition: FieldDefinition, value: Optional[str] = None
+    ):
         Field._validate_required_value_not_empty(field_definition, value)
 
-        ret_value: str = ''
+        ret_value: str = ""
         if isinstance(value, (datetime.date, datetime.datetime)):
             ret_value = value.isoformat()
-        ret_value = str(field_definition.default or '') if value is None else str(value)
+        ret_value = str(field_definition.default or "") if value is None else str(value)
 
         ret_value = field_definition.correct_input(ret_value)
 
         field_definition.is_valid(ret_value, raise_exc=True)
         return field_definition.get_fixed_width_value(ret_value)
 
     @staticmethod
     def _validate_required_value_not_empty(
-        field_definition: FieldDefinition, value: Optional[str]) -> None:
-        if value is None and field_definition.required and field_definition.default is None:
+        field_definition: FieldDefinition, value: Optional[str]
+    ) -> None:
+        if (
+            value is None
+            and field_definition.required
+            and field_definition.default is None
+        ):
             raise EmptyRequiredFieldError(field_definition.field_name)
```

### Comparing `ach-file-0.1.5b0/ach/record_types/record_type_base.py` & `ach-file-0.1.6b0/ach/record_types/record_type_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,95 +9,107 @@
 
 
 class InvalidRecordSizeError(Exception):
     """
     Raises when a RecordType's FieldDefinitions result in
     an invalid record size.
     """
+
     msg_format = (
         "FieldDefinition list for {} would result in an invalid record size"
         " of {} (valid record size is {})"
     )
 
     def __init__(
         self,
         record_type_class_name: str,
         invalid_record_size: int,
-        valid_record_size: int = RECORD_SIZE
+        valid_record_size: int = RECORD_SIZE,
     ):
         self.record_type_class_name = record_type_class_name
         self.invalid_record_size = invalid_record_size
         self.valid_record_size = valid_record_size
         self.message = self.msg_format.format(
-            record_type_class_name, invalid_record_size, valid_record_size)
+            record_type_class_name, invalid_record_size, valid_record_size
+        )
         super().__init__(self.message)
 
 
 class InvalidRecordTypeParametersError(Exception):
     """
     Raises when a RecordType accepts an invalid parameter by keyword.
     """
+
     msg_format = "RecordType class {} received invalid kwargs on instantiation: {}"
 
     def __init__(self, record_type_class_name: str, invalid_kwargs: List[str]) -> None:
         self.record_type_class_name = record_type_class_name
         self.invalid_kwargs = invalid_kwargs
         self.message = self.msg_format.format(
-            self.record_type_class_name, invalid_kwargs)
+            self.record_type_class_name, invalid_kwargs
+        )
         super().__init__(self.message)
 
 
 class RecordTypeAggregateFieldCreationError(Exception):
     """
     Raises after aggregating multiple Field creation exceptions.
 
     Attributes:
         errors: List[Exception] -- List of multiple errors that occurred when trying to create
             multiple Fields for a RecordType
         failed_keys: List[str] -- List of keys that failed to be set
         class_name: str -- Name of class where errors were encountered
     """
-    msg_format = "Encountered {} errors generating Fields for class {}; failed keys: {}; {}"
 
-    def __init__(self, class_name: str, errors: List[Exception], failed_keys: List[str]):
+    msg_format = (
+        "Encountered {} errors generating Fields for class {}; failed keys: {}; {}"
+    )
+
+    def __init__(
+        self, class_name: str, errors: List[Exception], failed_keys: List[str]
+    ):
         self.class_name = class_name
         self.errors = errors
         self.failed_keys = failed_keys
         self.message = self.msg_format.format(
-            len(errors), self.class_name, failed_keys, errors)
+            len(errors), self.class_name, failed_keys, errors
+        )
         super().__init__(self.message)
 
 
 class RecordType:
     """
     Base class for record types.
     Renders Fields as a record line by validating FieldDefinitions and generating Fields from them.
     """
+
     field_definition_dict: Dict[str, FieldDefinition] = {}
 
     def __init__(
         self,
         field_definition_dict: Optional[Dict[str, FieldDefinition]] = None,
         desired_record_size: int = RECORD_SIZE,
         **kwargs
     ):
         if field_definition_dict:
             self.field_definition_dict = field_definition_dict
 
         self._validate_field_definition_list(
-            self.field_definition_dict, desired_record_size)
-        self._validate_no_unknown_key_arguments(
-            self.field_definition_dict, kwargs)
+            self.field_definition_dict, desired_record_size
+        )
+        self._validate_no_unknown_key_arguments(self.field_definition_dict, kwargs)
 
         self.fields: Dict[str, Field] = self._generate_fields_dict(
-            self.field_definition_dict, kwargs)
+            self.field_definition_dict, kwargs
+        )
 
     def render_record_line(self) -> str:
         """Render single record as a line in a valid ACH file."""
-        result = ''
+        result = ""
         for field in self.fields.values():
             result += field.value
         return result
 
     @classmethod
     def get_required_kwargs(cls) -> Dict[str, FieldDefinition]:
         """
@@ -148,26 +160,35 @@
         Raises RecordTypeAggregateFieldCreationError at the end if any errors were encountered.
         """
         failed_keys, exceptions = [], []
         for key, value in kwargs.items():
             self._catch_set_value_on_field_errors(failed_keys, exceptions, key, value)
         if failed_keys:
             raise RecordTypeAggregateFieldCreationError(
-                type(self).__name__, exceptions, failed_keys) from exceptions[0]
+                type(self).__name__, exceptions, failed_keys
+            ) from exceptions[0]
 
-    def _generate_fields_dict(self, field_def_dict: Dict, kwargs: Dict) -> Dict[str, Field]:
+    def _generate_fields_dict(
+        self, field_def_dict: Dict, kwargs: Dict
+    ) -> Dict[str, Field]:
         fields = {}
         failed_keys, exceptions = [], []
         for key in field_def_dict:
             self._catch_set_value_on_field_errors(
-                failed_keys, exceptions, key, kwargs.get(key),
-                field_def_dict=field_def_dict, fields_dict=fields)
+                failed_keys,
+                exceptions,
+                key,
+                kwargs.get(key),
+                field_def_dict=field_def_dict,
+                fields_dict=fields,
+            )
         if exceptions:
             raise RecordTypeAggregateFieldCreationError(
-                type(self).__name__, exceptions, failed_keys) from exceptions[0]
+                type(self).__name__, exceptions, failed_keys
+            ) from exceptions[0]
         return fields
 
     def _catch_set_value_on_field_errors(
         self,
         failed_keys: List[str],
         exceptions: List[Exception],
         key: str,
@@ -188,14 +209,15 @@
 
     @classmethod
     def _validate_field_definition_list(
         cls,
         field_definition_dict: Dict[str, FieldDefinition],
         desired_record_size: int = RECORD_SIZE,
     ) -> None:
-
         resulting_record_size = 0
         for field_def in field_definition_dict.values():
             resulting_record_size += field_def.length
 
         if resulting_record_size != desired_record_size:
-            raise InvalidRecordSizeError(cls.__name__, resulting_record_size, desired_record_size)
+            raise InvalidRecordSizeError(
+                cls.__name__, resulting_record_size, desired_record_size
+            )
```

### Comparing `ach-file-0.1.5b0/ach_file.egg-info/PKG-INFO` & `ach-file-0.1.6b0/ach_file.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ach-file
-Version: 0.1.5b0
+Version: 0.1.6b0
 Summary: Highly configurable and permissive library to generate ACH files
 Home-page: https://github.com/freemish/ach-file
 Author: Molly Gouletas
 Author-email: molly.gouletas@gmail.com
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ach-file-0.1.5b0/ach_file.egg-info/SOURCES.txt` & `ach-file-0.1.6b0/ach_file.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ach-file-0.1.5b0/setup.py` & `ach-file-0.1.6b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from distutils.core import setup
 from setuptools import find_packages
 
 setup(
     name='ach-file',
     author='Molly Gouletas',
     author_email='molly.gouletas@gmail.com',
-    version='0.1.5.beta',
+    version='0.1.6.beta',
     packages=find_packages(exclude=['tests']),
     url='https://github.com/freemish/ach-file',
     license='MIT License',
     description='Highly configurable and permissive library to generate ACH files',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     classifiers=[
```

