# Comparing `tmp/stockpick-1.3.1-py3-none-any.whl.zip` & `tmp/stockpick-1.3.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 90855 bytes, number of entries: 17
+Zip file size: 90869 bytes, number of entries: 17
 -rw-r--r--  2.0 unx     8196 b- defN 22-Jul-05 07:12 stockpick/.DS_Store
 -rw-r--r--  2.0 unx      130 b- defN 23-Apr-25 08:50 stockpick/__init__.py
 -rw-r--r--  2.0 unx     3901 b- defN 23-Mar-29 08:18 stockpick/corpus_process.py
 -rw-r--r--  2.0 unx     1091 b- defN 22-Jun-29 08:41 stockpick/enum_table
--rw-r--r--  2.0 unx    13350 b- defN 23-Apr-26 09:00 stockpick/extractor.py
+-rw-r--r--  2.0 unx    13371 b- defN 23-Apr-28 06:26 stockpick/extractor.py
 -rw-r--r--  2.0 unx    14078 b- defN 23-Apr-26 06:47 stockpick/extractor_new.py
 -rw-------  2.0 unx   222580 b- defN 22-Jun-28 11:54 stockpick/gupiao_dict.txt
 -rw-r--r--  2.0 unx     3155 b- defN 23-Mar-21 09:17 stockpick/index_table
 -rw-------  2.0 unx      697 b- defN 22-Jun-28 12:13 stockpick/question.txt
 -rw-r--r--  2.0 unx     1533 b- defN 23-Feb-23 07:48 stockpick/scope_table
 -rw-r--r--  2.0 unx     1589 b- defN 23-Apr-07 06:03 stockpick/sentences.txt
 -rw-r--r--  2.0 unx      131 b- defN 22-Jul-04 09:17 stockpick/unit_table
 -rw-r--r--  2.0 unx      717 b- defN 23-Apr-06 02:29 stockpick/utils.py
--rw-r--r--  2.0 unx      220 b- defN 23-Apr-26 11:00 stockpick-1.3.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-26 11:00 stockpick-1.3.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-26 11:00 stockpick-1.3.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1331 b- defN 23-Apr-26 11:00 stockpick-1.3.1.dist-info/RECORD
-17 files, 272801 bytes uncompressed, 88699 bytes compressed:  67.5%
+-rw-r--r--  2.0 unx      220 b- defN 23-Apr-28 06:27 stockpick-1.3.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-28 06:27 stockpick-1.3.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-28 06:27 stockpick-1.3.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1331 b- defN 23-Apr-28 06:27 stockpick-1.3.2.dist-info/RECORD
+17 files, 272822 bytes uncompressed, 88713 bytes compressed:  67.5%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: stockpick/unit_table
 Comment: 
 
 Filename: stockpick/utils.py
 Comment: 
 
-Filename: stockpick-1.3.1.dist-info/METADATA
+Filename: stockpick-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: stockpick-1.3.1.dist-info/WHEEL
+Filename: stockpick-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: stockpick-1.3.1.dist-info/top_level.txt
+Filename: stockpick-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: stockpick-1.3.1.dist-info/RECORD
+Filename: stockpick-1.3.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stockpick/extractor.py

```diff
@@ -293,23 +293,22 @@
 
 
 
 
 
 
 
-ex = Extractor()
-sentences = corpus_process.get_sentence()
-#sentences = ["市值-100.7~300.6亿以内?市盈大于2小于3市净率在1-3之间"]
-#sentences = ["净利润增长率在5-10%之间"]
-for sentence in sentences:
-    print(sentence)
-    res = ex.process_sentence(sentence)
-    print(res)
-    print("\n\n\n")
+# ex = Extractor()
+# sentences = corpus_process.get_sentence()
+# sentences = ["市值-100.7~300.6亿以内?市盈大于2小于3市净率在1-3之间，并且换手率小于5%"]
+# #sentences = ["净利润增长率在5-10%之间"]
+# for sentence in sentences:
+#     print(sentence)
+#     res = ex.process_sentence(sentence)
+#     print(res)
```

## Comparing `stockpick-1.3.1.dist-info/RECORD` & `stockpick-1.3.2.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 stockpick/.DS_Store,sha256=LXybLAy3n_mJ5ENzjsUY6K2CavMWBO69QQVaixrzQkI,8196
 stockpick/__init__.py,sha256=hDuOrJBpQxnUvi1-4kfWtgfXGBerWP3Yj-BtOyXQ5bs,130
 stockpick/corpus_process.py,sha256=16hCEVlxToKpjCHrM2y8lm3ZV1uDEv0WDqzL-_ONIdY,3901
 stockpick/enum_table,sha256=j_8irWQ4Pnuf79oOrM9BtkBqcZ0qW671Lb31JmmpbjU,1091
-stockpick/extractor.py,sha256=SBZRfZS4u4uJoqgVyutc5zztFCgrcYlJikHMCyOX8DQ,13350
+stockpick/extractor.py,sha256=VMFi-RuANhXhvNZRFpNgw61wAw_Ztowm2qeLzW2WYyI,13371
 stockpick/extractor_new.py,sha256=ccy-JkNx38Ss2MAfLvTkTePuBL-M1l-IdiG2QBOLI40,14078
 stockpick/gupiao_dict.txt,sha256=StFtBkrP2xx4hG2pmvBhd2ZTCht-eesLCtJf4a2e_20,222580
 stockpick/index_table,sha256=RX-blsmWXvbo1CAW65mt0mtHgiaNuAK6G4LLr30-OQo,3155
 stockpick/question.txt,sha256=sRfFNP_rNTPxd7Lv09f74rSTkkKuAuzNJcm6ZImd7N4,697
 stockpick/scope_table,sha256=rwEK8lHWdA27fAwpwfVEbdl7ErBLVjspGWGzNx_ZMoQ,1533
 stockpick/sentences.txt,sha256=FnIorIW7Z_CerDtwLanm9BlBOerG0RZHbPLPktAbBRM,1589
 stockpick/unit_table,sha256=1DzgbTs-S87tTPND5YM7N6f9YI4nXz-XT-RBJ0OidgY,131
 stockpick/utils.py,sha256=LjvxYsBNxSX-wu6-uiUmOwmEMVVbPrOdbNj3KZ9vkic,717
-stockpick-1.3.1.dist-info/METADATA,sha256=CnuuPwRiYUGowmD8vIrOYisOs_ZjdmJTDq2vnHI1gN0,220
-stockpick-1.3.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-stockpick-1.3.1.dist-info/top_level.txt,sha256=BufNdGunPZT_TJ3_9gD7VLobclDjXXDghnY5N0eANQg,10
-stockpick-1.3.1.dist-info/RECORD,,
+stockpick-1.3.2.dist-info/METADATA,sha256=4e_VVaayNmAvmERfSWd4NH2kycjCcR7VglP3aaJrhNs,220
+stockpick-1.3.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+stockpick-1.3.2.dist-info/top_level.txt,sha256=BufNdGunPZT_TJ3_9gD7VLobclDjXXDghnY5N0eANQg,10
+stockpick-1.3.2.dist-info/RECORD,,
```

