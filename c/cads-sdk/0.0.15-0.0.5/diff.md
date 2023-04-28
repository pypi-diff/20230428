# Comparing `tmp/cads_sdk-0.0.15-py3-none-any.whl.zip` & `tmp/cads_sdk-0.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,20 +1,28 @@
-Zip file size: 55297 bytes, number of entries: 18
--rw-rw-r--  2.0 unx     1265 b- defN 23-Apr-28 02:33 cads_sdk/__init__.py
--rw-rw-r--  2.0 unx     1264 b- defN 23-Apr-01 02:59 cads_sdk/nosql/__init__.py
--rw-rw-r--  2.0 unx    11231 b- defN 23-Apr-17 08:04 cads_sdk/nosql/codec.py
--rw-rw-r--  2.0 unx    84386 b- defN 23-Apr-28 02:32 cads_sdk/nosql/converter.py
--rw-rw-r--  2.0 unx    19499 b- defN 23-Apr-20 10:32 cads_sdk/nosql/display.py
--rw-rw-r--  2.0 unx     1187 b- defN 23-Apr-10 10:46 cads_sdk/nosql/etl.py
--rw-rw-r--  2.0 unx      591 b- defN 23-Apr-09 13:11 cads_sdk/nosql/utils.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Apr-09 14:03 cads_sdk/petastorm/__init__.py
--rw-rw-r--  2.0 unx    19967 b- defN 23-Apr-10 04:34 cads_sdk/petastorm/dataset_metadata.py
--rw-rw-r--  2.0 unx    10508 b- defN 23-Apr-10 07:19 cads_sdk/petastorm/fs_utils.py
--rw-rw-r--  2.0 unx     5427 b- defN 23-Apr-10 04:42 cads_sdk/petastorm/utils.py
--rw-rw-r--  2.0 unx    22554 b- defN 23-Apr-18 15:18 cads_sdk/pytorch/__init__.py
--rw-rw-r--  2.0 unx    10653 b- defN 23-Apr-17 08:05 cads_sdk/pytorch/codec.py
--rw-rw-r--  2.0 unx    78369 b- defN 23-Apr-20 08:23 cads_sdk/pytorch/converter.py
--rw-rw-r--  2.0 unx     7126 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1479 b- defN 23-Apr-28 02:36 cads_sdk-0.0.15.dist-info/RECORD
-18 files, 275607 bytes uncompressed, 52891 bytes compressed:  80.8%
+Zip file size: 69131 bytes, number of entries: 26
+-rw-rw-r--  2.0 unx     1253 b- defN 23-Mar-31 02:38 cads_sdk/__init__.py
+-rw-rw-r--  2.0 unx     4469 b- defN 23-Mar-22 09:21 cads_sdk/create_yaml_file.py
+-rw-rw-r--  2.0 unx     6309 b- defN 23-Mar-22 09:21 cads_sdk/datahub_api.py
+-rw-rw-r--  2.0 unx     9905 b- defN 23-Mar-22 09:21 cads_sdk/hive_metastore.py
+-rw-rw-r--  2.0 unx     3319 b- defN 23-Mar-22 09:21 cads_sdk/ingest_hive_datahub.py
+-rw-rw-r--  2.0 unx     1767 b- defN 23-Mar-22 09:21 cads_sdk/pandas_decrypt.py
+-rw-rw-r--  2.0 unx    50207 b- defN 23-Mar-28 16:20 cads_sdk/pyspark_add_on.py
+-rw-rw-r--  2.0 unx     4100 b- defN 23-Mar-22 09:21 cads_sdk/utils.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Mar-22 09:21 cads_sdk/nosql/__init__.py
+-rw-rw-r--  2.0 unx    11885 b- defN 23-Mar-30 03:54 cads_sdk/nosql/codec.py
+-rw-rw-r--  2.0 unx    67828 b- defN 23-Mar-31 02:31 cads_sdk/nosql/converter.py
+-rw-rw-r--  2.0 unx    14277 b- defN 23-Mar-29 02:33 cads_sdk/nosql/display.py
+-rw-rw-r--  2.0 unx     1184 b- defN 23-Mar-29 09:53 cads_sdk/nosql/etl.py
+-rw-rw-r--  2.0 unx     1203 b- defN 22-Dec-27 06:55 spark_sdk/__init__.py
+-rw-rw-r--  2.0 unx        1 b- defN 22-Dec-27 06:55 spark_sdk/_version.py
+-rw-rw-r--  2.0 unx     4469 b- defN 22-Dec-27 06:55 spark_sdk/create_yaml_file.py
+-rw-rw-r--  2.0 unx     9905 b- defN 22-Dec-27 06:55 spark_sdk/hive_metastore.py
+-rw-rw-r--  2.0 unx     3319 b- defN 22-Dec-27 06:55 spark_sdk/ingest_hive_datahub.py
+-rw-rw-r--  2.0 unx     1766 b- defN 22-Dec-27 06:55 spark_sdk/pandas_decrypt.py
+-rw-rw-r--  2.0 unx    44328 b- defN 22-Dec-27 06:55 spark_sdk/pandas_to_dwh.py
+-rw-rw-r--  2.0 unx    48933 b- defN 22-Dec-27 06:55 spark_sdk/pyspark_add_on.py
+-rw-rw-r--  2.0 unx     3758 b- defN 22-Dec-27 06:55 spark_sdk/utils.py
+-rw-rw-r--  2.0 unx     7006 b- defN 23-Mar-31 02:39 cads_sdk-0.0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Mar-31 02:39 cads_sdk-0.0.5.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-Mar-31 02:39 cads_sdk-0.0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     2102 b- defN 23-Mar-31 02:39 cads_sdk-0.0.5.dist-info/RECORD
+26 files, 303394 bytes uncompressed, 65775 bytes compressed:  78.3%
```

## zipnote {}

```diff
@@ -1,10 +1,31 @@
 Filename: cads_sdk/__init__.py
 Comment: 
 
+Filename: cads_sdk/create_yaml_file.py
+Comment: 
+
+Filename: cads_sdk/datahub_api.py
+Comment: 
+
+Filename: cads_sdk/hive_metastore.py
+Comment: 
+
+Filename: cads_sdk/ingest_hive_datahub.py
+Comment: 
+
+Filename: cads_sdk/pandas_decrypt.py
+Comment: 
+
+Filename: cads_sdk/pyspark_add_on.py
+Comment: 
+
+Filename: cads_sdk/utils.py
+Comment: 
+
 Filename: cads_sdk/nosql/__init__.py
 Comment: 
 
 Filename: cads_sdk/nosql/codec.py
 Comment: 
 
 Filename: cads_sdk/nosql/converter.py
@@ -12,44 +33,47 @@
 
 Filename: cads_sdk/nosql/display.py
 Comment: 
 
 Filename: cads_sdk/nosql/etl.py
 Comment: 
 
-Filename: cads_sdk/nosql/utils.py
+Filename: spark_sdk/__init__.py
+Comment: 
+
+Filename: spark_sdk/_version.py
 Comment: 
 
-Filename: cads_sdk/petastorm/__init__.py
+Filename: spark_sdk/create_yaml_file.py
 Comment: 
 
-Filename: cads_sdk/petastorm/dataset_metadata.py
+Filename: spark_sdk/hive_metastore.py
 Comment: 
 
-Filename: cads_sdk/petastorm/fs_utils.py
+Filename: spark_sdk/ingest_hive_datahub.py
 Comment: 
 
-Filename: cads_sdk/petastorm/utils.py
+Filename: spark_sdk/pandas_decrypt.py
 Comment: 
 
-Filename: cads_sdk/pytorch/__init__.py
+Filename: spark_sdk/pandas_to_dwh.py
 Comment: 
 
-Filename: cads_sdk/pytorch/codec.py
+Filename: spark_sdk/pyspark_add_on.py
 Comment: 
 
-Filename: cads_sdk/pytorch/converter.py
+Filename: spark_sdk/utils.py
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/METADATA
+Filename: cads_sdk-0.0.5.dist-info/METADATA
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/WHEEL
+Filename: cads_sdk-0.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/top_level.txt
+Filename: cads_sdk-0.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: cads_sdk-0.0.15.dist-info/RECORD
+Filename: cads_sdk-0.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cads_sdk/__init__.py

```diff
@@ -1,31 +1,43 @@
-__version__ = '0.0.15'
+from .pyspark_add_on import PySpark, PyArrow, Utf8Encoder
+from .pyspark_add_on import to_dwh, drop_table, drop_table_and_delete_data, read_table, sql, refresh_table, spark_dataframe_to_dwh
+from .pyspark_add_on import ls, mkdir, cat, exists, info, open
+from .pyspark_add_on import read_dwh_pd, read_csv, read_json, write_json, read_parquet, read_dwh
+from .pyspark_add_on import show, refresh_table
+from .pyspark_add_on import limit_timestamp
+from .pyspark_add_on import spark_dataframe_info
+from .create_yaml_file import CreateYamlDWH
+from .pandas_decrypt import decrypt, decrypt_column
+
+#from .nosql.reader import _repr_html_ as PandasDataFrame_repr_html_
+
+# from .pyspark_add_on.PySpark import to_dwh
+from .utils import modulereload, choose_num_core
+from pandas.core.series import Series
+
+
+import pandas as pd
+from pandas import DataFrame
+
+
+DataFrame.to_dwh = to_dwh
+#DataFrame._repr_html_ = PandasDataFrame_repr_html_
+modulereload(pd)
+
+Series.decrypt_column = decrypt_column
+pd.read_dwh = read_dwh_pd
+modulereload(pd)
+
+
+from pyspark.sql import DataFrame as SparkDataFrame
+SparkDataFrame.to_dwh = spark_dataframe_to_dwh
+SparkDataFrame.info = spark_dataframe_info
+
+
+SparkDataFrame.show = show
+
+
+
+__version__ = '0.0.5'
+__all__ = ["PySpark", "PyArrow"]
 
-__doc__ = """
-cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
-=====================================================================
-**cads-sdk**
-Function to convert 
--------------
-Here are just a few of the things that cads_sdk does well:
-# Image pre-processing ready for train
-    - Function Convert from image folders to parquet: 
-      from cads.nosql.converter import ConvertFromFolderImage
-    - Function Convert from zip fize to parquet: 
-      from cads.nosql.converter import ConvertFromFolderImage
-    - Function Convert parquet to folder of image: 
-      from cads.nosql.converter import ConvertToFolderImage
-    - Function to display parquet image
-      from cads.nosql import display
-      
-# Audio pre-processing ready for train
-    - Function Convert from audio folders to parquet: 
-      from cads.nosql.converter import ConvertToFolderAudio
-    - Function Convert from audio folders to parquet: 
-      from cads.nosql.converter import ConvertFromFolderAudio
-# Video
-    - Function Convert from video files to parquet of frame: 
-      from cads.nosql.converter import ConvertFromVideo2Image
-    - Function to display frame parquet
-      from cads.nosql import display
-"""
```

## cads_sdk/nosql/__init__.py

```diff
@@ -1,79 +0,0 @@
-00000000: 5f5f 646f 635f 5f20 3d20 2222 220a 6361  __doc__ = """.ca
-00000010: 6473 2d73 646b 3a20 4675 6e63 7469 6f6e  ds-sdk: Function
-00000020: 7320 746f 2068 656c 7020 4461 7461 2053  s to help Data S
-00000030: 6369 656e 7469 7374 2077 6f72 6b20 6d6f  cientist work mo
-00000040: 7265 2065 6666 6563 7469 7665 6c79 2077  re effectively w
-00000050: 6974 6820 756e 7374 7275 6374 7572 6564  ith unstructured
-00000060: 2064 6174 6120 616e 6420 6461 7461 6c61   data and datala
-00000070: 6b65 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ke.=============
-00000080: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000090: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000000a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000000b0: 3d3d 3d3d 3d3d 3d3d 0a2a 2a63 6164 732d  ========.**cads-
-000000c0: 7364 6b2a 2a0a 4675 6e63 7469 6f6e 2074  sdk**.Function t
-000000d0: 6f20 636f 6e76 6572 7420 0a2d 2d2d 2d2d  o convert .-----
-000000e0: 2d2d 2d2d 2d2d 2d2d 0a48 6572 6520 6172  --------.Here ar
-000000f0: 6520 6a75 7374 2061 2066 6577 206f 6620  e just a few of 
-00000100: 7468 6520 7468 696e 6773 2074 6861 7420  the things that 
-00000110: 6361 6473 5f73 646b 2064 6f65 7320 7765  cads_sdk does we
-00000120: 6c6c 3a0a 2320 496d 6167 6520 7072 652d  ll:.# Image pre-
-00000130: 7072 6f63 6573 7369 6e67 2072 6561 6479  processing ready
-00000140: 2066 6f72 2074 7261 696e 0a20 2020 202d   for train.    -
-00000150: 2046 756e 6374 696f 6e20 436f 6e76 6572   Function Conver
-00000160: 7420 6672 6f6d 2069 6d61 6765 2066 6f6c  t from image fol
-00000170: 6465 7273 2074 6f20 7061 7271 7565 743a  ders to parquet:
-00000180: 200a 2020 2020 2020 6672 6f6d 2063 6164   .      from cad
-00000190: 732e 6e6f 7371 6c2e 636f 6e76 6572 7465  s.nosql.converte
-000001a0: 7220 696d 706f 7274 2043 6f6e 7665 7274  r import Convert
-000001b0: 4672 6f6d 466f 6c64 6572 496d 6167 650a  FromFolderImage.
-000001c0: 2020 2020 2d20 4675 6e63 7469 6f6e 2043      - Function C
-000001d0: 6f6e 7665 7274 2066 726f 6d20 7a69 7020  onvert from zip 
-000001e0: 6669 7a65 2074 6f20 7061 7271 7565 743a  fize to parquet:
-000001f0: 200a 2020 2020 2020 6672 6f6d 2063 6164   .      from cad
-00000200: 732e 6e6f 7371 6c2e 636f 6e76 6572 7465  s.nosql.converte
-00000210: 7220 696d 706f 7274 2043 6f6e 7665 7274  r import Convert
-00000220: 4672 6f6d 466f 6c64 6572 496d 6167 650a  FromFolderImage.
-00000230: 2020 2020 2d20 4675 6e63 7469 6f6e 2043      - Function C
-00000240: 6f6e 7665 7274 2070 6172 7175 6574 2074  onvert parquet t
-00000250: 6f20 666f 6c64 6572 206f 6620 696d 6167  o folder of imag
-00000260: 653a 200a 2020 2020 2020 6672 6f6d 2063  e: .      from c
-00000270: 6164 732e 6e6f 7371 6c2e 636f 6e76 6572  ads.nosql.conver
-00000280: 7465 7220 696d 706f 7274 2043 6f6e 7665  ter import Conve
-00000290: 7274 546f 466f 6c64 6572 496d 6167 650a  rtToFolderImage.
-000002a0: 2020 2020 2d20 4675 6e63 7469 6f6e 2074      - Function t
-000002b0: 6f20 6469 7370 6c61 7920 7061 7271 7565  o display parque
-000002c0: 7420 696d 6167 650a 2020 2020 2020 6672  t image.      fr
-000002d0: 6f6d 2063 6164 732e 6e6f 7371 6c20 696d  om cads.nosql im
-000002e0: 706f 7274 2064 6973 706c 6179 0a20 2020  port display.   
-000002f0: 2020 200a 2320 4175 6469 6f20 7072 652d     .# Audio pre-
-00000300: 7072 6f63 6573 7369 6e67 2072 6561 6479  processing ready
-00000310: 2066 6f72 2074 7261 696e 0a20 2020 202d   for train.    -
-00000320: 2046 756e 6374 696f 6e20 436f 6e76 6572   Function Conver
-00000330: 7420 6672 6f6d 2061 7564 696f 2066 6f6c  t from audio fol
-00000340: 6465 7273 2074 6f20 7061 7271 7565 743a  ders to parquet:
-00000350: 200a 2020 2020 2020 6672 6f6d 2063 6164   .      from cad
-00000360: 732e 6e6f 7371 6c2e 636f 6e76 6572 7465  s.nosql.converte
-00000370: 7220 696d 706f 7274 2043 6f6e 7665 7274  r import Convert
-00000380: 546f 466f 6c64 6572 4175 6469 6f0a 2020  ToFolderAudio.  
-00000390: 2020 2d20 4675 6e63 7469 6f6e 2043 6f6e    - Function Con
-000003a0: 7665 7274 2066 726f 6d20 6175 6469 6f20  vert from audio 
-000003b0: 666f 6c64 6572 7320 746f 2070 6172 7175  folders to parqu
-000003c0: 6574 3a20 0a20 2020 2020 2066 726f 6d20  et: .      from 
-000003d0: 6361 6473 2e6e 6f73 716c 2e63 6f6e 7665  cads.nosql.conve
-000003e0: 7274 6572 2069 6d70 6f72 7420 436f 6e76  rter import Conv
-000003f0: 6572 7446 726f 6d46 6f6c 6465 7241 7564  ertFromFolderAud
-00000400: 696f 0a23 2056 6964 656f 0a20 2020 202d  io.# Video.    -
-00000410: 2046 756e 6374 696f 6e20 436f 6e76 6572   Function Conver
-00000420: 7420 6672 6f6d 2076 6964 656f 2066 696c  t from video fil
-00000430: 6573 2074 6f20 7061 7271 7565 7420 6f66  es to parquet of
-00000440: 2066 7261 6d65 3a20 0a20 2020 2020 2066   frame: .      f
-00000450: 726f 6d20 6361 6473 2e6e 6f73 716c 2e63  rom cads.nosql.c
-00000460: 6f6e 7665 7274 6572 2069 6d70 6f72 7420  onverter import 
-00000470: 436f 6e76 6572 7446 726f 6d56 6964 656f  ConvertFromVideo
-00000480: 3249 6d61 6765 0a20 2020 202d 2046 756e  2Image.    - Fun
-00000490: 6374 696f 6e20 746f 2064 6973 706c 6179  ction to display
-000004a0: 2066 7261 6d65 2070 6172 7175 6574 0a20   frame parquet. 
-000004b0: 2020 2020 2066 726f 6d20 6361 6473 2e6e       from cads.n
-000004c0: 6f73 716c 2e63 6f6e 7665 7274 6572 2069  osql.converter i
-000004d0: 6d70 6f72 7420 436f 6e76 6572 7446 726f  mport ConvertFro
-000004e0: 6d46 6f6c 6465 7241 7564 696f 0a22 2222  mFolderAudio."""
```

## cads_sdk/nosql/codec.py

```diff
@@ -1,15 +1,16 @@
-import spark_sdk as ss
 from pyspark.sql.types import StructField, StructType, IntegerType, BinaryType, StringType, TimestampType, FloatType
 
 from spark_sdk.utils import import_or_install
 import_or_install("petastorm")
 import petastorm
+from petastorm.etl.dataset_metadata import materialize_dataset
 from petastorm.codecs import ScalarCodec, NdarrayCodec #, CompressedImageCodec
 from petastorm.unischema import dict_to_spark_row, Unischema, UnischemaField
+from petastorm.codecs import ScalarCodec, CompressedImageCodec, NdarrayCodec
 
 from cads_sdk.nosql.etl import read_mp3,read_pcm
 from zipfile import ZipFile
 
 from abc import abstractmethod
 
 import numpy as np
@@ -104,15 +105,25 @@
                                    [int(cv2.IMWRITE_JPEG_QUALITY), self._quality])
         return bytearray(contents)
 
     def decode(self, unischema_field, value):
         """Decodes the image using OpenCV."""
         # cv returns a BGR or grayscale image. Convert to RGB (unless a grayscale image).
         image_bgr_or_gray = cv2.imdecode(np.frombuffer(value, dtype=np.uint8), cv2.IMREAD_UNCHANGED)
-        return image_bgr_or_gray
+        if len(image_bgr_or_gray.shape) == 2:
+            # Greyscale image
+            return image_bgr_or_gray
+        elif len(image_bgr_or_gray.shape) == 3 and image_bgr_or_gray.shape[2] == 3:
+            # Convert BGR to RGB (opencv assumes BGR)
+            # why here convert back?
+            # image_rgb = image_bgr_or_gray[:, :, (2, 1, 0)]
+            return image_rgb
+        else:
+            raise ValueError('Unexpected image dimensions. Supported dimensions are (H, W) or (H, W, 3). '
+                             'Got {}'.format(image_bgr_or_gray.shape))
 
     def spark_dtype(self):
         # Lazy loading pyspark to avoid creating pyspark dependency on data reading code path
         # (currently works only with make_batch_reader). We should move all pyspark related code into a separate module
         import pyspark.sql.types as sql_types
 
         return sql_types.BinaryType()
```

## cads_sdk/nosql/converter.py

```diff
@@ -16,216 +16,34 @@
     os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 opencv-python")
     import cv2
     OPENCV_AVAILABLE = False
     
     
 from zipfile import ZipFile
 
-from pyspark.sql.types import StructField, StructType, IntegerType, BinaryType, StringType, TimestampType, FloatType, LongType
-
-from petastorm.etl.dataset_metadata import materialize_dataset
-
-import warnings
-warnings.simplefilter(action='ignore', category=FutureWarning)
+from pyspark.sql.types import StructField, StructType, IntegerType, BinaryType, StringType, TimestampType, FloatType
 
 from cads_sdk.nosql.codec import *
 from cads_sdk.nosql.etl import read_mp3,read_pcm,padding
-from cads_sdk.nosql.utils import get_size_of_dir,get_size_of_list,check_delta
 
-class ConvertFromFolder:
-    def __init__(
-        self,
-        input_path,
-        input_type,
-        output_path,
-        table_name = '',
-        database = '',
-        repartition=False,
-        numPartition=None,
-        file_format = 'parquet',
-        compression = 'zstd',
-        input_recursive = False,
-        shorten = False,
-        
-        debug=False
-    ):
-        # input sesssion
-        self.input_path = input_path
-        self.input_type = input_type
-        self.input_recursive = input_recursive
-        
-        # output session
-        self.output_path = output_path
-        self.table_name = table_name
-        self.database = database
-        self.repartition = repartition
-        self.numPartition = numPartition
-        self.compression = compression
-        self.file_format = file_format
-        self.shorten = shorten
-        
-        self.debug = debug
-        
-        if debug:
-            self.temp_folder = tempfile.TemporaryDirectory(dir='./tmp_sdk')
-            self.tmp_file = os.path.join(self.temp_folder.name, 'sdk.log')
-            self.log_file = open(self.tmp_file, 'w+')
-            logging.basicConfig(level=logging.DEBUG, filename=self.tmp_file, filemode='w+')
-            
-        else:
-            logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.INFO)
-        
-        if '.delta' in output_path:
-            self.file_format = 'delta'
-        else:
-            self.file_format = file_format
-            
-        
-    def _generate_input_files(self):
-        if isinstance(self.input_path, str):
-            list_file = self.get_all_file_in_directory()
-        elif isinstance(self.input_path, (tuple, list)):
-            list_file = self.input_path
-        if self.shorten:
-            self.commonpath = os.path.commonpath(list_file)
-        return list_file
-    
-    def get_all_file_in_directory(self):
-        input_files = []
-        if isinstance(self.input_type, str):
-            if self.input_recursive:
-                self.input_path = os.path.join(self.input_path, "**")
-            self.input_path = os.path.join(self.input_path, "*."+self.input_type)
-            input_files = glob(self.input_path, recursive=self.input_recursive)
-            return input_files
-        elif isinstance(self.input_type, (tuple, list)):
-            for t in self.input_type:
-                if self.input_recursive:
-                    self.input_path = os.path.join(self.input_path, "**")
-                self.input_path = os.path.join(self.input_path, "*."+t)
-                input_files.extend(glob(self.input_path, recursive=self.input_recursive))
-            return input_files
-    
-    def convert_to_hdfs_path(self, input_path):
-        if "file:" in input_path:
-            return input_path
-        else:
-            if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
-                return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(input_path.replace("hdfs:", ""))
-            else:
-                return input_path
-            
-    def _generate_output_path(self):
-        if "." + self.file_format in self.output_path:
-            output_path = self.output_path
-        else:
-            output_path = self.output_path + f".{self.file_format}"
-        logging.info(f"Write at path: {output_path}")
-        return output_path
-
-    def _generate_table_name(self):
-        table_name = self.table_name
-        logging.info(f"Save metadata at: {table_name}")
-        return table_name
-            
-    def get_num_partition(self, ROWGROUP_SIZE_MB = 256):
-        if self.numPartition:
-            return self.numPartition
-        if isinstance(self.analyze_path, str):
-            memory = os.stat(self.analyze_path).st_size
-        elif isinstance(self.analyze_path, (tuple, list)):
-            memory = get_size_of_list(self.analyze_path)
-        else:
-            memory = 0
-        logging.info(f"Total folder memory: {memory}")
-        numPartition = int(round(memory/1024/1024/ROWGROUP_SIZE_MB))
-        if numPartition <= 8:
-            return None
-        else: 
-            return numPartition
-    
-    def coalesce_dataframe(self, spark_df, numPartition):
-        if self.file_format != 'delta':
-            numPartition = self.get_num_partition()
-            if numPartition:
-                if numPartition > 8:
-                    return spark_df.repartition(numPartition)
-                else:
-                    return spark_df.coalesce(numPartition)
-        return spark_df
-    
-    
-    def get_spark(self):
-        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False, 
-                         optimze_file_size=("spark.databricks.delta.optimize.maxFileSize", 268435456)).spark
-    
-    def create_dataframe(self, 
-                         spark, 
-                         Schema, 
-                         input_files):
-        from pyspark.sql.functions import expr
-        self.unischema = Schema
-        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
-        if self.shorten:
-            return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema()).withColumn("rel_path", expr(f"""replace(path, '{self.commonpath}', '') """))
-        else:
-            return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
-    
-    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
-        if '.parquet' in output_path.lower():
-            file_format = 'parquet'
-        else:
-            file_format = 'delta'
-            
-        if "file:" in output_path:
-            self.coalesce_dataframe(spark_df, numPartition).write \
-                .format(file_format) \
-                .option('compression', compression) \
-                .mode('overwrite') \
-                .option("path", output_path) \
-                .save()
-        else:
-            if table_name == '' or database == '':
-                raise ValueError("You must add table_name and database")
-            self.coalesce_dataframe(spark_df, numPartition).write \
-                .format(file_format) \
-                .option('compression', compression) \
-                .mode('overwrite') \
-                .option("path", output_path) \
-                .saveAsTable(database + '.' + table_name)
-        
-        if file_format == 'delta':
-            if self.shorten:
-                ss.sql(f"""
-                OPTIMIZE delta.`{output_path}` ZORDER BY(rel_path)
-                """)
-            
-            ss.sql(f"""
-            VACUUM delta.`{output_path}` RETAIN 0 HOURS
-            """)
-
-
-class ConvertFromFolderImage(ConvertFromFolder):
+class ConvertFromFolderImage:
     """
     Create a parquet/delta file given local Image directory
     
 
     Parameters
     ----------
     input_path : unicode, str 
         The input filename include ``png``, ``jpeg`` image
         User can add system file pattern like *
         Examples:
-        input_path="./path"
-        input_path="/home/username/path"
-        
-    input_type : unicode, str
-        str: 'jpg'
-        or
-        type: ('jpg', 'png')
+        input_path="**/*.jpg"
+        input_path="**/*.png"
+        This pattern get all jpg in folder with different directory levels
+        View https://docs.python.org/3/library/glob.html
 
     output_path : unicode
         Ouput directory location maybe file:/ (local file) or hdfs:/ (datalake path)
         Examples:
         output_path = "file:/home/username/"
         output_path = "hdfs:/user/username/"
         
@@ -247,28 +65,25 @@
     numPartition : int
         Default None
         Number of part each user want to seperate parquet file into
 
     file_format : str
         Default: parquet
         File format user want to write parquet/delta
-        IF user want to query table and filter faster: use delta
-        Function will auto optimize dataframe to best practice partition size and ZOrder by path
         
     compression: str 
         Default: zstd
         Compression method user want to compress parquet file
         Value: None, zstd, snappy
         See spark.sql.parquet.compression.codec
         https://spark.apache.org/docs/2.4.3/sql-data-sources-parquet.html
         
     image_type: str
         Default: jpg
         Value png or jpg
-        Or ('png', 'jpg')
         
     image_color : int
         Default: 3
         Value 3, 2 or 1, shape of image have color is 3 or 1 if gray image
         
     size : List of Tuple
         Default: jpg
@@ -279,208 +94,206 @@
         Default: None
         Value: None, padding, resize
         Mode of image user want to resize
         If in folder user have various size of image, 300, 400 500
         User will add size = 500:
         And resize_mode  = 'padding'
         Then function will convert all image 300, 400, 500 to shape of 500
-    
-    input_recursive : bool
-        Default: True
-        If True: 
-        will loop through folder to get all pattern
-        
-    shorten : bool
-        Default: False
-        If True: 
-        Create a column shorten of path that can be filter more quickly
 
     debug : bool
         If debug=True:
         Write log into sdk.log file and print more debug information
 
 
     Examples
     --------
     ::
         ```
         from cads_sdk.nosql.codec import ConvertFromFolderImage
 
         converter = ConvertFromFolderImage(
-                      input_path="/home/username/image_storage/images",
+                      input_path="/home/username/image_storage/images/**/*.jpg",
+                      input_recursive = True, # will loop through folder to get all pattern
                       #setting output
                       output_path = f"hdfs:/user/username/image/img_images_jpg.parquet",
                       table_name = 'img_images_jpg',
                       database = 'default',
                       file_format = 'parquet', # delta|parquet
-                      compression = 'zstd', # |snappy|zstd
+                      compression = 'zstd', # |snappy
                       # setting converter
                       image_type = 'jpg',
                       image_color = 3,
                       resize_mode="padding", # |padding|resize
                       size = [(212,212),
                              (597, 597)],
-                      input_recursive = True, # will loop through folder to get all pattern
                      )
 
         converter.execute()
         
         from cads_sdk.nosql.codec import ConvertFromFolderImage
 
         converter = ConvertFromFolderImage(
-                      input_path="/home/username/image_storage/device_images",
+                      input_path="/home/username/image_storage/device_images/**/*.jpg",
+                      input_recursive = True, # will loop through folder to get all pattern
+
                       #setting output
-                      output_path = f"file:/home/username/image/img_user_device_jpg.delta",
+                      output_path = f"hdfs:/user/username/image/img_user_device_jpg.delta",
                       table_name = 'img_user_device_jpg',
                       database = 'default',
                       file_format = 'delta', # |parquet
-                      compression = 'zstd', # |snappy|zstd
+                      compression = 'zstd', # |snappy
 
                       # setting converter
-                      image_type = 'jpg', # |'png'|('jpg', 'png')
+                      image_type = 'jpg',
                       image_color = 3,
                       resize_mode=None, # |padding|resize
                       size = [(212,212),
                              (597, 597)],
-                      input_recursive = True, # will loop through folder to get all pattern
                      )
 
         converter.execute()
         ```
         
-        Function will convert all Image in file:'/home/username/device_images/' to absolute directory file:/home/username/image/img_images_jpg.parquet
+        Function will convert all Image in file:'/home/username/device_images/' to absolute directory hdfs:/user/username/image/img_images_jpg.parquet
     """
    
     def __init__(
         self,
         input_path,
-        input_type,
         output_path,
         table_name = '',
         database = '',
         repartition=False,
         numPartition=None,
         file_format = 'parquet',
         compression = 'zstd',
         
         image_type = 'jpg',
         image_color = 3,
         size=[(720,360)],
         resize_mode=None,
-        input_recursive = False,
-        shorten = False,
         
+        input_recursive = False,
         debug=False
     ):
+        
+        self.input_path = input_path
+        self.output_path = output_path
+        self.table_name = table_name
+        self.database = database
+        self.input_recursive = input_recursive
         self.image_type = image_type
         self.image_color = image_color
         self.size = size
         self.resize_mode = resize_mode
+        self.repartition = repartition
+        self.numPartition = numPartition
+        self.compression = compression
+        self.file_format = file_format
         
+        self.debug = debug
         
-        super().__init__(input_path=input_path,
-                        input_type=input_type,
-                        output_path=output_path,
-                        table_name=table_name,
-                        database=database,
-                        repartition=repartition,
-                        numPartition=numPartition,
-                        file_format=file_format,
-                        compression=compression,
-                        input_recursive=input_recursive,
-                        shorten=shorten,
-                        debug=debug)
-        
-        if isinstance(self.input_type, (tuple, list)):
-            self.image_type = 'jpg'
+        if debug:
+            self.temp_folder = tempfile.TemporaryDirectory(dir='./tmp_sdk')
+            self.tmp_file = os.path.join(self.temp_folder.name, 'sdk.log')
+            self.log_file = open(self.tmp_file, 'w+')
+            logging.basicConfig(level=logging.DEBUG, filename=self.tmp_file, filemode='w+')
             
-    # specific function for image
-    def _generate_output_path(self, s):
-        if self.resize_mode:
-            if "." + self.file_format in self.output_path:
-                output_path = self.output_path.replace("." + self.file_format, "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format))
-            else:
-                output_path = self.output_path + "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format)
         else:
-            if "." + self.file_format in self.output_path:
-                output_path = self.output_path
+            logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.INFO)
+            
+    def convert_to_hdfs_path(self, input_path):
+        if "file:" in input_path:
+            return input_path
+        else:
+            if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
+                return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(input_path.replace("hdfs:", ""))
             else:
-                output_path = self.output_path + f".{self.file_format}"
-        logging.info(f"Write at path: {output_path}")
-        return output_path
+                return input_path
 
-    def _generate_table_name(self, s):
-        if self.resize_mode:
-            if self.table_name:
-                table_name = self.table_name + "_{s0}_{s1}".format(s0=str(s[0]), s1=str(s[1]))
-            else:
-                table_name = ''
+    
+    def coalesce_dataframe(self, spark_df, numPartition):
+        if numPartition:
+            return spark_df.coalesce(numPartition)
+        return spark_df
+    
+    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
+        if '.parquet' in output_path.lower():
+            file_format = 'parquet'
         else:
-            table_name = self.table_name
-        logging.info(f"Save metadata at: {table_name}")
-        return table_name
+            file_format = 'delta'
             
-    def create_dataframe(self, 
-                         spark, 
-                         Schema, 
-                         input_files,
-                         size):
-        from pyspark.sql.functions import expr
-        self.unischema = Schema
-        self.s = size
-        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
-        if not self.resize_mode:
-            logging.warning(f"Not resize image, If get size error try to turn resize_mode='padding' or resize_mode='resize'")
-        if self.shorten:
-            return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema()).withColumn("rel_path", expr(f"""replace(path, '{self.commonpath}', '') """))
+        if "file:" in output_path:
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .save()
         else:
-            return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
-        
+            if table_name == '' or database == '':
+                raise ValueError("You must add table_name and database")
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .saveAsTable(database + '.' + table_name)
+          
+    
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""
         for row in partitionData:
             path = row.path
             if self.debug:
                 print(f"Convert Image {path}") #, file=self.log_file)
                 
             img = cv2.imread(path)
-            if type(img).__name__ != "NoneType":
-                if self.resize_mode == 'padding':
-                    row_dict = {
-                        'path': path,
-                        'size': img.shape.__str__(),
-                        'image': padding(img, (self.s[0], self.s[1]))
-                    }
-
-                    yield dict_to_spark_row(self.unischema, row_dict)
-                elif self.resize_mode == 'resize':
-                    row_dict = {
-                        'path': path,
-                        'size': img.shape.__str__(),
-                        'image': cv2.resize(img, (self.s[0], self.s[1]))
-                    }
+            if self.resize_mode == 'padding':
+                row_dict = {
+                    'path': path,
+                    'size': f"{img.shape[0]}, {img.shape[1]}",
+                    'image': padding(img, (self.s[0], self.s[1]))
+                }
 
-                    yield dict_to_spark_row(self.unischema, row_dict)
-                else:
-                    row_dict = {
-                        'path': path,
-                        'size': img.shape.__str__(),
-                        'image': open(path, 'rb').read()
-                    }
+                yield dict_to_spark_row(self.unischema, row_dict)
+            elif self.resize_mode == 'resize':
+                row_dict = {
+                    'path': path,
+                    'size': f"{img.shape[0]}, {img.shape[1]}",
+                    'image': cv2.resize(img, (self.s[0], self.s[1]))
+                }
 
-                    yield dict_to_spark_row(self.unischema, row_dict)
+                yield dict_to_spark_row(self.unischema, row_dict)
             else:
                 row_dict = {
                     'path': path,
-                    'size': "Can not get size",
+                    'size': f"{img.shape[0]}, {img.shape[1]}",
                     'image': open(path, 'rb').read()
                 }
 
                 yield dict_to_spark_row(self.unischema, row_dict)
-       
+
+                
+    def create_dataframe(self, 
+                         spark, 
+                         Schema, 
+                         input_files,
+                         size):
+        
+
+        self.unischema = Schema
+        self.s = size
+        
+        
+        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
+        if not self.resize_mode:
+            logging.warning(f"Not resize image, If get size error try to turn resize_mode='padding' or resize_mode='resize'")
+        return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
+                
                     
     def create_image_schema(self, size, image_type, image_color):
         """
         :param size: Image size, schema need to be consistency
         :param image_type: Image type is compress JPG or PNG
         :param image_color: 3 dimention color or 1 dimention colors
         """
@@ -495,74 +308,81 @@
             return Unischema('ImageSchema', [
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('size', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('image', np.bytes_, (size[0], size[1], image_color), ImageZipCodec(BinaryType()), False)
         ])
     
     
+    
+    def get_spark(self):
+        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
+    
+    
     def check_size(self, img, list_size):
-        """
-        Check size of image to put it in different table
-        """
         for s in list_size:
             if img.shape[0] <= s[0] and img.shape[1] <= s[1]:
                 return s
         self.size.append(s)
         self.dict_image[(img.shape[0], img.shape[1])] = []
-        return s
-
+        return a
+        #return (img.shape[0], img.shape[1])
+    
     
-    def execute(self, ROWGROUP_SIZE_MB = 256):
+    def execute(self):
         self.dict_image = {}
+        ROWGROUP_SIZE_MB = 128
+        
         for s in self.size:
             self.dict_image[s] = []
-            
-        if self.resize_mode:
-            if len(self.size) == 0:
-                raise ValueError("User must input size when using resize_mode")
-            
-            list_file = self._generate_input_files()
-            
-            # classify image into each size in list
-            for p in list_file:
+        
+        if self.resize_mode and len(self.size) > 1:
+            for p in sorted(glob(self.input_path, recursive=self.input_recursive)):
                 img = cv2.imread(p)
-                if type(img).__name__ != "NoneType":
-                    self.dict_image[self.check_size(img, self.size)].append(p)
+                self.dict_image[self.check_size(img, self.size)].append(p)
         else:
-            self.dict_image[self.size[0]] = self._generate_input_files()
+            self.dict_image[self.size[0]] = sorted(glob(self.input_path, recursive=self.input_recursive))
 
         for s in self.size:
+            self.output_path = self.convert_to_hdfs_path(self.output_path)
+            if "." + self.file_format in self.output_path:
+                output_path = self.output_path.replace("." + self.file_format, "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format))
+            else:
+                output_path = self.output_path + "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format)
+            
+            if self.table_name:
+                table_name = self.table_name + "_{s0}_{s1}".format(s0=str(s[0]), s1=str(s[1]))
+            else:
+                table_name = ''
+            
+            spark = self.get_spark()
+
+            Schema = self.create_image_schema(s, self.image_type, self.image_color)
             if self.dict_image[s]:
-                self.analyze_path = self.dict_image[s]
-                Schema = self.create_image_schema(s, self.image_type, self.image_color)
-                self.output_path = self.convert_to_hdfs_path(self.output_path)
-                output_path = self._generate_output_path(s)
-                table_name = self._generate_table_name(s)
-                spark = self.get_spark()
-                
+                logging.info(f"Write at path: {output_path}")
+                logging.info(f"Save metadata at: {table_name}")
                 with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
                     self.write_to_path(spark_df = self.create_dataframe(spark=spark,
                                           Schema=Schema,
                                           input_files=self.dict_image[s],
                                           size=s),
 
                                     output_path = output_path,
                                     table_name = table_name, 
                                     database = self.database,
                                     numPartition = self.numPartition,
                                     compression = self.compression)
-                    
-        total_files = sum([len(self.dict_image[s]) for s in self.size])
-        if total_files==0:
-            logging.warn("No files were found, check your input_path or image_type")
+        total_image = 0
+        for s in self.size:
+            total_image += len(self.dict_image[s])
+            if total_image==0:
+                logging.warn("No files were found, check your input_path")
                 
         logging.info("Convert complete")
-        
-        
-class ConvertFromZipImage(ConvertFromFolderImage):
+                
+class ConvertFromZipImage:
     """
     Create a parquet/delta file given local Image directory
     
 
     Parameters
     ----------
     input_path : unicode, str 
@@ -626,479 +446,314 @@
         Default: None
         Value: None, padding, resize
         Mode of image user want to resize
         If in folder user have various size of image, 300, 400 500
         User will add size = 500:
         And resize_mode  = 'padding'
         Then function will convert all image 300, 400, 500 to shape of 500
-        
-    shorten : bool
-        Default: False
-        If True: 
-        Create a column shorten of path that can be filter more quickly
-        
+
     debug : bool
         If debug=True:
         Write log into sdk.log file and print more debug information
 
 
     Examples
     --------
     ::
         ```
         from cads_sdk.nosql.codec import ConvertFromZipImage
 
         converter = ConvertFromZipImage(
                       input_path="/home/username/image_storage/MOT17.zip",
-                      
+                      input_recursive = True, # will loop through folder to get all pattern
                       #setting output
                       output_path = f"hdfs:/user/username/image/img_images_jpg.parquet",
                       table_name = 'img_images_jpg',
                       database = 'default',
                       file_format = 'parquet', # delta|parquet
-                      compression = 'zstd', # |snappy|zstd
+                      compression = 'zstd', # |snappy
                       # setting converter
-                      image_type = 'jpg', # |'png'|('jpg', 'png')
+                      image_type = 'jpg',
                       image_color = 3,
                       resize_mode=None, # |padding|resize
-                      size = [(212,212)],
-                      
-                      input_recursive = True, # will loop through folder to get all pattern
+                      size = [(212,212),
+                             (597, 597)],
                      )
 
         converter.execute()
         ```
         
         Function will convert all Image in file:'/home/username/image_storage/MOT17.zip' to absolute directory hdfs:/user/username/image/img_images_jpg.parquet
     """
    
         
     def __init__(
         self,
         input_path,
-        input_type,
         output_path,
         table_name = '',
         database = '',
         repartition=False,
         numPartition=None,
         file_format = 'parquet',
         compression = 'zstd',
         
         image_type = 'jpg',
         image_color = 3,
         size=[(720,360)],
         resize_mode=None,
-        input_recursive = False,
-        
-        shorten = False,
         
+        input_recursive = False,
         debug=False
     ):
         
-        super().__init__(input_path=input_path,
-                        input_type=input_type,
-                        output_path=output_path,
-                        table_name=table_name,
-                        database=database,
-                        repartition=repartition,
-                        numPartition=numPartition,
-                        file_format=file_format,
-                        compression=compression,
-                        image_type=image_type,
-                        image_color=image_color,
-                        size=size,
-                        resize_mode=resize_mode,
-                        input_recursive=input_recursive,
-                        shorten=shorten,
-                        debug=debug)
+        self.input_path = input_path
+        self.output_path = output_path
+        self.table_name = table_name
+        self.database = database
+        self.input_recursive = input_recursive
+        self.image_type = image_type
+        self.image_color = image_color
+        self.size = size
+        self.resize_mode = resize_mode
+        self.repartition = repartition
+        self.numPartition = numPartition
+        self.compression = compression
+        self.file_format = file_format
+        
+        self.debug = debug
         
-    def _generate_input_files(self):
-        list_file = []
-        for i in self.input_files:
-            if isinstance(self.input_type, str):
-                if i.endswith('.'+self.input_type):
-                    list_file.append(i)
-            elif isinstance(self.input_type, (list, tuple)):
-                for t in self.input_type:
-                    if '.'+t in i:
-                        list_file.append(i)
-        if self.shorten:
-            self.commonpath = os.path.commonpath(list_file)
-        return list_file
-    
+        if debug:
+            self.temp_folder = tempfile.TemporaryDirectory(dir='./tmp_sdk')
+            self.tmp_file = os.path.join(self.temp_folder.name, 'sdk.log')
+            self.log_file = open(self.tmp_file, 'w+')
+            logging.basicConfig(level=logging.DEBUG, filename=self.tmp_file, filemode='w+')
+            
+        else:
+            logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.INFO)
+            
+    def convert_to_hdfs_path(self, input_path):
+        if "file:" in input_path:
+            return input_path
+        else:
+            if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
+                return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(input_path.replace("hdfs:", ""))
+            else:
+                return input_path
         
+    
+    
+    def coalesce_dataframe(self, spark_df, numPartition):
+        if numPartition:
+            return spark_df.coalesce(numPartition)
+        return spark_df
+    
+    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
+        if '.parquet' in output_path.lower():
+            file_format = 'parquet'
+        else:
+            file_format = 'delta'
+            
+        if "file:" in output_path:
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .save()
+        else:
+            if table_name == '' or database == '':
+                raise ValueError("You must add table_name and database")
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .saveAsTable(database + '.' + table_name)
+            
+            
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""          
         for row in partitionData:
             path = row.path
             if self.debug:
                 print(f"Convert Image {path}") #, file=self.log_file)
                 
             with ZipFile(self.input_path, 'r') as zipObj:
-                memfile = zipObj.read(path)
-                img = cv2.imdecode(np.frombuffer(memfile, dtype=np.uint8), cv2.IMREAD_UNCHANGED)
-                if type(img).__name__ != "NoneType":
-                    if self.resize_mode == 'padding':
-                        if img.shape[0] < self.s[0]:
-                            row_dict = {
-                                'path': path,
-                                'size': img.shape.__str__(),
-                                'image': padding(img, (self.s[0], self.s[1]))
-                            }
-                            yield dict_to_spark_row(self.unischema, row_dict)
-                        else:
-                            row_dict = {
-                                'path': path,
-                                'size': img.shape.__str__(),
-                                'image': img
-                            }
-                            yield dict_to_spark_row(self.unischema, row_dict)
-
-                    elif self.resize_mode == 'resize':
-                        if img.shape[0] < self.s[0]:
-                            row_dict = {
-                                'path': path,
-                                'size': img.shape.__str__(),
-                                'image': cv2.resize(img, (self.s[0], self.s[1]))
-                            }
-                            yield dict_to_spark_row(self.unischema, row_dict)
-                        else:
-                            row_dict = {
-                                'path': path,
-                                'size': img.shape.__str__(),
-                                'image': img
-                            }
-                            yield dict_to_spark_row(self.unischema, row_dict)
-
+                img = cv2.imdecode(np.frombuffer(zipObj.read(path), dtype=np.uint8), cv2.IMREAD_UNCHANGED)
+                if self.resize_mode == 'padding':
+                    if img.shape[0] < self.s[0]:
+                        row_dict = {
+                            'path': path,
+                            'size': f"{img.shape[0]}, {img.shape[1]}",
+                            'image': padding(img, (self.s[0], self.s[1]))
+                        }
+                        yield dict_to_spark_row(self.unischema, row_dict)
                     else:
                         row_dict = {
+                        'path': path,
+                        'image': img
+                        }
+                        yield dict_to_spark_row(self.unischema, row_dict)
+
+                elif self.resize_mode == 'resize':
+                    if img.shape[0] < self.s[0]:
+                        row_dict = {
                             'path': path,
-                            'size': img.shape.__str__(),
-                            'image': memfile
+                            'size': f"{img.shape[0]}, {img.shape[1]}",
+                            'image': cv2.resize(img, (self.s[0], self.s[1]))
+                        }
+                        yield dict_to_spark_row(self.unischema, row_dict)
+                    else:
+                        row_dict = {
+                        'path': path,
+                        'size': f"{img.shape[0]}, {img.shape[1]}",
+                        'image': img
                         }
                         yield dict_to_spark_row(self.unischema, row_dict)
+
                 else:
                     row_dict = {
                         'path': path,
-                        'size': "Can not get size",
-                        'image': memfile
+                        'size': f"{img.shape[0]}, {img.shape[1]}",
+                        'image': zipObj.read(path)
                     }
-
                     yield dict_to_spark_row(self.unischema, row_dict)
+
+
+    def create_dataframe(self, 
+                         spark, 
+                         Schema, 
+                         input_files,
+                         size):
+        
+        self.unischema = Schema
+        self.s = size
+        
+        # with materialize_dataset(spark, output_path, ImageSchema, ROWGROUP_SIZE_MB):
+        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
+        if not self.resize_mode:
+            logging.warning(f"Not resize image, If get size error try to turn resize_mode='padding' or resize_mode='resize'")
+        return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
+                
+                    
+    def create_image_schema(self, size, image_type, image_color):
+        """
+        :param size: Image size, schema need to be consistency
+        :param image_type: Image type is compress JPG or PNG
+        :param image_color: 3 dimention color or 1 dimention colors
+        """
+        if self.resize_mode:
+            return Unischema('ImageSchema', [
+            UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
+            UnischemaField('size', np.str_, (), ScalarCodec(StringType()), False),
+            UnischemaField('image', np.bytes_, (size[0], size[1], image_color), ImageZipCodec(BinaryType()), False)
+        ])
+        
+        return Unischema('ImageSchema', [
+            UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
+            UnischemaField('size', np.str_, (), ScalarCodec(StringType()), False),
+            UnischemaField('image', np.bytes_, (size[0], size[1], image_color), ImageZipCodec(BinaryType()), False)
+        ])
+    
+    
+    
+    def get_spark(self):
+        return ss.PySpark(driver_memory='16G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
+    
     
+    def check_size(self, img, list_size):
+        for s in list_size:
+            if img.shape[0] <= s[0] and img.shape[1] <= s[1]:
+                return s
+        self.size.append(s)
+        self.dict_image[(img.shape[0], img.shape[1])] = []
+        return a
+        #return (img.shape[0], img.shape[1])
     
-    def execute(self, ROWGROUP_SIZE_MB = 128):
+    
+    def execute(self):
         self.dict_image = {}
-
+        ROWGROUP_SIZE_MB = 128
+        
         with ZipFile(self.input_path, 'r') as zipObj:
             self.input_files = zipObj.namelist()
         logging.info(f"Total file in zip: {len(self.input_files)}")
         
         for s in self.size:
             self.dict_image[s] = []
         
-        self.dict_image[self.size[0]] = self._generate_input_files()
-        
-        if self.dict_image[s]:
-            self.analyze_path = self.input_path
-            Schema = self.create_image_schema(s, self.image_type, self.image_color)
-            self.output_path = self.convert_to_hdfs_path(self.output_path)
-            output_path = self._generate_output_path(s)
-            table_name = self._generate_table_name(s)
-            spark = self.get_spark()
-
-            with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=self.dict_image[s],
-                                      size=s),
-
-                                output_path = output_path,
-                                table_name = table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
-
-        total_files = sum([len(self.dict_image[s]) for s in self.size])
-        if total_files==0:
-            logging.warn("No files were found, check your input_path or image_type")
-                
-        logging.info("Convert complete")
-        
-
-class MergeFromFolderImage(ConvertFromFolderImage):
-    """
-    Create a parquet/delta file given local Image directory
-    
-
-    Parameters
-    ----------
-    input_path : unicode, str 
-        The input directory include ``png``, ``jpeg`` image
-        User can add system file pattern like *
-        Examples:
-        input_path="/path/to/MOT17.zip"
-        This pattern get all jpg in folder with different directory levels
-        View https://docs.python.org/3/library/glob.html
-
-    output_path : unicode
-        Ouput directory location maybe file:/ (local file) or hdfs:/ (datalake path)
-        Examples:
-        output_path = "file:/home/username/"
-        output_path = "hdfs:/user/username/"
-        
-    table_name : str
-        Table_name store metadata
-        User should input table_name follow dwh convention: img_abc, vid_abc, audio_abc
-        Examples: img_abc
-        
-    database : str
-        Database to store metadata
-        User should input database follow dwh convention: default
-        Examples: default
-        
-
-    repartition : bool 
-        Default: False
-        Data will be repartition to target file size
-        
-    numPartition : int
-        Default None
-        Number of part each user want to seperate parquet file into
-
-    file_format : str
-        Default: parquet
-        File format user want to write parquet/delta
-        
-    compression: str 
-        Default: zstd
-        Compression method user want to compress parquet file
-        Value: None, zstd, snappy
-        See spark.sql.parquet.compression.codec
-        https://spark.apache.org/docs/2.4.3/sql-data-sources-parquet.html
-        
-    image_type : str
-        Default: jpg
-        Value png or jpg
-        
-    image_color : int
-        Default: 3
-        Value 3, 2 or 1, shape of image have color is 3 or 1 if gray image
-        
-    size : List of Tuple
-        Default: jpg
-        List size user want to resize or padding
-        Examples: size = [(320, 180), (500, 100)]
-        
-    resize_mode : str
-        Default: None
-        Value: None, padding, resize
-        Mode of image user want to resize
-        If in folder user have various size of image, 300, 400 500
-        User will add size = 500:
-        And resize_mode  = 'padding'
-        Then function will convert all image 300, 400, 500 to shape of 500
-
-    debug : bool
-        If debug=True:
-        Write log into sdk.log file and print more debug information
-
-
-    Examples
-    --------
-    ::
-        ```
-        from cads_sdk.nosql.converter import ConvertFromZipImage
-
-        converter = ConvertFromZipImage(
-                      input_path="/home/username/image_storage/MOT17.zip",
-                      
-                      #setting output
-                      output_path = f"hdfs:/user/username/image/img_images_jpg.parquet",
-                      table_name = 'img_images_jpg',
-                      database = 'default',
-                      file_format = 'parquet', # delta|parquet
-                      compression = 'zstd', # |snappy|zstd
-                      # setting converter
-                      image_type = 'jpg', # |'png'|('jpg', 'png')
-                      image_color = 3,
-                      resize_mode=None, # |padding|resize
-                      size = [(212,212)],
-                      
-                      input_recursive = True, # will loop through folder to get all pattern
-                     )
-
-        converter.execute()
-        ```
-        
-        Function will convert all Image in file:'/home/username/image_storage/MOT17.zip' to absolute directory hdfs:/user/username/image/img_images_jpg.parquet
-    """
-   
-        
-    def __init__(
-        self,
-        input_path,
-        input_type,
-        output_path,
-        table_name = '',
-        database = '',
-        repartition=False,
-        numPartition=None,
-        file_format = 'delta',
-        compression = 'zstd',
-        
-        image_type = 'jpg',
-        image_color = 3,
-        size=[(720,360)],
-        resize_mode=None,
-        input_recursive = False,
-        
-        shorten=False,
-        merge_keys = ['path'],
-        
-        debug=False
-    ):
-        
-        super().__init__(input_path=input_path,
-                         input_type=input_type,
-                        output_path=output_path,
-                        table_name=table_name,
-                        database=database,
-                        repartition=repartition,
-                        numPartition=numPartition,
-                        file_format=file_format,
-                        compression=compression,
-
-                        image_type=image_type,
-                        image_color=image_color,
-                        size=size,
-                        resize_mode=resize_mode,
-                        input_recursive=input_recursive,
-                        shorten=shorten,
-                        debug=debug)
-        self.merge_keys = merge_keys
-
-    
-    def check_output(self, output_path):
-        if not ss.exists(output_path):
-            raise ValueError(f"Path {output_path} is not exists, you can only merge with exists path")
-            
-        if not check_delta(output_path):
-            raise ValueError(f"Path {output_path} is not a delta table, you can only merge with delta table")
-                    
-    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
-        if '.parquet' in output_path.lower():
-            file_format = 'delta'
-        else:
-            file_format = 'delta'
-        
-        spark_df.createOrReplaceTempView('new')
-        # Merge new dataframe image into old dataframe
+        for i in self.input_files:
+            if i.endswith('.'+self.image_type):
+                self.dict_image[self.size[0]].append(i)
         
-        sql_compare = ''
-        for k in self.merge_keys:
-            sql_compare+= f"""NVL(o.{k},'') = NVL(n.{k},'')"""
-            
-        ss.sql(f"""
-          MERGE INTO delta.`{output_path}` o
-          USING new n ON
-          {sql_compare}
-            
-          WHEN NOT MATCHED
-          THEN INSERT *
-        """)
-        
-        if file_format == 'delta':
-            ss.sql(f"""
-            OPTIMIZE delta.`{output_path}` ZORDER BY(path)
-            """)
-            
-            ss.sql(f"""
-            VACUUM delta.`{output_path}` RETAIN 0 HOURS
-            """)
-    
-    def execute(self, ROWGROUP_SIZE_MB = 256):
-        self.dict_image = {}
-
-
-        for s in self.size:
-            self.dict_image[s] = []
-            
-        if self.resize_mode:
-            if len(self.size) == 0:
-                raise ValueError("User must input size when using resize_mode")
-            
-            list_file = self._generate_input_files()
-            
-            # classify image into each size in list
-            for p in list_file:
-                img = cv2.imread(p)
-                self.dict_image[self.check_size(img, self.size)].append(p)
-        else:
-            self.dict_image[self.size[0]] = self._generate_input_files()
-
         for s in self.size:
             if self.dict_image[s]:
-                Schema = self.create_image_schema(s, self.image_type, self.image_color)
-                self.numPartition = self.get_num_partition(self.dict_image[s])
                 self.output_path = self.convert_to_hdfs_path(self.output_path)
-                output_path = self._generate_output_path(s)
-                self.check_output(output_path)
-                table_name = self._generate_table_name(s)
+                if "." + self.file_format in self.output_path:
+                    output_path = self.output_path.replace("." + self.file_format, "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format))
+                else:
+                    output_path = self.output_path + "_{s0}_{s1}.{file_format}".format(s0=str(s[0]), s1=str(s[1]), file_format=self.file_format)
+
+                if self.table_name:
+                    table_name = self.table_name + "_{s0}_{s1}".format(s0=str(s[0]), s1=str(s[1]))
+                else:
+                    table_name = ''
+
                 spark = self.get_spark()
-                
+
+                Schema = self.create_image_schema(s, self.image_type, self.image_color)
+                # if self.dict_image[s]:
+                logging.info(f"Write at path: {output_path}")
+                logging.info(f"Save metadata at: {table_name}")
                 with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
                     self.write_to_path(spark_df = self.create_dataframe(spark=spark,
                                           Schema=Schema,
                                           input_files=self.dict_image[s],
                                           size=s),
 
                                     output_path = output_path,
                                     table_name = table_name, 
                                     database = self.database,
                                     numPartition = self.numPartition,
                                     compression = self.compression)
-        total_files = sum([len(self.dict_image[s]) for s in self.size])
-        if total_files==0:
-            logging.warn("No files were found, check your input_path or image_type")
+                
+        total_image = 0
+        for s in self.size:
+            total_image += len(self.dict_image[s])
+            if total_image==0:
+                logging.warn("No files were found, check your input_path or image_type")
                 
         logging.info("Convert complete")
         
         
 class ConvertToFolderImage:
     """
     Create a folder Image given hdfs_path/local_path or pyspark.sql.dataframe.DataFrame
     
 
     Parameters
     ----------
     data : unicode, str or pyspark.sql.dataframe.DataFrame
-        The input (parquet) filename or dataframe include Image
-        Example: df, 'file:/absolute/path/to/file.parquet'
+        The input filename to load Image or dataframe include Image
 
     input_path : unicode
-        Path to a local file (parquet) or hdfs file containing the Image.
-        Example: df, 'file:/absolute/path/to/file.parquet'
+        Path to a local file or hdfs file containing the Image.
         
     output_path : unicode
-        Path to a local file that function execute() will convert parquet/delta back to a Image file (jpg, png)
-        Examples:
-        output_path = "/home/username/tmp"
+        Path to a local file that function execute() will convert parquet/delta back to a Image file (jpg, png) 
 
     write_mode : str
-        Default: 'recovery'
         Specify the write_mode user want to
         If write_mode = 'recovery' 
         Function will convert Image to a multiple level of directory base on column path
         If write_mode != 'recovery'
         Function will convert all Image in parquet/hdfs file to one directory (output_path)
 
     raw_input_path : str
-    
         Glob path that user input when use ConvertFromFolderVideo function
         For example: "/home/username/image_storage/images/**/*.jpg"
         When output it will replace '/home/username/image_storage/images/'  by ''
         That turn column path from absolute path to relative path
         
     keep_origin_jpg: bool | default False
         JPG is a lossly format when cv2 read jpg convert to array cv2.imread()
@@ -1180,15 +835,21 @@
         if "file:" in input_path:
             return input_path
         else:
             if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
                 return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(self.input_path.replace("hdfs:", ""))
             else:
                 return input_path
-
+            
+    def check_delta(self, input_path):
+        list_file = ss.ls(input_path)
+        for f in list_file:
+            if '_delta_log' in f:
+                return True
+        return False
         
     def mkdir_folder(self, output_path):
         if not os.path.exists(output_path):
             os.makedirs(output_path)
             
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
@@ -1218,15 +879,15 @@
             
     def execute(self):
         self.mkdir_folder(os.path.dirname(self.output_path))
         spark = self.get_spark()
         if self.data:
             self.data.foreach(self.write_abtract)
         else:
-            if check_delta(self.input_path):
+            if self.check_delta(self.input_path):
                 logging.info("Detect Delta File")
                 df = ss.sql(f"""select * from delta.`{self.input_path}`""")
             else:
                 df = ss.sql(f"""select * from parquet.`{self.input_path}`""")
             df.foreach(self.write_to_folder)
         logging.info("Convert complete")
             
@@ -1237,50 +898,103 @@
 from abc import abstractmethod
 from io import BytesIO
 import logging
 
 import numpy as np
 import zlib
 
-class ConvertFromFolderVideo(ConvertFromFolder):
+class ConvertFromFolderVideo:
     def __init__(
         self,
         input_path,
-        input_type,
         output_path,
         table_name = '',
         database = '',
         repartition=True,
         numPartition=None,
         file_format = 'parquet',
         compression = 'zstd',
-        input_recursive = True,
+        input_recursive = False,
         thumbnail_width = 256,
         thumbnail_height = 144,
-        
-        shorten = False,
+
         
         debug=False
     ):
-        super().__init__(input_path=input_path,
-                input_type=input_type,
-                output_path=output_path,
-                table_name=table_name,
-                database=database,
-                repartition=repartition,
-                numPartition=numPartition,
-                file_format=file_format,
-                compression=compression,
-                input_recursive=input_recursive,
-                shorten=shorten,
-                debug=debug)
         
+        self.input_path = input_path
+        self.output_path = output_path
+        self.table_name = table_name
+        self.database = database
+        self.input_recursive = input_recursive
+        self.repartition = repartition
+        self.numPartition = numPartition
+        self.compression = compression
+        self.file_format = file_format
         
         self.thumbnail_width = thumbnail_width
         self.thumbnail_height = thumbnail_height
+        
+        self.debug = debug
+        
+        if debug:
+            self.temp_folder = tempfile.TemporaryDirectory(dir='./tmp_sdk')
+            self.tmp_file = os.path.join(self.temp_folder.name, 'sdk.log')
+            self.log_file = open(self.tmp_file, 'w+')
+            logging.basicConfig(level=logging.DEBUG, filename=self.tmp_file, filemode='w+')
+        else:
+            logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.INFO)
+            
+            
+    def convert_to_hdfs_path(self, input_path):
+        if "file:" in input_path:
+            return input_path
+        else:
+            if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
+                return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(input_path.replace("hdfs:", ""))
+            else:
+                return input_path
+
+    def coalesce_dataframe(self, spark_df, numPartition):
+        if numPartition:
+            return spark_df.coalesce(numPartition)
+        return spark_df
+    
+    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
+        if '.parquet' in output_path.lower():
+            file_format = 'parquet'
+        else:
+            file_format = 'delta'
+            
+        if "file:" in output_path:
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .save()
+        else:
+            if table_name == '' or database == '':
+                raise ValueError("You must add table_name and database")
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .saveAsTable(database + '.' + table_name)
+            
+            #     pass
+            # spark_df.coalesce(numPartition) \
+            #         .write \
+            #         .format(file_format) \
+            #         .option('compression', compression) \
+            #         .mode('overwrite') \
+            #         .option("path", output_path) \
+            #         .save()
+               
 
 
             
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""
         for row in partitionData:
             path = row.path
@@ -1289,50 +1003,54 @@
 
             cap = cv2.VideoCapture(path)
             frame_size = (int(cap.get(3)), int(cap.get(4)))
             frame_number = cap.get(cv2.CAP_PROP_FRAME_COUNT) / 2
             cap.set(cv2.CAP_PROP_POS_FRAMES, frame_number-1)
             res, frame = cap.read()
             frame = cv2.resize(frame, (self.thumbnail_width, self.thumbnail_height))
-            # frame = frame[:, :, (2, 1, 0)]
+            frame = frame[:, :, (2, 1, 0)]
             duration = cap.get(cv2.CAP_PROP_FRAME_COUNT)/cap.get(cv2.CAP_PROP_FPS)
             
             row_dict = {
                 'path': path,
                 'thumbnail': frame,
                 'duration': duration,
                 'frame_size': str(frame_size),
                 'video': open(path, "rb").read()}
             
             yield dict_to_spark_row(self.unischema, row_dict)
     
+    def create_dataframe(self, spark, Schema, input_files):
+        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
+        self.unischema = Schema
+        return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
+        
+    def get_spark(self):
+        return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
+    
     def get_schema(self):
         return Unischema('VideoShema', [
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('thumbnail', np.uint8, (self.thumbnail_height, self.thumbnail_width, 3), CompressedImageCodec('.jpg'), False),
             UnischemaField('duration', np.float_, (), ScalarCodec(FloatType()), False),
             UnischemaField('frame_size', np.str_, (), ScalarCodec(StringType()), False),
-            UnischemaField('video', np.bytes_, (), VideoCodec(), False)
+            UnischemaField('video', np.bytes_, (), petastorm.codecs.VideoCodec(), False)
         ])
     
-    def execute(self, ROWGROUP_SIZE_MB = 256):
+    def execute(self):
+        ROWGROUP_SIZE_MB = 256
         input_files = sorted(glob(self.input_path, recursive=self.input_recursive))
         self.output_path = self.convert_to_hdfs_path(self.output_path)
         
         spark = self.get_spark()
         Schema = self.get_schema()
         
         if input_files:
-            input_files = self._generate_input_files()
-            self.analyze_path = input_files
-            self.output_path = self.convert_to_hdfs_path(self.output_path)
-            output_path = self._generate_output_path()
-            table_name = self._generate_table_name()
-            Schema = self.get_schema()
-            spark = self.get_spark()
+            logging.info(f"Write at path: {self.output_path}")
+            logging.info(f"Save metadata at: {self.table_name}")
             
             with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
                 self.write_to_path(spark_df = self.create_dataframe(spark=spark,
                                       Schema=Schema,
                                       input_files=input_files),
 
                                 output_path = self.output_path,
@@ -1343,106 +1061,14 @@
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
             
 
 class ConvertFromVideo2Image:
-    """
-    Create a parquet/delta file given local Video file
-    
-
-    Parameters
-    ----------
-    input_path : unicode, str 
-        The input filename include ``mp4``
-        Just only 1 video at the time
-        Examples:
-        input_path="**/*.mp4"
-
-    output_path : unicode
-        Ouput directory location maybe file:/ (local file) or hdfs:/ (datalake path)
-        Examples:
-        output_path = "file:/home/username/"
-        output_path = "hdfs:/user/username/"
-        
-    table_name : str
-        Table_name store metadata
-        User should input table_name follow dwh convention: img_abc, vid_abc, audio_abc
-        Examples: img_abc
-        
-    database : str
-        Database to store metadata
-        User should input database follow dwh convention: default
-        Examples: default
-        
-
-    repartition : bool 
-        Default: False
-        Data will be repartition to target file size
-        
-    numPartition : int
-        Default None
-        Number of part each user want to seperate parquet file into
-
-    file_format : str
-        Default: parquet
-        File format user want to write parquet/delta
-        
-    compression: str 
-        Default: zstd
-        Compression method user want to compress parquet file
-        Value: None, zstd, snappy
-        See spark.sql.parquet.compression.codec
-        https://spark.apache.org/docs/2.4.3/sql-data-sources-parquet.html
-        
-    image_type: str
-        Default: jpg
-        Value png or jpg
-        
-    image_color : int
-        Default: 3
-        Value 3, 2 or 1, shape of image have color is 3 or 1 if gray image
-        
-    size : List of Tuple
-        Default: jpg
-        List size user want to resize or padding
-        Examples: size = [(320, 180), (500, 100)]
-        
-    resize_mode : str
-        Default: None
-        Value: None, padding, resize
-        Mode of image user want to resize
-        If in folder user have various size of image, 300, 400 500
-        User will add size = 500:
-        And resize_mode  = 'padding'
-        Then function will convert all image 300, 400, 500 to shape of 500
-    
-    input_recursive : bool
-        Default: True
-        If True: 
-        will loop through folder to get all pattern
-
-    debug : bool
-        If debug=True:
-        Write log into sdk.log file and print more debug information
-
-
-    Examples
-    --------
-    from cads_sdk.nosql.converter import ConvertFromVideo2Image
-    converter = ConvertFromVideo2Image(
-                  input_path='/home/username/image_storage/vid/palawan1.mp4',
-                  input_recursive = False,
-                  output_path = f"file:/home/username/image_storage/vid_image.parquet",
-                 )
-
-    converter.execute()
-    
-    """
     def __init__(
         self,
         input_path,
         output_path,
         table_name = '',
         database = '',
         repartition=True,
@@ -1513,37 +1139,39 @@
                 raise ValueError("You must add table_name and database")
             self.coalesce_dataframe(spark_df, numPartition).write \
                 .format(file_format) \
                 .option('compression', compression) \
                 .mode('overwrite') \
                 .option("path", output_path) \
                 .saveAsTable(database + '.' + table_name)
-        
-        if file_format == 'delta':
-            ss.sql(f"""
-            OPTIMIZE delta.`{output_path}` ZORDER BY(1)
-            """)
-            
-            ss.sql(f"""
-            VACCUUM delta.`{output_path}` RETAINS 0 HOURS
-            """)
+            
+            #     pass
+            # spark_df.coalesce(numPartition) \
+            #         .write \
+            #         .format(file_format) \
+            #         .option('compression', compression) \
+            #         .mode('overwrite') \
+            #         .option("path", output_path) \
+            #         .save()
+               
+
 
             
     def row_generator(self, partitionData):
         """Returns a dict of row input to rdd spark dataframe"""
         for row in partitionData:
             frame_id = row.frame_id
             if self.debug:
                 print(f"Convert video {path}")#, file=self.log_file)
                 
             cap = cv2.VideoCapture(row.path)
             cap.set(cv2.CAP_PROP_POS_FRAMES, frame_id-1)
             res, frame = cap.read()
             # frame = cv2.resize(frame, (self.thumbnail_width, self.thumbnail_height))
-            # frame = frame[:, :, (2, 1, 0)]
+            frame = frame[:, :, (2, 1, 0)]
             
             row_dict = {
                 'frame_id': row.frame_id,
                 'path': row.path,
                 'duration': row.duration,
                 'frame_size': row.frame_size,
                 'total_frame': row.total_frame,
@@ -1572,14 +1200,23 @@
         self.thumbnail_height = frame_size[1]
         
         return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
         
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
     
+#     def get_schema(self):
+#         return Unischema('VideoShema', [
+#             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
+#             UnischemaField('thumbnail', np.uint8, (self.thumbnail_height, self.thumbnail_width, 3), CompressedImageCodec('.jpg'), False),
+#             UnischemaField('duration', np.float_, (), ScalarCodec(FloatType()), False),
+#             UnischemaField('frame_size', np.str_, (), ScalarCodec(StringType()), False),
+#             UnischemaField('video', np.bytes_, (), petastorm.codecs.VideoCodec(), False)
+#         ])
+    
     def get_schema(self):
         return Unischema('VideoImage', [
             UnischemaField('frame_id', np.int, (), ScalarCodec(IntegerType()), False),
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('duration', np.float_, (), ScalarCodec(FloatType()), False),
             UnischemaField('frame_size', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('total_frame', np.str_, (), ScalarCodec(FloatType()), False),
@@ -1611,15 +1248,14 @@
                                 numPartition = self.numPartition,
                                 compression = self.compression)
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
         
-
 class ConvertToFolderVideo:
     """
     Create a folder Video given hdfs_path/local_path or pyspark.sql.dataframe.DataFrame
     
 
     Parameters
     ----------
@@ -1717,14 +1353,21 @@
         if "file:" in input_path:
             return input_path
         else:
             if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
                 return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(self.input_path.replace("hdfs:", ""))
             else:
                 return input_path
+            
+    def check_delta(self, input_path):
+        list_file = ss.ls(input_path)
+        for f in list_file:
+            if '_delta_log' in f:
+                return True
+        return False
         
     def mkdir_folder(self, output_path):
         if not os.path.exists(output_path):
             os.makedirs(output_path)
             
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
@@ -1743,15 +1386,15 @@
             
     def execute(self):
         self.mkdir_folder(os.path.dirname(self.output_path))
         spark = self.get_spark()
         if self.data:
             self.data.foreach(self.write_abtract)
         else:
-            if check_delta(self.input_path):
+            if self.check_delta(self.input_path):
                 logging.info("Detect Delta File")
                 df = ss.sql(f"""select * from delta.`{self.input_path}`""")
             else:
                 df = ss.sql(f"""select * from parquet.`{self.input_path}`""")
             df.foreach(self.write_to_folder)
         logging.info("Convert complete")
         
@@ -1759,144 +1402,72 @@
 #---------------------------------#     
 #------- AUDIO SESSION -----------#
 #---------------------------------#
 
 import_or_install("pydub")
 import pydub
 import_or_install("scipy")
-from scipy.io import wavfile
-import_or_install("pydub")
-import pydub
-import_or_install("scipy")
-from scipy.io import wavfile
-class ConvertFromFolderAudio(ConvertFromFolder):
-    """
-    Create a parquet/delta file given local Image directory
-    
-
-    Parameters
-    ----------
-    input_path : unicode, str 
-        The input filename include ``mp3``, ``waw``, ``pcm``
-        User can add system file pattern like *
-        Examples:
-        input_path="./"
-        input_path="/home/username/path/"
-        
-    input_type : unicode, str
-        str: 'mp3'
-
-    output_path : unicode
-        Ouput directory location maybe file:/ (local file) or hdfs:/ (datalake path)
-        Examples:
-        output_path = "file:/home/username/"
-        output_path = "hdfs:/user/username/"
-        
-    table_name : str
-        Table_name store metadata
-        User should input table_name follow dwh convention: img_abc, vid_abc, audio_abc
-        Examples: img_abc
-        
-    database : str
-        Database to store metadata
-        User should input database follow dwh convention: default
-        Examples: default
-        
-
-    repartition : bool 
-        Default: False
-        Data will be repartition to target file size
-        
-    numPartition : int
-        Default None
-        Number of part each user want to seperate parquet file into
-
-    file_format : str
-        Default: parquet
-        File format user want to write parquet/delta
-        
-    compression: str 
-        Default: zstd
-        Compression method user want to compress parquet file
-        Value: None, zstd, snappy
-        See spark.sql.parquet.compression.codec
-        https://spark.apache.org/docs/2.4.3/sql-data-sources-parquet.html
+from scipy.io import wavfile        
         
     
-    input_recursive : bool
-        Default: True
-        If True: 
-        will loop through folder to get all pattern
-
-    debug : bool
-        If debug=True:
-        Write log into sdk.log file and print more debug information
-
-
-    Examples
-    --------
-    ::
-        ```
-        from cads_sdk.nosql.converter import ConvertFromFolderAudio
-        # Test case 1, write with mp3 audio:
-        converter = ConvertFromFolderAudio(
-                      input_path='./audio_mp3/*.mp3',
-                      input_recursive = False,
-                      output_path = f"file:/home/username/image_storage/audio_mp3.parquet",
-                     )
-        converter.execute()
-
-        # Test case 2, write with PCM audio:
-        converter = ConvertFromFolderAudio(
-                      input_path='./audio_pcm/*.pcm',
-                      input_recursive = False,
-                      output_path = f"file:/home/username/image_storage/audio_pcm.parquet",
-                     )
-
-        converter.execute()
+class ConvertFromFolderAudio:
+    """
+    # Test case 2, write with PCM audio:
+    converter = ConvertFromFolderAudio(
+                  input_path='./audio_pcm/*.pcm',
+                  input_recursive = False,
+                  output_path = f"file:/home/username/image_storage/audio_pcm.parquet",
+                 )
 
-        # Test case 3, write with Wav audio:
-        converter = ConvertFromFolderAudio(
-                      input_path='./audio_wav/*.wav',
-                      input_recursive = False,
-                      output_path = f"file:/home/username/image_storage/audio_wav.parquet",
-                     )
+    converter.execute()
+    
+    # Test case 3, write with Wav audio:
+    converter = ConvertFromFolderAudio(
+                  input_path='./audio_wav/*.wav',
+                  input_recursive = False,
+                  output_path = f"file:/home/username/image_storage/audio_wav.parquet",
+                 )
 
-        converter.execute()
-        ```
+    converter.execute()
     """
     
     def __init__(
         self,
         input_path,
-        input_type,
         output_path,
         table_name = '',
         database = '',
-        repartition=False,
-        numPartition=None,
+        repartition=True,
+        numPartition=1,
         file_format = 'parquet',
         compression = 'zstd',
         input_recursive = False,
-        shorten = False,
+
         
         debug=False
     ):
-        super().__init__(input_path=input_path,
-                        input_type=input_type,
-                        output_path=output_path,
-                        table_name=table_name,
-                        database=database,
-                        repartition=repartition,
-                        numPartition=numPartition,
-                        file_format=file_format,
-                        compression=compression,
-                        input_recursive=input_recursive,
-                        shorten=shorten,
-                        debug=debug)
+        
+        self.input_path = input_path
+        self.output_path = output_path
+        self.table_name = table_name
+        self.database = database
+        self.input_recursive = input_recursive
+        self.repartition = repartition
+        self.numPartition = numPartition
+        self.compression = compression
+        self.file_format = file_format
+        self.debug = debug
+        
+        if debug:
+            self.temp_folder = tempfile.TemporaryDirectory(dir='./tmp_sdk')
+            self.tmp_file = os.path.join(self.temp_folder.name, 'sdk.log')
+            self.log_file = open(self.tmp_file, 'w+')
+            logging.basicConfig(level=logging.DEBUG, filename=self.tmp_file, filemode='w+')
+        else:
+            logging.basicConfig(format='%(asctime)s - %(levelname)s - %(message)s', level=logging.INFO)
             
     def guess_type(self, input_path):
         dict_type = {
             'wav': np.float64,
             'pcm': np.float64,
             'mp3': np.int16,
             'mp4': np.bytes_,
@@ -1916,14 +1487,42 @@
             'mp4': np.bytes_,
             'jpg': np.uint8,
             'png': np.uint8
         }
         
         return dict_type[self.guess_type(input_path)]
     
+    
+    def coalesce_dataframe(self, spark_df, numPartition):
+        if numPartition:
+            return spark_df.coalesce(numPartition)
+        return spark_df
+    
+    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
+        if '.parquet' in output_path.lower():
+            file_format = 'parquet'
+        else:
+            file_format = 'delta'
+            
+        if "file:" in output_path:
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .save()
+        else:
+            if table_name == '' or database == '':
+                raise ValueError("You must add table_name and database")
+            self.coalesce_dataframe(spark_df, numPartition).write \
+                .format(file_format) \
+                .option('compression', compression) \
+                .mode('overwrite') \
+                .option("path", output_path) \
+                .saveAsTable(database + '.' + table_name)
 
             
     def row_generator(self, partitionData):
         """Returns a single entry in the generated dataset. Return a bunch of random values as an example."""
         for row in partitionData:
             path = row.path
             if self.debug:
@@ -1943,15 +1542,15 @@
                 else:
                     channels = 1
 
                 with open(path, 'rb') as file:
                     data = file.read()
 
             if self.guess_type(path) == 'pcm':
-                samplerate, data = read_pcm(path)
+                samplerate, data = self.read_pcm(path)
                 channels = 1
 
             elif self.guess_type(path) == 'mp3':
                 samplerate, data = read_mp3(path)
                 if len(data.shape) == 2:
                     data = data.T
                     channels = 2
@@ -1964,226 +1563,78 @@
             row_dict = {'path': path,
                     'samplerate': samplerate,
                     'channels': channels,
                     'audio': data}
 
             yield dict_to_spark_row(self.unischema, row_dict)
     
+    def convert_to_hdfs_path(self, input_path):
+        if "file:" in input_path:
+            return input_path
+        else:
+            if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
+                return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(self.input_path.replace("hdfs:", ""))
+            else:
+                return input_path
+            
+    def create_dataframe(self, spark, Schema, input_files):
+        
+        
+        spark_df = spark.createDataFrame(pd.DataFrame(input_files, columns=['path']))
+        self.unischema = Schema
+        return spark.createDataFrame(spark_df.rdd.mapPartitions(self.row_generator), Schema.as_spark_schema())
+        
+    def get_spark(self):
+        return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
     
     def get_schema(self):
         return Unischema('Audio', [
             UnischemaField('path', np.str_, (), ScalarCodec(StringType()), False),
             UnischemaField('samplerate', np.int_, (), ScalarCodec(IntegerType()), False),
             UnischemaField('channels', np.int_, (), ScalarCodec(IntegerType()), False),
-            UnischemaField('audio', self.numpy_map_type(self.input_path), (1000,), AudioCodec(self.guess_type(self.input_path)), False)
+            UnischemaField('audio', self.numpy_map_type(self.input_path), (1000,), petastorm.codecs.AudioCodec(self.guess_type(self.input_path)), False)
         ])
     
-    def execute(self, ROWGROUP_SIZE_MB = 256):
-        input_files = self._generate_input_files()
-        self.analyze_path = input_files
-        self.numPartition = self.get_num_partition()
+    def execute(self):
+        ROWGROUP_SIZE_MB = 256
+        input_files = sorted(glob(self.input_path, recursive=self.input_recursive))
         self.output_path = self.convert_to_hdfs_path(self.output_path)
-        output_path = self._generate_output_path()
-        table_name = self._generate_table_name()
-        Schema = self.get_schema()
-        spark = self.get_spark()
-        
-        if input_files:
-            with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
-                self.write_to_path(spark_df = self.create_dataframe(spark=spark,
-                                      Schema=Schema,
-                                      input_files=input_files),
-
-                                output_path = output_path,
-                                table_name = table_name, 
-                                database = self.database,
-                                numPartition = self.numPartition,
-                                compression = self.compression)
-        else:
-            logging.warn("No files were found, check your input_path")
-            
-        logging.info("Convert complete")
-
-
-        
-class MergeFromFolderAudio(ConvertFromFolderAudio):
-    """
-    Create a parquet/delta file given local Image directory
-    
-
-    Parameters
-    ----------
-    input_path : unicode, str 
-        The input directory include ``mp3``, ``pcm``, ``wav`` file
-        User can add system file pattern like *
-        Examples:
-        input_path="/path/to/MOT17.zip"
-        This pattern get all jpg in folder with different directory levels
-        View https://docs.python.org/3/library/glob.html
-
-    output_path : unicode
-        Ouput directory location maybe file:/ (local file) or hdfs:/ (datalake path)
-        Examples:
-        output_path = "file:/home/username/"
-        output_path = "hdfs:/user/username/"
-        
-    table_name : str
-        Table_name store metadata
-        User should input table_name follow dwh convention: img_abc, vid_abc, audio_abc
-        Examples: img_abc
-        
-    database : str
-        Database to store metadata
-        User should input database follow dwh convention: default
-        Examples: default
-        
-
-    repartition : bool 
-        Default: False
-        Data will be repartition to target file size
-        
-    numPartition : int
-        Default None
-        Number of part each user want to seperate parquet file into
-
-    file_format : str
-        Default: parquet
-        File format user want to write parquet/delta
         
-    compression: str 
-        Default: zstd
-        Compression method user want to compress parquet file
-        Value: None, zstd, snappy
-        See spark.sql.parquet.compression.codec
-        https://spark.apache.org/docs/2.4.3/sql-data-sources-parquet.html
-        
-
-    debug : bool
-        If debug=True:
-        Write log into sdk.log file and print more debug information
-
-
-    Examples
-    --------
-    ::
-        ```
-        from cads_sdk.nosql.converter import MergeFromFolderAudio
-
-        converter = ConvertFromFolderAudio(
-                      input_path='./audio_wav/*.wav',
-                      input_recursive = False,
-                      output_path = f"file:/home/username/image_storage/audio_wav.delta",
-                     )
-
-        converter.execute()
-        ```
-        
-        Function will convert all Audio in file:'./audio_wav/*.wav' to absolute directory "file:/home/username/image_storage/audio_wav.delta"
-    """
-   
-        
-    def __init__(
-        self,
-        input_path,
-        input_type,
-        output_path,
-        table_name = '',
-        database = '',
-        repartition=False,
-        numPartition=None,
-        file_format = 'delta',
-        compression = 'zstd',
-        
-        shorten=False,
-        merge_keys = ['path'],
-        input_recursive = False,
-        
-        debug=False
-    ):
-        
-        super().__init__(input_path=input_path,
-                         input_type=input_type,
-                        output_path=output_path,
-                        table_name=table_name,
-                        database=database,
-                        repartition=repartition,
-                        numPartition=numPartition,
-                        file_format=file_format,
-                        compression=compression,
-                        input_recursive=input_recursive,
-                        shorten=shorten,
-                        debug=debug)
-        self.merge_keys = merge_keys
-
-    
-    def check_output(self, output_path):
-        if not ss.exists(output_path):
-            raise ValueError(f"Path {output_path} is not exists, you can only merge with exists path")
-            
-        if not check_delta(output_path):
-            raise ValueError(f"Path {output_path} is not a delta table, you can only merge with delta table")
-                    
-    def write_to_path(self, spark_df, output_path, table_name = '', database='', numPartition=8, compression='zstd'):
-        if '.parquet' in output_path.lower():
-            file_format = 'delta'
-        else:
-            file_format = 'delta'
-        
-        spark_df.createOrReplaceTempView('new')
-        # Merge new dataframe image into old dataframe
-        
-        sql_compare = ''
-        for k in self.merge_keys:
-            sql_compare+= f"""NVL(o.{k},'') = NVL(n.{k},'')"""
-            
-        ss.sql(f"""
-          MERGE INTO delta.`{output_path}` o
-          USING new n ON
-          {sql_compare}
-            
-          WHEN NOT MATCHED
-          THEN INSERT *
-        """)
-        
-        if file_format == 'delta':
-            ss.sql(f"""
-            OPTIMIZE delta.`{output_path}` ZORDER BY(path)
-            """)
-            
-            ss.sql(f"""
-            VACUUM delta.`{output_path}` RETAIN 0 HOURS
-            """)
-    
-    def execute(self, ROWGROUP_SIZE_MB = 256):
-        input_files = self._generate_input_files()
-        self.analyze_path = input_files
-        self.numPartition = self.get_num_partition()
-        self.output_path = self.convert_to_hdfs_path(self.output_path)
-        output_path = self._generate_output_path()
-        table_name = self._generate_table_name()
-        Schema = self.get_schema()
         spark = self.get_spark()
+        Schema = self.get_schema()
         
         if input_files:
-            with materialize_dataset(spark, output_path, Schema, ROWGROUP_SIZE_MB):
+            logging.info(f"Write at path: {self.output_path}")
+            logging.info(f"Save metadata at: {self.table_name}")
+            
+            with materialize_dataset(spark, self.output_path, Schema, ROWGROUP_SIZE_MB):
                 self.write_to_path(spark_df = self.create_dataframe(spark=spark,
                                       Schema=Schema,
                                       input_files=input_files),
 
-                                output_path = output_path,
-                                table_name = table_name, 
+                                output_path = self.output_path,
+                                table_name = self.table_name, 
                                 database = self.database,
                                 numPartition = self.numPartition,
                                 compression = self.compression)
         else:
             logging.warn("No files were found, check your input_path")
             
         logging.info("Convert complete")
+                
+#             self.create_dataframe(spark=spark,
+#                                   Schema=Schema,
+#                                   input_files=input_files,
+#                                   output_path=self.output_path,
+#                                   table_name = self.table_name, 
+#                                   database=self.database,
+#                                   numPartition=self.numPartition,
+#                                   compression=self.compression)
+            
             
-
             
 class ConvertToFolderAudio:
     """
     Create a folder Audio given hdfs_path/local_path or pyspark.sql.dataframe.DataFrame
     
 
     Parameters
@@ -2283,14 +1734,21 @@
         if "file:" in input_path:
             return input_path
         else:
             if "hdfs://hdfs-cluster.datalake.bigdata.local:8020" not in os.path.dirname(input_path):
                 return "hdfs://hdfs-cluster.datalake.bigdata.local:8020" + os.path.abspath(self.input_path.replace("hdfs:", ""))
             else:
                 return input_path
+            
+    def check_delta(self, input_path):
+        list_file = ss.ls(input_path)
+        for f in list_file:
+            if '_delta_log' in f:
+                return True
+        return False
         
     def mkdir_folder(self, output_path):
         if not os.path.exists(output_path):
             os.makedirs(output_path)
             
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='8', executor_memory='4G', port='', yarn=False).spark
@@ -2309,14 +1767,14 @@
             
     def execute(self):
         self.mkdir_folder(os.path.dirname(self.output_path))
         spark = self.get_spark()
         if self.data:
             self.data.foreach(self.write_abtract)
         else:
-            if check_delta(self.input_path):
+            if self.check_delta(self.input_path):
                 logging.info("Detect Delta File")
                 df = ss.sql(f"""select * from delta.`{self.input_path}`""")
             else:
                 df = ss.sql(f"""select * from parquet.`{self.input_path}`""")
             df.foreach(self.write_to_folder)
         logging.info("Convert complete")
```

## cads_sdk/nosql/display.py

```diff
@@ -1,8 +1,7 @@
-import spark_sdk as ss
 import os
 try:
     from PIL import Image
 except:
     os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 Pillow")
     from PIL import Image
     pass
@@ -16,31 +15,14 @@
     OPENCV_AVAILABLE = False
 
 from cads_sdk.nosql.etl import read_mp3,read_pcm
 
 import base64
 import io
 
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Sequence,
-    Tuple,
-    Type,
-    Union,
-    cast,
-    overload,
-    TYPE_CHECKING,
-)
-from pyspark.sql.column import Column
-
 import pandas as pd
 pd.options.display.width = 200
 
 
 def cvtColor(binary):
     b,g,r = Image.open(io.BytesIO(binary)).split()
     return Image.merge("RGB", (r, g, b))
@@ -54,140 +36,26 @@
     return i
 
 def image_base64(im):
     # if isinstance(im, str):
     #     im = get_thumbnail(im)
     im = get_thumbnail(im)    
     with io.BytesIO() as buffer:
-        if im.mode != 'RGB':
-            im = im.convert('RGB')
         im.save(buffer, 'jpeg')
         return base64.b64encode(buffer.getvalue()).decode()
 
 def image_formatter(im):
     return f'<img src="data:image/jpeg;base64,{image_base64(im)}">'
     # return f'<img src="data:image/jpeg;base64,{image_base64(im)}">'
 
     
-    
-def _create_idx_dataframe(self, orderBy='path'):
-    from pyspark.sql.functions import spark_partition_id, monotonically_increasing_id, count, lit, first, sum, col, udf
-    from pyspark.sql.window import Window
-
-    offset = 1
-    df_with_partition_id = self.withColumn("partition_id", spark_partition_id()).withColumn("inc_id", monotonically_increasing_id())
-
-    partition_offsets = df_with_partition_id \
-        .orderBy("partition_id") \
-        .groupBy("partition_id") \
-        .agg(count(lit(1)).alias("cnt"), first("inc_id").alias("inc_id")) \
-        .withColumn("cnt", sum("cnt").over(Window.orderBy("partition_id")) - col("cnt") - col("inc_id") + lit(offset).alias("cnt")) \
-        .select(["partition_id", "cnt"]) \
-        .collect()
-
-    get_offset = {}
-    for row in partition_offsets:
-        get_offset[row[0]] = row[1]
-
-
-    spark_df = df_with_partition_id \
-        .withColumn("partition_offset", udf(lambda partition_id: get_offset[partition_id], "long")(col("partition_id"))) \
-        .withColumn("idx", col("partition_offset") + col("inc_id")) \
-        .drop("partition_id", "partition_offset", "inc_id")
-    return spark_df
-
-def _filter_idx(self):
-    self.createOrReplaceTempView('spark_df')
-
-    spark_df = ss.sql(f"""
-    select 
-        *
-    from spark_df
-    where idx between {self.from_idx} and {self.to_idx}
-    """)
-    return spark_df.drop('idx')
-
-def convert_to_index_sliceable(self):
-    if isinstance(self.from_idx, int):
-        self.from_idx = self.from_idx
-        if isinstance(self.to_idx, int):
-            self.to_idx = self.to_idx
-        else:
-            self.to_idx = self.from_idx + self.limit_idx
-    else:
-        self.from_idx = 0
-        if isinstance(self.to_idx, int):
-            self.to_idx = self.to_idx
-        else:
-            self.to_idx = self.limit_idx
-    from pyspark.sql import DataFrame as SparkDataFrame
-    SparkDataFrame.from_idx = self.from_idx
-    SparkDataFrame.to_idx = self.to_idx
-
-
-def __getitem__(self, item: Union[int, str, Column, List, Tuple]) -> Union[Column, "DataFrame"]:
-        """Returns the column as a :class:`Column`.
-
-        .. versionadded:: 1.3.0
-
-        Examples
-        --------
-        >>> df.select(df['age']).collect()
-        [Row(age=2), Row(age=5)]
-        >>> df[ ["name", "age"]].collect()
-        [Row(name='Alice', age=2), Row(name='Bob', age=5)]
-        >>> df[ df.age > 3 ].collect()
-        [Row(age=5, name='Bob')]
-        >>> df[df[0] > 3].collect()
-        [Row(age=5, name='Bob')]
-        """
-        if isinstance(item, str):
-            jc = self._jdf.apply(item)
-            return Column(jc)
-        elif isinstance(item, Column):
-            return self.filter(item)
-        elif isinstance(item, (list, tuple)):
-            return self.select(*item)
-        elif isinstance(item, int):
-            jc = self._jdf.apply(self.columns[item])
-            return Column(jc)
-        elif isinstance(item, slice):
-            self.from_idx = item.start
-            self.to_idx = item.stop
-            self.limit_idx = 100
-
-            self.convert_to_index_sliceable()
-            self = self._create_idx_dataframe()
-            spark_df = self._filter_idx()
-            return spark_df
-            
-        else:
-            raise TypeError("unexpected item type: %s" % type(item))
-    
-    
 def toPandasImage(self, limit:int = 100, mode='RGB'):
-    """
-    Function to display image in parquet as a DataFrame
-    Parameters
-    ----------
-    limit : int
-        Default: 100
-        Limit number of display image at the same time
-        Maxium is 100
-    mode : str
-        Color mode 
-        Default: 'RGB'
-        RGB or BGR
-        
-    """
     if limit > 100:
         limit = 100
-    self = self.limit(limit)
-    pdf = pd.DataFrame.from_records(self.collect(), columns=self.columns)
-    # pdf = self.limit(limit).toPandas()
+    pdf = self.limit(limit).toPandas()
     
     need_convert_dict = {}
     for c in self.schema:
         if "BinaryType" in str(c.dataType):
             c_name = c.name
             # pdf[c_name] = pdf[c_name].apply(lambda x: Image.open(io.BytesIO(x)))
             if mode=='BGR':
@@ -197,20 +65,14 @@
             need_convert_dict[c_name] = image_formatter
     DataFrame.need_convert_dict = need_convert_dict
     pdf.need_convert_dict = need_convert_dict
     return pdf
 
 
 from pyspark.sql import DataFrame as SparkDataFrame
-SparkDataFrame.__getitem__ = __getitem__
-SparkDataFrame.convert_to_index_sliceable = convert_to_index_sliceable
-SparkDataFrame._create_idx_dataframe = _create_idx_dataframe
-SparkDataFrame._filter_idx = _filter_idx
-
-
 SparkDataFrame.toPandasImage = toPandasImage
 
 from pandas._config import get_option
 from io import StringIO
 from pandas.io.formats import format as fmt
 from typing import Optional
 
@@ -268,27 +130,29 @@
 from pandas import DataFrame
 DataFrame._repr_html_ = _repr_html_
 
 import os
 import tempfile
 
 
-from spark_sdk.utils import import_or_install
+from cads_sdk.utils import import_or_install
 import_or_install("ipywidgets")
 try:
     os.system("jupyter nbextension enable --py --sys-prefix widgetsnbextension")
 except:
     os.system("pip install --proxy http://proxy.hcm.fpt.vn:80 ipywidgets")
     os.system("jupyter nbextension enable --py --sys-prefix widgetsnbextension")
     
 from ipywidgets.widgets import Box
 from ipywidgets import widgets
 from traitlets import traitlets
 
-from spark_sdk import PySpark
+from cads_sdk import PySpark
+import cads_sdk as ss
+
 import numpy as np
 from io import BytesIO
 
 class LoadedButton(widgets.Button):
     """A button that can holds a value as a attribute."""
 
     def __init__(self, value=None, *args, **kwargs):
@@ -312,31 +176,28 @@
         
         self.input_path = input_path
         self.width = width
         self.height = height
         self.html_attributes = html_attributes
         self.thumbnail_width = thumbnail_width
         self.thumbnail_height = thumbnail_height
-        self.from_idx = from_idx
-        self.to_idx = to_idx
         self.limit = limit
         
-    def convert_to_index_sliceable(self):
-        if isinstance(self.from_idx, int):
-            self.from_idx = self.from_idx
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
+        if isinstance(from_idx, int):
+            self.from_idx = from_idx
+            if isinstance(to_idx, int):
+                self.to_idx = to_idx
             else:
-                self.to_idx = self.from_idx + self.limit
+                self.to_idx = from_idx + limit
         else:
             self.from_idx = 0
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
+            if isinstance(to_idx, int):
+                self.to_idx = to_idx
             else:
-                self.to_idx = self.limit
+                self.to_idx = limit
         
         
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
     
     def check_delta(self, input_path):
         list_file = ss.ls(input_path)
@@ -371,56 +232,77 @@
         self.tmp_file = os.path.join(self.temp_folder.name, self.base_path)
 
         _ = [self.write_to_folder(row) for row in df.collect()]
 
         from IPython.display import Video
         self.output.append_display_data(Video(self.tmp_file, width=self.width, height=self.height))
 
-    def __getitem__(self, key):
-        _valid_types = (
-            "integer, integer slice (START point is INCLUDED, END "
-            "point is EXCLUDED), listlike of integers, boolean array"
-        )
-        
-        from pandas.core.indexers import (check_array_indexer, is_list_like_indexer)
-        
-        if not isinstance(key, slice):
-            raise ValueError("Invalid call for scalar access (getting)!")
-        # if not is_list_like_indexer(key):
-        #     raise ValueError(f"Can only index by location with a {key}]")
-            
-        
-        self.from_idx = key.start
-        self.to_idx = key.stop
-        return self._repr_html_()
-        
+#     def __getitem__(self, key):
+#         _valid_types = (
+#             "integer, integer slice (START point is INCLUDED, END "
+#             "point is EXCLUDED), listlike of integers, boolean array"
+#         )
+        
+#         from pandas.core.indexers import (check_array_indexer, is_list_like_indexer)
+        
+#         if not isinstance(key, tuple):
+#             raise ValueError("Invalid call for scalar access (getting)!")
+#         if not is_list_like_indexer(key):
+#             raise ValueError(f"Can only index by location with a {key}]")
+        
+#         spark_df = spark_df._create_idx_dataframe()
+#         spark_df = spark_df._filter_idx()
+#         self._repr_html_
+        
+
+    def _create_idx_dataframe(self, spark_df, orderBy='path'):
+        spark_df.createOrReplaceTempView('spark_df')
+        
+        spark_df = ss.sql(f"""
+        select 
+            *,
+            row_number() OVER(ORDER BY {orderBy}) idx
+        from spark_df
+        """)
+        return spark_df
+    
+    def _filter_idx(self, spark_df):
+        spark_df.createOrReplaceTempView('spark_df')
+        columns = spark_df.schema.names
+        columns.pop(-1)
+        
+        spark_df = ss.sql(f"""
+        select 
+            *
+        from spark_df
+        where idx between {self.from_idx} and {self.to_idx}
+        """)
+        return spark_df
         
     def _repr_html_(self):
         width = height = ''
         if self.width:
             width = ' width="%d"' % self.width
         if self.height:
             height = ' height="%d"' % self.height
             
         if isinstance(self.input_path, str):
             df_path = self.generate_sql("path, thumbnail")
-        
-            if self.from_idx:
-                self.convert_to_index_sliceable()
-                df_path = df_path[self.from_idx:self.to_idx]
+            df_path = self._create_idx_dataframe(df_path)
+            df_path = self._filter_idx(df_path).limit(self.limit)
         else:
             raise ValueError("Check your input_path, it not string or can not be found")
         
         selection_box = widgets.VBox()
         selection_toggles = []
         selected_labels = {}
         labels = {}
         
         
-        layout = widgets.Layout(width=str(pd.options.display.width*5)+'px', height=f"{self.thumbnail_height}px")
+        layout = widgets.Layout(width=str(pd.options.display.max_colwidth*5)+'px', height=f"{self.thumbnail_height}px")
         
         for row in sorted(df_path.orderBy("path").collect()):
             o = LoadedButton(description=row.path, value=row.path, layout=layout)
             o.on_click(self.displayVideo)
             
             
             thumbnail = widgets.Image(
@@ -446,66 +328,42 @@
 
 class Audio(object):
     """
     Audio 
     Function to display all audio files in parquet file as a list of buttons
     When click on button with lable, audio user just clicked will pop up and display
     
-    :param 
-    input_path: path to parquet/delta file
+    :param input_path: path to parquet/delta file
 
     Return:
     HTML list of buttons base on path name can be clicked to display Video
     
     # Test case 1: Open parquet pcm file
     from cads_sdk.nosql.reader import Video
     Audio('file:/home/duyvnc/image_storage/audio_pcm.parquet')
     
     # Test case 2: Open parquet mp3 file
     Audio('file:/home/duyvnc/image_storage/audio_mp3.parquet')
     
     # Test case 3: Open parquet wav file
     Audio('file:/home/duyvnc/image_storage/audio_wav.parquet')
     """
-    def __init__(self, 
-                 input_path=None, 
-                 width=None, 
-                 height=None, 
-                 html_attributes="controls",
-                 thumbnail_width = 256,
-                 thumbnail_height = 144,
-                 from_idx = None,
-                 to_idx = None,
-                 limit = 100
-                ):
+    
+    def __init__(self, input_path=None, video=None, data=None, url=None, filename=None, embed=False,
+                 mimetype="wav", width=None, height=None, html_attributes="controls", limit=100):
         
         self.input_path = input_path
+        self.video = video
+        self.mimetype = mimetype
+        self.embed = embed
         self.width = width
         self.height = height
         self.html_attributes = html_attributes
-        self.thumbnail_width = thumbnail_width
-        self.thumbnail_height = thumbnail_height
-        self.from_idx = from_idx
-        self.to_idx = to_idx
         self.limit = limit
         
-    def convert_to_index_sliceable(self):
-        if isinstance(self.from_idx, int):
-            self.from_idx = self.from_idx
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.from_idx + self.limit
-        else:
-            self.from_idx = 0
-            if isinstance(self.to_idx, int):
-                self.to_idx = self.to_idx
-            else:
-                self.to_idx = self.limit
-        
     def get_spark(self):
         return ss.PySpark(driver_memory='32G', num_executors='4', executor_memory='4G', port='', yarn=False).spark
     
     def check_delta(self, input_path):
         list_file = ss.ls(input_path)
         for f in list_file:
             if '_delta_log' in f:
@@ -543,62 +401,41 @@
         get_value = ex.description
         df = self.generate_sql("*").filter(f"path = '{get_value}'").limit(1)
         
         _ = [self.write_to_folder(row) for row in df.collect()]
         
         # df.foreach(self.write_to_folder)
         
-        
     def _repr_html_(self):
         width = height = ''
         if self.width:
             width = ' width="%d"' % self.width
         if self.height:
             height = ' height="%d"' % self.height
             
         if isinstance(self.input_path, str):
-            df_path = self.generate_sql("path")
+            df_path = self.generate_sql("path").limit(self.limit)
+        
         
-            if self.from_idx:
-                self.convert_to_index_sliceable()
-                df_path = df_path[self.from_idx:self.to_idx]
         
         selection_box = widgets.VBox()
         selection_toggles = []
         selected_labels = {}
         
-        layout = widgets.Layout(width=str(pd.options.display.width*5)+'px', height='40px')
+        layout = widgets.Layout(width=str(pd.options.display.max_colwidth*5)+'px', height='40px')
         
         for row in df_path.orderBy('path').collect():
             o = LoadedButton(description=row.path, value=row.path,layout=layout)
             o.on_click(self.displayAudio)
             selection_toggles.append(o)
 
         selection_box.children = selection_toggles
         self.output = widgets.Output()
         return display(selection_box, self.output)
     
-    def __getitem__(self, key):
-        _valid_types = (
-            "integer, integer slice (START point is INCLUDED, END "
-            "point is EXCLUDED), listlike of integers, boolean array"
-        )
-        
-        from pandas.core.indexers import (check_array_indexer, is_list_like_indexer)
-        
-        if not isinstance(key, slice):
-            raise ValueError("Invalid call for scalar access (getting)!")
-        # if not is_list_like_indexer(key):
-        #     raise ValueError(f"Can only index by location with a {key}]")
-            
-        
-        self.from_idx = key.start
-        self.to_idx = key.stop
-        return self._repr_html_()
-    
     def __repr__(self):
         return ""
     
     
 def __repr__(self):
     return """If not display widget try copy this to your terminal
     pip install --proxy http://proxy.hcm.fpt.vn:80 ipywidgets
```

## cads_sdk/nosql/etl.py

```diff
@@ -1,24 +1,24 @@
 import pydub
 import numpy as np
 import cv2
-import os
 
 def read_mp3(f, normalized=False):
     """MP3 to numpy array"""
     
     a = pydub.AudioSegment.from_mp3(f)
     y = np.array(a.get_array_of_samples())
     if a.channels == 2:
         y = y.reshape((-1, 2))
     if normalized:
         return a.frame_rate, np.float32(y) / 2**15
     else:
         return a.frame_rate, y
-
+    
+    
         
 def read_pcm(input_path, dtype='float64'):
     with open(input_path, 'rb') as file:
         y = file.read()
         y = np.frombuffer(y, dtype = 'int16')
         i = np.iinfo(y.dtype)
         abs_max = 2 ** (i.bits - 1)
@@ -29,9 +29,8 @@
 def padding(img, expected_size, borderType=cv2.BORDER_CONSTANT, value=(255,255,255)):
     delta_width = expected_size[0] - img.shape[0]
     delta_height = expected_size[1] - img.shape[1]
     pad_width = delta_width // 2
     pad_height = delta_height // 2
     # padding = (pad_width, pad_height, delta_width - pad_width, delta_height - pad_height)
 
-    return cv2.copyMakeBorder(img, pad_width, delta_width - pad_width, pad_height, delta_height - pad_height, borderType, value=value)
-
+    return cv2.copyMakeBorder(img, pad_width, delta_width - pad_width, pad_height, delta_height - pad_height, borderType, value=value)
```

## Comparing `cads_sdk-0.0.15.dist-info/METADATA` & `cads_sdk-0.0.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: cads-sdk
-Version: 0.0.15
+Version: 0.0.5
 Summary: Function to help Data Scientist work more effectively with DWH
 Home-page: http://git.bigdata.local/data-engineers/sdk/utilities
 Author: duyvnc
 Author-email: duyvnc@fpt.com.vn
 License: duyvnc
 Platform: UNKNOWN
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
-Requires-Dist: spark-sdk (>=0.4.20)
+Requires-Dist: spark-sdk (>=0.4.19)
 Requires-Dist: opencv-python
 Requires-Dist: Pillow
 Requires-Dist: scipy
 Requires-Dist: pydub
 Requires-Dist: ipywidgets
 Requires-Dist: petastorm
 
 -----------------
 
 # cads-sdk: Functions to help Data Scientist work more effectively with unstructured data and datalake
-[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.0.15-blue)](https://pypi.org/project/cads-sdk/)
+[![PyPI Latest Release](https://img.shields.io/badge/pypi-0.4.20-blue)](https://pypi.org/project/cads-sdk/)
 [![Package Status](https://img.shields.io/badge/status-stable-green)](https://pypi.org/project/cads-sdk/)
-[![Downloads](https://static.pepy.tech/personalized-badge/cads-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cads-sdk)
+[![Downloads](https://static.pepy.tech/personalized-badge/spark-sdk?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/cads-sdk)
 [![Powered by NumFOCUS](https://img.shields.io/badge/powered%20by-CADS-orange.svg?style=flat&colorA=E1523D&colorB=007D8A)](https://blog.cads.live/)
 
 
 
 ## What is it?
 
 **cads-sdk** Function to help Data Scientist work more effectively with unstructured data. Include different function work with image, audio
@@ -81,15 +81,14 @@
 # Image
 ### Convert a folder image to parquet
 ```python
 from cads_sdk.nosql.converter import ConvertFromFolderImage
 
 converter = ConvertFromFolderImage(
               input_path="/path/to/folder/**/*.jpg",
-              input_type = 'jpg' # 'jpg' | ('jpg', 'png')
               input_recursive = True,
 
               #setting output
               output_path = f"file:/output/path/image_storage",
 
               # setting converter
               image_type = 'jpg',
@@ -103,16 +102,14 @@
 
 # convert directly from .zip file to parquet
 from cads_sdk.nosql.converter import ConvertFromZipImage
 
 converter = ConvertFromZipImage(
               input_path="/path/to/image_storage/ETHZ.zip",
               input_recursive = True, # will loop through folder to get all pattern
-              input_type = 'jpg' # 'jpg' | ('jpg', 'png')
-
               #setting output
               output_path = f"file:/output/path/img_ethz.parquet",
               table_name = 'img_ethz',
               database = 'default',
               file_format = 'parquet', # delta|parquet
               compression = 'zstd', # zstd|snappy
               # setting converter
@@ -168,15 +165,14 @@
 ### Suport pcm, mp3, wav format
 ### Convert a folder audio to parquet
 ```python
 from cads_sdk.nosql.converter import ConvertFromFolderImage
 
 converter = ConvertFromFolderAudio(
               input_path='/path/to/audio_wav/*.wav', #(1)
-              input_type = 'wav' # 'wav'| 'mp3' | 'pcm' ('wav', 'mp3')
               input_recursive = False,
               output_path = f"file:/output/path/audio_wav.parquet",
              )
 
 converter.execute()
 ```
 ### Convert a parquet to folder audio
@@ -196,16 +192,18 @@
 from cads_sdk.nosql.display import Audio
 Audio('file:/path/to/audio_mp3.parquet')
 ```
 # Video
 ```python
 from cads_sdk.nosql.converter import ConvertFromVideo2Image
 converter = ConvertFromVideo2Image(
-              input_path='/home/username/vid/palawan1.mp4',
-              output_path = f"file:/home/username/vid_image.parquet",
+              input_path='/home/username/image_storage/vid/palawan1.mp4',
+              input_recursive = False,
+              output_path = f"file:/home/username/image_storage/vid_image.parquet",
+
              )
 
 converter.execute()
 ```
 ### For more information use class instance
 ```python
 ConvertFromFolderImage.__doc__
```

