# Comparing `tmp/georgio-2023.118.1193-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip` & `tmp/georgio-2023.118.1197-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1059452 bytes, number of entries: 7
--rw-r--r--  4.6 unx     3047 b- defN 23-Apr-28 19:55 georgio-2023.118.1193.dist-info/METADATA
--rw-r--r--  4.6 unx      129 b- defN 23-Apr-28 19:55 georgio-2023.118.1193.dist-info/WHEEL
--rw-r--r--  4.6 unx    11350 b- defN 23-Apr-28 19:55 georgio-2023.118.1193.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx       47 b- defN 23-Apr-28 19:55 georgio-2023.118.1193.dist-info/license_files/NOTICE
--rw-r--r--  4.6 unx      111 b- defN 23-Apr-28 19:55 georgio/__init__.py
--rwxr-xr-x  4.6 unx  4415240 b- defN 23-Apr-28 19:55 georgio/georgio.cpython-39-x86_64-linux-gnu.so
--rw-r--r--  4.6 unx      630 b- defN 23-Apr-28 19:55 georgio-2023.118.1193.dist-info/RECORD
-7 files, 4430554 bytes uncompressed, 1058328 bytes compressed:  76.1%
+Zip file size: 1059473 bytes, number of entries: 7
+-rw-r--r--  4.6 unx     3047 b- defN 23-Apr-28 20:00 georgio-2023.118.1197.dist-info/METADATA
+-rw-r--r--  4.6 unx      129 b- defN 23-Apr-28 20:00 georgio-2023.118.1197.dist-info/WHEEL
+-rw-r--r--  4.6 unx    11350 b- defN 23-Apr-28 20:00 georgio-2023.118.1197.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx       47 b- defN 23-Apr-28 20:00 georgio-2023.118.1197.dist-info/license_files/NOTICE
+-rw-r--r--  4.6 unx      111 b- defN 23-Apr-28 20:00 georgio/__init__.py
+-rwxr-xr-x  4.6 unx  4415240 b- defN 23-Apr-28 20:00 georgio/georgio.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--  4.6 unx      630 b- defN 23-Apr-28 20:00 georgio-2023.118.1197.dist-info/RECORD
+7 files, 4430554 bytes uncompressed, 1058349 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: georgio-2023.118.1193.dist-info/METADATA
+Filename: georgio-2023.118.1197.dist-info/METADATA
 Comment: 
 
-Filename: georgio-2023.118.1193.dist-info/WHEEL
+Filename: georgio-2023.118.1197.dist-info/WHEEL
 Comment: 
 
-Filename: georgio-2023.118.1193.dist-info/license_files/LICENSE
+Filename: georgio-2023.118.1197.dist-info/license_files/LICENSE
 Comment: 
 
-Filename: georgio-2023.118.1193.dist-info/license_files/NOTICE
+Filename: georgio-2023.118.1197.dist-info/license_files/NOTICE
 Comment: 
 
 Filename: georgio/__init__.py
 Comment: 
 
 Filename: georgio/georgio.cpython-39-x86_64-linux-gnu.so
 Comment: 
 
-Filename: georgio-2023.118.1193.dist-info/RECORD
+Filename: georgio-2023.118.1197.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## georgio/georgio.cpython-39-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --sections {}

```diff
@@ -34,14 +34,14 @@
   [29] .debug_info       PROGBITS        0000000000000000 0fa7f9 0ddf76 00      0   0  1
   [30] .debug_abbrev     PROGBITS        0000000000000000 1d876f 000fc6 00      0   0  1
   [31] .debug_line       PROGBITS        0000000000000000 1d9735 06a013 00      0   0  1
   [32] .debug_str        PROGBITS        0000000000000000 243748 13d114 01  MS  0   0  1
   [33] .debug_pubtypes   PROGBITS        0000000000000000 38085c 0000c6 00      0   0  1
   [34] .debug_ranges     PROGBITS        0000000000000000 380922 091770 00      0   0  1
   [35] .symtab           SYMTAB          0000000000000000 412098 0091e0 18     36 1455  8
-  [36] .strtab           STRTAB          0000000000000000 41b278 01a190 00      0   0  1
-  [37] .shstrtab         STRTAB          0000000000000000 435408 00017e 00      0   0  1
+  [36] .strtab           STRTAB          0000000000000000 41b278 01a192 00      0   0  1
+  [37] .shstrtab         STRTAB          0000000000000000 43540a 00017e 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

### readelf --wide --symbols {}

```diff
@@ -643,64 +643,64 @@
    534: 000000000000c580     0 FUNC    LOCAL  DEFAULT   11 deregister_tm_clones
    535: 000000000000c5b0     0 FUNC    LOCAL  DEFAULT   11 register_tm_clones
    536: 000000000000c5f0     0 FUNC    LOCAL  DEFAULT   11 __do_global_dtors_aux
    537: 0000000000066128     1 OBJECT  LOCAL  DEFAULT   25 completed.0
    538: 0000000000061df8     0 OBJECT  LOCAL  DEFAULT   20 __do_global_dtors_aux_fini_array_entry
    539: 000000000000c630     0 FUNC    LOCAL  DEFAULT   11 frame_dummy
    540: 0000000000061df0     0 OBJECT  LOCAL  DEFAULT   19 __frame_dummy_init_array_entry
-   541: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.0
-   542: 000000000000c640     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17hd979f0f854fbeee6E
-   543: 000000000000c650     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17hdc1189a9e5f867d0E
-   544: 000000000000c660     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h6ba2d1048c64ea8cE
-   545: 000000000000c670   510 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_10trampoline16trampoline_inner17hba1a064a3097ec58E
+   541: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.0
+   542: 000000000000c640     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17h6064e3786872f34fE
+   543: 000000000000c650     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h166ce87cbb0731a6E
+   544: 000000000000c660     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h4e05bb1de10d2a2eE
+   545: 000000000000c670   510 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_10trampoline16trampoline_inner17he3245367a3595406E
    546: 000000000005ed50     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table3
-   547: 000000000000c870   445 FUNC    LOCAL  DEFAULT   11 _ZN7georgio33great_circle_distance_with_radius17hc145202091a4857fE
-   548: 000000000000ca30   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_69_$LT$impl$u20$georgio..great_circle_distance_with_radius..MakeDef$GT$3DEF10trampoline17hf46c34048437de85E
-   549: 000000000000caa0   611 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_46__pyfunction_great_circle_distance_with_radius17h5da6da619ffc9b9eE
-   550: 000000000000cd10   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_57_$LT$impl$u20$georgio..great_circle_distance..MakeDef$GT$3DEF10trampoline17h3d70761bf46c1bdeE
-   551: 000000000000cd80   539 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_34__pyfunction_great_circle_distance17h5c90bce25ae903b2E
-   552: 000000000000cfa0   315 FUNC    LOCAL  DEFAULT   11 _ZN7georgio27line_of_bearing_with_radius17h28decf3f8d392f2cE
-   553: 000000000000d0e0   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_63_$LT$impl$u20$georgio..line_of_bearing_with_radius..MakeDef$GT$3DEF10trampoline17h852bd0f2a84d3105E
-   554: 000000000000d150   629 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_40__pyfunction_line_of_bearing_with_radius17h4fad95cb7369fe96E
-   555: 000000000000d3d0   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_51_$LT$impl$u20$georgio..line_of_bearing..MakeDef$GT$3DEF10trampoline17ha5398f443eb6a1d7E
-   556: 000000000000d440   787 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_28__pyfunction_line_of_bearing17h5d9c3860ddbdc65bE
-   557: 000000000000d760   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_58_$LT$impl$u20$georgio..bounding_box_for_point..MakeDef$GT$3DEF10trampoline17h3a2ba0f2aa02100aE
-   558: 000000000000d7d0   828 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_35__pyfunction_bounding_box_for_point17h2b385783bc661c36E
-   559: 000000000000db10   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_49_$LT$impl$u20$georgio..wm_upper_left..MakeDef$GT$3DEF10trampoline17h2bc3e2c85f91dc42E
-   560: 000000000000db80   488 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_26__pyfunction_wm_upper_left17h678c4ad5aeb927eeE
-   561: 000000000000dd70   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_45_$LT$impl$u20$georgio..wm_bounds..MakeDef$GT$3DEF10trampoline17h51279b711e8f239dE
-   562: 000000000000dde0   686 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_22__pyfunction_wm_bounds17ha50d26ff74771c55E
-   563: 000000000000e090   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_57_$LT$impl$u20$georgio..wm_tile_expanded_bbox..MakeDef$GT$3DEF10trampoline17h6b7383039080cdd5E
-   564: 000000000000e100  1244 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_34__pyfunction_wm_tile_expanded_bbox17hd39bb6ecd146df9aE
-   565: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.1
-   566: 000000000000e880   135 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec11finish_grow17h0f0680c571a6bf5cE
-   567: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.12
-   568: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.15
-   569: 000000000000ea80     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17hd979f0f854fbeee6E
-   570: 000000000000ea90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17hdc1189a9e5f867d0E
-   571: 000000000000eaa0     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h6ba2d1048c64ea8cE
-   572: 0000000000066008   120 OBJECT  LOCAL  DEFAULT   24 _ZN7georgio7georgio3DEF17h59ce644008367a00E
+   547: 000000000000c870   445 FUNC    LOCAL  DEFAULT   11 _ZN7georgio33great_circle_distance_with_radius17h8d204aba89340480E
+   548: 000000000000ca30   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_69_$LT$impl$u20$georgio..great_circle_distance_with_radius..MakeDef$GT$3DEF10trampoline17h4a201d4e317ca937E
+   549: 000000000000caa0   611 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_46__pyfunction_great_circle_distance_with_radius17h2e75ff33b4e5382eE
+   550: 000000000000cd10   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_57_$LT$impl$u20$georgio..great_circle_distance..MakeDef$GT$3DEF10trampoline17h4a3414da561c209fE
+   551: 000000000000cd80   539 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_34__pyfunction_great_circle_distance17hcfe48c8236a03285E
+   552: 000000000000cfa0   315 FUNC    LOCAL  DEFAULT   11 _ZN7georgio27line_of_bearing_with_radius17h0995938e266a3069E
+   553: 000000000000d0e0   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_63_$LT$impl$u20$georgio..line_of_bearing_with_radius..MakeDef$GT$3DEF10trampoline17h94e4f1c05cbe97bfE
+   554: 000000000000d150   629 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_40__pyfunction_line_of_bearing_with_radius17ha25209c681204143E
+   555: 000000000000d3d0   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_51_$LT$impl$u20$georgio..line_of_bearing..MakeDef$GT$3DEF10trampoline17he73f4f45ef432c00E
+   556: 000000000000d440   787 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_28__pyfunction_line_of_bearing17h4bef21559472a755E
+   557: 000000000000d760   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_58_$LT$impl$u20$georgio..bounding_box_for_point..MakeDef$GT$3DEF10trampoline17hf9c1ddf43c25a8a2E
+   558: 000000000000d7d0   828 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_35__pyfunction_bounding_box_for_point17hc50635714e99e173E
+   559: 000000000000db10   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_49_$LT$impl$u20$georgio..wm_upper_left..MakeDef$GT$3DEF10trampoline17hb117ff3e28b8750aE
+   560: 000000000000db80   488 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_26__pyfunction_wm_upper_left17hd00bff5216eb6a99E
+   561: 000000000000dd70   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_45_$LT$impl$u20$georgio..wm_bounds..MakeDef$GT$3DEF10trampoline17ha150e425d68a517cE
+   562: 000000000000dde0   686 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_22__pyfunction_wm_bounds17h1a70f88d1486ff91E
+   563: 000000000000e090   101 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_57_$LT$impl$u20$georgio..wm_tile_expanded_bbox..MakeDef$GT$3DEF10trampoline17hc58de32b8417dbadE
+   564: 000000000000e100  1244 FUNC    LOCAL  DEFAULT   11 _ZN7georgio1_34__pyfunction_wm_tile_expanded_bbox17h4bbad28f7029c966E
+   565: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.1
+   566: 000000000000e880   135 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec11finish_grow17h8e6501fdcc414dbdE
+   567: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.12
+   568: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.15
+   569: 000000000000ea80     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17h6064e3786872f34fE
+   570: 000000000000ea90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h166ce87cbb0731a6E
+   571: 000000000000eaa0     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h4e05bb1de10d2a2eE
+   572: 0000000000066008   120 OBJECT  LOCAL  DEFAULT   24 _ZN7georgio7georgio3DEF17h9660d3e25df670a4E
    573: 000000000005ed84     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table17
-   574: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.2
-   575: 000000000000edc0    49 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast13destroy_value17h7e3909d473e99117E
-   576: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.3
-   577: 000000000000ee00    12 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr110drop_in_place$LT$core..option..Option$LT$pyo3..instance..Py$LT$pyo3..types..traceback..PyTraceback$GT$$GT$$GT$17hb3321db519edac54E
-   578: 000000000000ee10    90 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr241drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..FnOnce$LT$$LP$pyo3..marker..Python$C$$RP$$GT$$u2b$Output$u20$$u3d$$u20$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$GT$17hcc6e9d403cb3a060E
-   579: 000000000000f870    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h9f2049ced3bddf70E
+   574: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.2
+   575: 000000000000edc0    49 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast13destroy_value17h6ae8a5d519fdd9f1E
+   576: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.3
+   577: 000000000000ee00    12 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr110drop_in_place$LT$core..option..Option$LT$pyo3..instance..Py$LT$pyo3..types..traceback..PyTraceback$GT$$GT$$GT$17he12a6bc4294cbee9E
+   578: 000000000000ee10    90 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr241drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..FnOnce$LT$$LP$pyo3..marker..Python$C$$RP$$GT$$u2b$Output$u20$$u3d$$u20$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$GT$17h349d6b6f36307bf4E
+   579: 000000000000f870    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h28ba74a08386abbaE
    580: 000000000005edc0     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table1
-   581: 000000000000ee70   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17h08a08fb1d4c4bac6E
-   582: 000000000000f000     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17hd5a52c4ed0c8f64dE
+   581: 000000000000ee70   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17h1d002b062c7545f0E
+   582: 000000000000f000     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17h1568be0e80b1b17fE
    583: 000000000005edcc     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table2
-   584: 000000000000efd0    30 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr51drop_in_place$LT$alloc..vec..Vec$LT$$RF$str$GT$$GT$17h551e62ff05915647E
-   585: 000000000000eff0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17hf56cf9b9ccef5810E
+   584: 000000000000efd0    30 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr51drop_in_place$LT$alloc..vec..Vec$LT$$RF$str$GT$$GT$17h9613fb8006255fe6E
+   585: 000000000000eff0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17hb0865fc31a50c987E
    586: 000000000005ee10     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table8
-   587: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.4
+   587: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.4
    588: 000000000005ee5c     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table1
    589: 000000000005ee78     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table2
-   590: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 1f6ox68pdmgesk6m
+   590: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 1hzwlgomd2b1nozj
    591: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3.3025e9cd-cgu.15
    592: 0000000000011370    12 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17hc70a4e410a2bfd94E
    593: 0000000000011400    30 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr106drop_in_place$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$17hfc141806601d459cE
    594: 0000000000011420    12 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr110drop_in_place$LT$core..option..Option$LT$pyo3..instance..Py$LT$pyo3..types..traceback..PyTraceback$GT$$GT$$GT$17hb8e23875775acb43E
    595: 0000000000011470    90 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr241drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..FnOnce$LT$$LP$pyo3..marker..Python$C$$RP$$GT$$u2b$Output$u20$$u3d$$u20$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$GT$17hd2d66450bbfe629fE
    596: 000000000005f0e0     0 NOTYPE  LOCAL  DEFAULT   16 GCC_except_table16
    597: 0000000000011680     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17h42706df4c0e8214dE
@@ -852,23 +852,23 @@
    743: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS miniz_oxide.d3ca669e-cgu.0
    744: 0000000000043190  1404 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core9init_tree17hcc023a30b30982f2E
    745: 0000000000043710   734 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core8transfer17hb096912a935018f7E
    746: 00000000000439f0   519 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core11apply_match17h82ef3f50adbf55c1E
    747: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS adler.6e15a4ca-cgu.0
    748: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS compiler_builtins.5665bd25-cgu.118
    749: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS compiler_builtins.5665bd25-cgu.9
-   750: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.9
-   751: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.10
-   752: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.11
-   753: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.13
-   754: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.14
-   755: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.5
-   756: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.6
-   757: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.7
-   758: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.19a0936c-cgu.8
+   750: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.9
+   751: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.10
+   752: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.11
+   753: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.13
+   754: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.14
+   755: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.5
+   756: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.6
+   757: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.7
+   758: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS georgio.f1a699e4-cgu.8
    759: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3.3025e9cd-cgu.14
    760: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS parking_lot_core.caf4f90a-cgu.8
    761: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3_ffi.76b49c2d-cgu.0
    762: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3_ffi.76b49c2d-cgu.13
    763: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3_ffi.76b49c2d-cgu.14
    764: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3_ffi.76b49c2d-cgu.2
    765: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS pyo3_ffi.76b49c2d-cgu.3
@@ -888,178 +888,178 @@
    779: 000000000005ed4c     0 OBJECT  LOCAL  DEFAULT   15 __FRAME_END__
    780: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
    781: 0000000000047470    25 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$core..cell..BorrowError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1341f40a7115bc9cE
    782: 00000000000380c0     8 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..backtrace_rs..symbolize..gimli..mmap..Mmap$u20$as$u20$core..ops..deref..Deref$GT$5deref17h940c9d723c6fe175E
    783: 000000000004ca70   212 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$core..alloc..layout..Layout$u20$as$u20$core..fmt..Debug$GT$3fmt17h3fb65d0d6c14ff92E
    784: 000000000004ef56    40 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.62.llvm.17695762341781453012
    785: 0000000000049230  1065 FUNC    LOCAL  DEFAULT   11 _ZN40_$LT$str$u20$as$u20$core..fmt..Debug$GT$3fmt17hbca8056dc7eead37E
-   786: 000000000000f010   134 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument16extract_argument17h5aa1dd28737f6df0E
-   787: 000000000000c3e0   133 FUNC    LOCAL  DEFAULT   11 _ZN4core6result13unwrap_failed17hdff5465d74574b44E
-   788: 00000000000112f0   116 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot4once4Once15call_once_force28_$u7b$$u7b$closure$u7d$$u7d$17hff0123c4ecbe695bE.llvm.13238893432200692226
-   789: 0000000000042e90    82 FUNC    LOCAL  DEFAULT   11 _ZN14rustc_demangle12try_demangle17ha38d067f0b56e9b4E
-   790: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRecursionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hbc35a11eab29e87bE
-   791: 000000000002fbf0   155 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hb63e126ce5a19bfaE
-   792: 0000000000014450    46 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h666e3307e953261aE
-   793: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Display$GT$3fmt17had475fdba9668400E
-   794: 000000000000e5e0   662 FUNC    LOCAL  DEFAULT   11 _ZN7georgio7georgio17h1b44db711282ebdbE
-   795: 0000000000009350   670 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35panic14PanicException18from_panic_payload17h430c4279adfc8d88E
-   796: 0000000000011bc0   266 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$pyo3..gil..GILPool$u20$as$u20$core..ops..drop..Drop$GT$4drop17h08e135a338916b16E
-   797: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyReferenceError$u20$as$u20$core..fmt..Debug$GT$3fmt17h901dbbe4b250cbe8E
-   798: 000000000000a320   688 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot9raw_mutex8RawMutex11unlock_slow17h103fe67ba22e95e2E
-   799: 0000000000012220    90 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr233drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..Fn$LT$$LP$$RF$pyo3..pyclass..create_type_object..PyTypeBuilder$C$$BP$mut$u20$pyo3_ffi..cpython..object..PyTypeObject$RP$$GT$$u2b$Output$u20$$u3d$$u20$$LP$$RP$$GT$$GT$17he316ae0b535df138E.llvm.11213889763605633493
-   800: 000000000004b930   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u32$GT$3fmt17h38717ee80e1406eeE
-   801: 0000000000012440    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h55d6234f69ffbd67E.llvm.11213889763605633493
-   802: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyTimeoutError$u20$as$u20$core..fmt..Display$GT$3fmt17h9712959ebdfc92a3E
-   803: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr117drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..str..error..Utf8Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hc41583d1f0be50bbE.llvm.3160907281880781123
-   804: 0000000000066130     8 OBJECT  LOCAL  DEFAULT   25 _ZN4pyo35panic14PanicException15type_object_raw11TYPE_OBJECT17hb4dc0203f02f3a3dE.llvm.5697929769133057476
-   805: 0000000000046850   256 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3ffi5c_str7CString19_from_vec_unchecked17h62597843d8fbe120E
-   806: 000000000004e6dc    23 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.31.llvm.1386185271139027476
-   807: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyImportWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h3e2dbfbce7a5d844E
-   808: 0000000000015bb0   213 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$T$u20$as$u20$pyo3..err..err_state..PyErrArguments$GT$9arguments17h0f0e2e9c11d38626E
-   809: 000000000000fea0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$u64$C$pyo3..err..PyErr$GT$$GT$17h4bf2d0703230475cE.llvm.18356750485614513129
-   810: 000000000000fa10     5 FUNC    LOCAL  DEFAULT   11 __rust_realloc
-   811: 0000000000062e40    24 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.6.llvm.8364735172703476354
-   812: 00000000000310f0   358 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix2fs4stat17h0e8d201e9293885bE
-   813: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$isize$GT$3fmt17hc7c4a8a0b43a9cb6E
-   814: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyIsADirectoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17hfd091bbda7e13da6E
-   815: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..asyncio..LimitOverrunError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1f4ebc3eec972281E
-   816: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyStopAsyncIteration$u20$as$u20$core..fmt..Debug$GT$3fmt17hc950ec3c6ea55917E
-   817: 0000000000062ca0    32 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.2.llvm.17695762341781453012
-   818: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Display$GT$3fmt17heb24a244de2c3c3fE
-   819: 000000000000c490     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index22slice_index_order_fail17h1f8a4ffeb1c00eb3E
-   820: 000000000002a790   230 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread6Thread3new17hb785c38d161c9c58E
-   821: 00000000000114d0    19 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr272drop_in_place$LT$lock_api..mutex..MutexGuard$LT$parking_lot..raw_mutex..RawMutex$C$$LP$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$C$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$RP$$GT$$GT$17hfae2b136a28cfc8eE.llvm.13238893432200692226
-   822: 00000000000624b8    32 OBJECT  LOCAL  DEFAULT   21 anon.96baa08bd4660f1c11ddd83a253e848d.0.llvm.3755404211422290406
-   823: 0000000000062cc0    24 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.10.llvm.17695762341781453012
-   824: 000000000003a2b0   194 FUNC    LOCAL  DEFAULT   11 __rust_start_panic
-   825: 000000000004e3dd    16 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.30.llvm.18356750485614513129
-   826: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyFileNotFoundError$u20$as$u20$core..fmt..Debug$GT$3fmt17h7d43a138ee1eb2edE
-   827: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyOverflowError$u20$as$u20$core..fmt..Debug$GT$3fmt17hf8ba314932d8a377E
-   828: 000000000004ed00    45 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.5.llvm.17695762341781453012
-   829: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i64$GT$3fmt17hadac23219b3f02f1E
-   830: 0000000000014680   513 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule5index17heeed66a24f2c17ddE
-   831: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyBytesWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hb72010652b12aecaE
-   832: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyRecursionError$u20$as$u20$core..fmt..Display$GT$3fmt17he096da8c5b1f6b58E
-   833: 0000000000009790   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$7reserve21do_reserve_and_handle17h5fd73e599ec51fbdE
-   834: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.11213889763605633493
-   835: 0000000000046650     9 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc18handle_alloc_error8rt_error17h4b79f8a717741b7cE
-   836: 000000000000fa60   506 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local17LocalKey$LT$T$GT$4with17h771d0fd2b2280c3aE
-   837: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr74drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..tuple..PyTuple$GT$$GT$17h6182412f885ebc33E.llvm.11213889763605633493
-   838: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyIndexError$u20$as$u20$core..fmt..Debug$GT$3fmt17h20dcaeb108562508E
-   839: 0000000000048e40    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter15debug_lower_hex17heb5fb064687c1b3cE
-   840: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionRefusedError$u20$as$u20$core..fmt..Debug$GT$3fmt17he7be66925f89c435E
-   841: 0000000000062850    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.52.llvm.1386185271139027476
-   842: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyFutureWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hb2c24c04d62bed65E
-   843: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyStopAsyncIteration$u20$as$u20$core..fmt..Display$GT$3fmt17hbed917b05b5b3dc9E
-   844: 0000000000015780    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$alloc..string..String$GT$17hada97ac0ee8fd35cE.llvm.3041393958569974349
-   845: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyPermissionError$u20$as$u20$core..fmt..Display$GT$3fmt17heac4af63d9da8e0cE
-   846: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyTimeoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h43beacce270ef9b0E
-   847: 0000000000049b90   274 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice6memchr14memchr_aligned17h0425dc535282f001E
-   848: 000000000000c030     8 FUNC    LOCAL  DEFAULT   11 _ZN4core6option13expect_failed17h09b982639336e7eaE
-   849: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyUnboundLocalError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd6f86235abaca577E
-   850: 0000000000047cb0   331 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders10DebugTuple5field17hbc0d06249379c2b0E
-   851: 000000000000a750   244 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core9word_lock8WordLock11unlock_slow17ha2d7f5843e1c2a04E
-   852: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr120drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..array..TryFromSliceError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h524a32b3308b2d42E.llvm.3160907281880781123
-   853: 0000000000062630    32 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.21.llvm.18356750485614513129
-   854: 0000000000062e10    48 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.4.llvm.8364735172703476354
-   855: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyUnicodeError$u20$as$u20$core..fmt..Display$GT$3fmt17h78e358a42b97532dE
-   856: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyEnvironmentError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha7a7d75ad3f4ca36E
-   857: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyModuleNotFoundError$u20$as$u20$core..fmt..Display$GT$3fmt17hb42ea06e60b64cd3E
-   858: 00000000000095f0   244 FUNC    LOCAL  DEFAULT   11 _ZN4pyo34sync20GILOnceCell$LT$T$GT$4init17hc1891bbae199820aE
-   859: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN83_$LT$pyo3..exceptions..asyncio..IncompleteReadError$u20$as$u20$core..fmt..Debug$GT$3fmt17h2778d37147d404e1E
-   860: 00000000000144f0   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.17695762341781453012
-   861: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..types..pysuper..PySuper$u20$as$u20$core..fmt..Debug$GT$3fmt17hfa7691b1b170c85aE
-   862: 00000000000167b0    16 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17he80ade25e775a4dcE.llvm.8364735172703476354
-   863: 00000000000111e0   209 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$pyo3..err..PyErr$u20$as$u20$core..convert..From$LT$pyo3..err..PyDowncastError$GT$$GT$4from17h7bf6063a4dacbf54E
-   864: 0000000000015ca0    36 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$alloc..borrow..Cow$LT$B$GT$$u20$as$u20$core..fmt..Display$GT$3fmt17ha186b3c0f7b72edaE
-   865: 0000000000000070    56 TLS     LOCAL  DEFAULT   18 _ZN16parking_lot_core11parking_lot16with_thread_data11THREAD_DATA7__getit5__KEY17hfc24aedae5303aaeE
-   866: 000000000000fd10   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.18356750485614513129
-   867: 000000000004ed58    82 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.9.llvm.17695762341781453012
-   868: 0000000000010560    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr65drop_in_place$LT$core..option..Option$LT$pyo3..err..PyErr$GT$$GT$17hfb4ab78da4d292adE.llvm.1386185271139027476
-   869: 0000000000017490    28 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr81drop_in_place$LT$alloc..vec..Vec$LT$parking_lot_core..parking_lot..Bucket$GT$$GT$17h306dca86cce70bcbE.llvm.11926435696733617703
-   870: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i64$GT$3fmt17hbedecd2bf46d1109E
-   871: 0000000000016aa0   215 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write10write_char17hfafc9261f4a524b3E
-   872: 000000000003c4e0    74 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev10Attributes3new17h1b99a887e63fcf65E
-   873: 000000000002f080     6 FUNC    LOCAL  DEFAULT   11 __rdl_dealloc
-   874: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.13238893432200692226
-   875: 000000000000ecf0   204 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17ha6ae3d8064512259E.llvm.3109625712416505353
-   876: 000000000002f130   117 FUNC    LOCAL  DEFAULT   11 __rdl_alloc_zeroed
-   877: 000000000004c920   331 FUNC    LOCAL  DEFAULT   11 _ZN4core7unicode12unicode_data15grapheme_extend6lookup17hd769465f95e4f17eE
-   878: 0000000000009260   198 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription37missing_required_positional_arguments17h4aaab2d80d41aa06E
-   879: 0000000000017560    99 FUNC    LOCAL  DEFAULT   11 _ZN65_$LT$smallvec..CollectionAllocErr$u20$as$u20$core..fmt..Debug$GT$3fmt17h348d4076a78dfa05E
-   880: 0000000000030c60    40 FUNC    LOCAL  DEFAULT   11 _ZN62_$LT$std..io..error..ErrorKind$u20$as$u20$core..fmt..Debug$GT$3fmt17hc0835769217bb923E
-   881: 0000000000010850   592 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr4take17h40241a7302745234E
-   882: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyBlockingIOError$u20$as$u20$core..fmt..Display$GT$3fmt17h1617c0cce31ee381E
-   883: 000000000002fc90    72 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$std..panicking..begin_panic_handler..StrPanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17hb536e81ec06af68dE
-   884: 000000000004e6c6    22 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.30.llvm.1386185271139027476
-   885: 000000000000c480     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index24slice_end_index_len_fail17h954ac87ccda54c62E
-   886: 00000000000170c0    28 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot11FairTimeout7gen_u3217ha9b92ff54ec47786E
-   887: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyUnicodeWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h340ed8ec354ed6a8E
-   888: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionResetError$u20$as$u20$core..fmt..Display$GT$3fmt17h8976d587936b6703E
-   889: 0000000000008230   592 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument25argument_extraction_error17hcc5846e9b8369abcE
-   890: 000000000004a040  1663 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5count14do_count_chars17h7ea02efffe3b2a1eE
-   891: 000000000004e662    46 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.27.llvm.1386185271139027476
-   892: 0000000000011cd0   257 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil15register_decref17h633f948c49d68cd7E
-   893: 000000000003d5c0  2886 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$rustc_demangle..legacy..Demangle$u20$as$u20$core..fmt..Display$GT$3fmt17h2a9c2521f98eeafcE
-   894: 0000000000013cd0    19 FUNC    LOCAL  DEFAULT   11 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h8e203ea97de01bdeE
-   895: 000000000000fec0    90 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking13panic_display17h0e52f2d4da7fc211E.llvm.18356750485614513129
-   896: 000000000004cbdf    57 FUNC    LOCAL  DEFAULT   11 __rust_probestack
-   897: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyNotImplementedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6bab9bbc77f02eb0E
-   898: 0000000000015230    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17hcd6cdfe90aaae05dE
-   899: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyBytesWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h21116da12387d51bE
-   900: 0000000000062de0    24 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.1.llvm.8364735172703476354
-   901: 0000000000054220     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
-   902: 0000000000063fb0    16 OBJECT  LOCAL  DEFAULT   21 _ZN6object3elf12ELF_NOTE_GNU17hfa4096b3f4b71b6dE
-   903: 000000000004c460   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp54_$LT$impl$u20$core..fmt..Display$u20$for$u20$usize$GT$3fmt17h379f79964edced29E
-   904: 0000000000013f70    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$alloc..string..String$GT$17hada97ac0ee8fd35cE.llvm.5697929769133057476
-   905: 0000000000010150   656 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std3num64_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$u32$GT$7extract17he39022322b8be308E
-   906: 000000000004e2da    79 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.8.llvm.18356750485614513129
-   907: 000000000004cc40     0 FUNC    LOCAL  DEFAULT   12 _fini
-   908: 0000000000031580     3 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5flush17h1a44ae04bd6f44c0E
-   909: 00000000000170e0   571 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot10ThreadData3new17he310ca209c68f23aE
-   910: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRuntimeWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h0cf2ae104cdc07ddE
-   911: 0000000000066000     8 OBJECT  LOCAL  DEFAULT   24 DW.ref.rust_eh_personality
-   912: 0000000000012e20    34 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h220ac3815ffc2c7dE.llvm.3160907281880781123
-   913: 0000000000047fa0    14 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders9DebugList5entry17hb9fff6b0c114051bE
-   914: 00000000000174b0   150 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3vec16Vec$LT$T$C$A$GT$16into_boxed_slice17h71e443bf4e876c92E
-   915: 000000000002f030    72 FUNC    LOCAL  DEFAULT   11 __rdl_alloc
-   916: 0000000000012e90    43 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hefa1e3e3960d0478E.llvm.3160907281880781123
-   917: 000000000004cc30    15 FUNC    LOCAL  DEFAULT   11 fstat64
-   918: 0000000000016100   207 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h4057060e368158d4E.llvm.11499977999870449161
-   919: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Display$GT$3fmt17hcdf689e84d830531E
-   920: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6548821cb49f34caE
-   921: 0000000000048e50    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter15debug_upper_hex17h4ae5ad4f6f2aa1d0E
-   922: 0000000000016d30   170 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$std..io..Write..write_fmt..Adapter$LT$T$GT$$u20$as$u20$core..fmt..Write$GT$9write_str17ha9be46769c3b856fE
-   923: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyRuntimeWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h9a6e38b075e35938E
-   924: 000000000004f265    28 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.2.llvm.8364735172703476354
-   925: 000000000004f2bb    85 OBJECT  LOCAL  DEFAULT   13 anon.e9136d4cc2f2bf733d592b5df8895207.2.llvm.17368754240468033560
-   926: 0000000000011ea0    36 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6string8PyString3new17h299959edd40321a2E
-   927: 000000000004cb50    25 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$core..alloc..layout..LayoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h05fc90456a37551fE
-   928: 00000000000466e0   355 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$$RF$str$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17h4f63cbf55da6c9bfE
-   929: 000000000000c4a0   116 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice29_$LT$impl$u20$$u5b$T$u5d$$GT$15copy_from_slice17len_mismatch_fail17h574184041027afeeE
-   930: 00000000000314b0    91 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5write17hbc541aca9a839525E
-   931: 00000000000096f0   152 FUNC    LOCAL  DEFAULT   11 _ZN4pyo34sync20GILOnceCell$LT$T$GT$4init17hf759f6fb2a9ea8d5E
-   932: 0000000000011de0   189 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil14register_owned17he07681caaf031a88E
-   933: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..types..bytearray..PyByteArray$u20$as$u20$core..fmt..Debug$GT$3fmt17h9ed6949921d7f740E
-   934: 000000000000a5f0   342 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core9word_lock8WordLock9lock_slow17ha8785b00dd2fc6d4E
-   935: 000000000002baa0   283 FUNC    LOCAL  DEFAULT   11 _ZN61_$LT$std..io..stdio..StderrLock$u20$as$u20$std..io..Write$GT$9write_all17h354a7d449f101f10E
-   936: 0000000000046950   486 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3fmt6format12format_inner17hb8a7cc9ead64df92E
-   937: 0000000000047130    68 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$alloc..ffi..c_str..NulError$u20$as$u20$core..fmt..Debug$GT$3fmt17h32068101aae54749E
-   938: 0000000000047c60    77 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders11DebugStruct6finish17h2684bb4eb733b8beE
-   939: 00000000000301b0   212 FUNC    LOCAL  DEFAULT   11 rust_panic
-   940: 0000000000042ef0     9 FUNC    LOCAL  DEFAULT   11 _ZN14rustc_demangle8Demangle6as_str17h7ac9e5628dfe27b4E
-   941: 00000000000167d0    27 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$3get17h77154b0a47b02f05E
-   942: 0000000000048e30    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9alternate17h1a3805d113b9007fE
-   943: 0000000000016e30    11 FUNC    LOCAL  DEFAULT   11 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h3b2256eaf5b2d864E
-   944: 0000000000013cf0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.11940621367560662805
-   945: 0000000000031260   315 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix2fs12canonicalize17hbb7a977ea3596806E
-   946: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyEOFError$u20$as$u20$core..fmt..Display$GT$3fmt17h66301cdb51d144cdE
-   947: 000000000004eb1b     8 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.18.llvm.17695762341781453012
-   948: 0000000000013800   144 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types10typeobject6PyType4name17heeb35ac9933d480dE
-   949: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..asyncio..CancelledError$u20$as$u20$core..fmt..Debug$GT$3fmt17h99a04508eedb7eb2E
+   786: 000000000000c3e0   133 FUNC    LOCAL  DEFAULT   11 _ZN4core6result13unwrap_failed17hdff5465d74574b44E
+   787: 00000000000112f0   116 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot4once4Once15call_once_force28_$u7b$$u7b$closure$u7d$$u7d$17hff0123c4ecbe695bE.llvm.13238893432200692226
+   788: 0000000000042e90    82 FUNC    LOCAL  DEFAULT   11 _ZN14rustc_demangle12try_demangle17ha38d067f0b56e9b4E
+   789: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRecursionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hbc35a11eab29e87bE
+   790: 000000000002fbf0   155 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hb63e126ce5a19bfaE
+   791: 0000000000014450    46 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h666e3307e953261aE
+   792: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Display$GT$3fmt17had475fdba9668400E
+   793: 0000000000009350   670 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35panic14PanicException18from_panic_payload17h430c4279adfc8d88E
+   794: 0000000000011bc0   266 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$pyo3..gil..GILPool$u20$as$u20$core..ops..drop..Drop$GT$4drop17h08e135a338916b16E
+   795: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyReferenceError$u20$as$u20$core..fmt..Debug$GT$3fmt17h901dbbe4b250cbe8E
+   796: 000000000000a320   688 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot9raw_mutex8RawMutex11unlock_slow17h103fe67ba22e95e2E
+   797: 0000000000012220    90 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr233drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..Fn$LT$$LP$$RF$pyo3..pyclass..create_type_object..PyTypeBuilder$C$$BP$mut$u20$pyo3_ffi..cpython..object..PyTypeObject$RP$$GT$$u2b$Output$u20$$u3d$$u20$$LP$$RP$$GT$$GT$17he316ae0b535df138E.llvm.11213889763605633493
+   798: 000000000004b930   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u32$GT$3fmt17h38717ee80e1406eeE
+   799: 0000000000012440    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h55d6234f69ffbd67E.llvm.11213889763605633493
+   800: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyTimeoutError$u20$as$u20$core..fmt..Display$GT$3fmt17h9712959ebdfc92a3E
+   801: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr117drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..str..error..Utf8Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hc41583d1f0be50bbE.llvm.3160907281880781123
+   802: 0000000000066130     8 OBJECT  LOCAL  DEFAULT   25 _ZN4pyo35panic14PanicException15type_object_raw11TYPE_OBJECT17hb4dc0203f02f3a3dE.llvm.5697929769133057476
+   803: 0000000000046850   256 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3ffi5c_str7CString19_from_vec_unchecked17h62597843d8fbe120E
+   804: 000000000004e6dc    23 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.31.llvm.1386185271139027476
+   805: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyImportWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h3e2dbfbce7a5d844E
+   806: 000000000000ecb0   204 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h4c985098722996e9E.llvm.11200713541412871589
+   807: 0000000000015bb0   213 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$T$u20$as$u20$pyo3..err..err_state..PyErrArguments$GT$9arguments17h0f0e2e9c11d38626E
+   808: 000000000000fea0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$u64$C$pyo3..err..PyErr$GT$$GT$17h4bf2d0703230475cE.llvm.18356750485614513129
+   809: 000000000000fa10     5 FUNC    LOCAL  DEFAULT   11 __rust_realloc
+   810: 0000000000062e40    24 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.6.llvm.8364735172703476354
+   811: 00000000000310f0   358 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix2fs4stat17h0e8d201e9293885bE
+   812: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$isize$GT$3fmt17hc7c4a8a0b43a9cb6E
+   813: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyIsADirectoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17hfd091bbda7e13da6E
+   814: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..asyncio..LimitOverrunError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1f4ebc3eec972281E
+   815: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyStopAsyncIteration$u20$as$u20$core..fmt..Debug$GT$3fmt17hc950ec3c6ea55917E
+   816: 0000000000062ca0    32 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.2.llvm.17695762341781453012
+   817: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Display$GT$3fmt17heb24a244de2c3c3fE
+   818: 000000000000c490     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index22slice_index_order_fail17h1f8a4ffeb1c00eb3E
+   819: 000000000002a790   230 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread6Thread3new17hb785c38d161c9c58E
+   820: 00000000000114d0    19 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr272drop_in_place$LT$lock_api..mutex..MutexGuard$LT$parking_lot..raw_mutex..RawMutex$C$$LP$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$C$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$RP$$GT$$GT$17hfae2b136a28cfc8eE.llvm.13238893432200692226
+   821: 0000000000062cc0    24 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.10.llvm.17695762341781453012
+   822: 000000000003a2b0   194 FUNC    LOCAL  DEFAULT   11 __rust_start_panic
+   823: 000000000004e3dd    16 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.30.llvm.18356750485614513129
+   824: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyFileNotFoundError$u20$as$u20$core..fmt..Debug$GT$3fmt17h7d43a138ee1eb2edE
+   825: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyOverflowError$u20$as$u20$core..fmt..Debug$GT$3fmt17hf8ba314932d8a377E
+   826: 000000000004ed00    45 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.5.llvm.17695762341781453012
+   827: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i64$GT$3fmt17hadac23219b3f02f1E
+   828: 0000000000014680   513 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule5index17heeed66a24f2c17ddE
+   829: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyBytesWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hb72010652b12aecaE
+   830: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyRecursionError$u20$as$u20$core..fmt..Display$GT$3fmt17he096da8c5b1f6b58E
+   831: 0000000000009790   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$7reserve21do_reserve_and_handle17h5fd73e599ec51fbdE
+   832: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.11213889763605633493
+   833: 0000000000046650     9 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc18handle_alloc_error8rt_error17h4b79f8a717741b7cE
+   834: 000000000000fa60   506 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local17LocalKey$LT$T$GT$4with17h771d0fd2b2280c3aE
+   835: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr74drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..tuple..PyTuple$GT$$GT$17h6182412f885ebc33E.llvm.11213889763605633493
+   836: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyIndexError$u20$as$u20$core..fmt..Debug$GT$3fmt17h20dcaeb108562508E
+   837: 0000000000048e40    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter15debug_lower_hex17heb5fb064687c1b3cE
+   838: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionRefusedError$u20$as$u20$core..fmt..Debug$GT$3fmt17he7be66925f89c435E
+   839: 0000000000062850    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.52.llvm.1386185271139027476
+   840: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyFutureWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hb2c24c04d62bed65E
+   841: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyStopAsyncIteration$u20$as$u20$core..fmt..Display$GT$3fmt17hbed917b05b5b3dc9E
+   842: 0000000000015780    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$alloc..string..String$GT$17hada97ac0ee8fd35cE.llvm.3041393958569974349
+   843: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyPermissionError$u20$as$u20$core..fmt..Display$GT$3fmt17heac4af63d9da8e0cE
+   844: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyTimeoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h43beacce270ef9b0E
+   845: 0000000000049b90   274 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice6memchr14memchr_aligned17h0425dc535282f001E
+   846: 000000000000c030     8 FUNC    LOCAL  DEFAULT   11 _ZN4core6option13expect_failed17h09b982639336e7eaE
+   847: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyUnboundLocalError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd6f86235abaca577E
+   848: 0000000000047cb0   331 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders10DebugTuple5field17hbc0d06249379c2b0E
+   849: 000000000000a750   244 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core9word_lock8WordLock11unlock_slow17ha2d7f5843e1c2a04E
+   850: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr120drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..array..TryFromSliceError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h524a32b3308b2d42E.llvm.3160907281880781123
+   851: 0000000000062630    32 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.21.llvm.18356750485614513129
+   852: 0000000000062e10    48 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.4.llvm.8364735172703476354
+   853: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyUnicodeError$u20$as$u20$core..fmt..Display$GT$3fmt17h78e358a42b97532dE
+   854: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyEnvironmentError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha7a7d75ad3f4ca36E
+   855: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyModuleNotFoundError$u20$as$u20$core..fmt..Display$GT$3fmt17hb42ea06e60b64cd3E
+   856: 00000000000095f0   244 FUNC    LOCAL  DEFAULT   11 _ZN4pyo34sync20GILOnceCell$LT$T$GT$4init17hc1891bbae199820aE
+   857: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN83_$LT$pyo3..exceptions..asyncio..IncompleteReadError$u20$as$u20$core..fmt..Debug$GT$3fmt17h2778d37147d404e1E
+   858: 00000000000144f0   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.17695762341781453012
+   859: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..types..pysuper..PySuper$u20$as$u20$core..fmt..Debug$GT$3fmt17hfa7691b1b170c85aE
+   860: 00000000000167b0    16 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17he80ade25e775a4dcE.llvm.8364735172703476354
+   861: 00000000000111e0   209 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$pyo3..err..PyErr$u20$as$u20$core..convert..From$LT$pyo3..err..PyDowncastError$GT$$GT$4from17h7bf6063a4dacbf54E
+   862: 0000000000015ca0    36 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$alloc..borrow..Cow$LT$B$GT$$u20$as$u20$core..fmt..Display$GT$3fmt17ha186b3c0f7b72edaE
+   863: 0000000000000070    56 TLS     LOCAL  DEFAULT   18 _ZN16parking_lot_core11parking_lot16with_thread_data11THREAD_DATA7__getit5__KEY17hfc24aedae5303aaeE
+   864: 000000000000fd10   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.18356750485614513129
+   865: 000000000004ed58    82 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.9.llvm.17695762341781453012
+   866: 0000000000010560    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr65drop_in_place$LT$core..option..Option$LT$pyo3..err..PyErr$GT$$GT$17hfb4ab78da4d292adE.llvm.1386185271139027476
+   867: 0000000000017490    28 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr81drop_in_place$LT$alloc..vec..Vec$LT$parking_lot_core..parking_lot..Bucket$GT$$GT$17h306dca86cce70bcbE.llvm.11926435696733617703
+   868: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i64$GT$3fmt17hbedecd2bf46d1109E
+   869: 0000000000016aa0   215 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write10write_char17hfafc9261f4a524b3E
+   870: 000000000003c4e0    74 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev10Attributes3new17h1b99a887e63fcf65E
+   871: 000000000002f080     6 FUNC    LOCAL  DEFAULT   11 __rdl_dealloc
+   872: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.13238893432200692226
+   873: 000000000002f130   117 FUNC    LOCAL  DEFAULT   11 __rdl_alloc_zeroed
+   874: 000000000004c920   331 FUNC    LOCAL  DEFAULT   11 _ZN4core7unicode12unicode_data15grapheme_extend6lookup17hd769465f95e4f17eE
+   875: 0000000000009260   198 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription37missing_required_positional_arguments17h4aaab2d80d41aa06E
+   876: 0000000000017560    99 FUNC    LOCAL  DEFAULT   11 _ZN65_$LT$smallvec..CollectionAllocErr$u20$as$u20$core..fmt..Debug$GT$3fmt17h348d4076a78dfa05E
+   877: 0000000000030c60    40 FUNC    LOCAL  DEFAULT   11 _ZN62_$LT$std..io..error..ErrorKind$u20$as$u20$core..fmt..Debug$GT$3fmt17hc0835769217bb923E
+   878: 0000000000010850   592 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr4take17h40241a7302745234E
+   879: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyBlockingIOError$u20$as$u20$core..fmt..Display$GT$3fmt17h1617c0cce31ee381E
+   880: 000000000002fc90    72 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$std..panicking..begin_panic_handler..StrPanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17hb536e81ec06af68dE
+   881: 000000000004e6c6    22 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.30.llvm.1386185271139027476
+   882: 000000000000c480     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index24slice_end_index_len_fail17h954ac87ccda54c62E
+   883: 00000000000170c0    28 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot11FairTimeout7gen_u3217ha9b92ff54ec47786E
+   884: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyUnicodeWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h340ed8ec354ed6a8E
+   885: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionResetError$u20$as$u20$core..fmt..Display$GT$3fmt17h8976d587936b6703E
+   886: 0000000000008230   592 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument25argument_extraction_error17hcc5846e9b8369abcE
+   887: 000000000004a040  1663 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5count14do_count_chars17h7ea02efffe3b2a1eE
+   888: 000000000004e662    46 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.27.llvm.1386185271139027476
+   889: 0000000000011cd0   257 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil15register_decref17h633f948c49d68cd7E
+   890: 000000000003d5c0  2886 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$rustc_demangle..legacy..Demangle$u20$as$u20$core..fmt..Display$GT$3fmt17h2a9c2521f98eeafcE
+   891: 0000000000013cd0    19 FUNC    LOCAL  DEFAULT   11 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h8e203ea97de01bdeE
+   892: 000000000000fec0    90 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking13panic_display17h0e52f2d4da7fc211E.llvm.18356750485614513129
+   893: 000000000004cbdf    57 FUNC    LOCAL  DEFAULT   11 __rust_probestack
+   894: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyNotImplementedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6bab9bbc77f02eb0E
+   895: 0000000000015230    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17hcd6cdfe90aaae05dE
+   896: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyBytesWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h21116da12387d51bE
+   897: 0000000000062de0    24 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.1.llvm.8364735172703476354
+   898: 000000000000f010   134 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument16extract_argument17h363e3443f9534907E
+   899: 0000000000054220     0 NOTYPE  LOCAL  DEFAULT   14 __GNU_EH_FRAME_HDR
+   900: 0000000000063fb0    16 OBJECT  LOCAL  DEFAULT   21 _ZN6object3elf12ELF_NOTE_GNU17hfa4096b3f4b71b6dE
+   901: 000000000004c460   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp54_$LT$impl$u20$core..fmt..Display$u20$for$u20$usize$GT$3fmt17h379f79964edced29E
+   902: 0000000000013f70    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$alloc..string..String$GT$17hada97ac0ee8fd35cE.llvm.5697929769133057476
+   903: 0000000000010150   656 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std3num64_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$u32$GT$7extract17he39022322b8be308E
+   904: 000000000004e2da    79 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.8.llvm.18356750485614513129
+   905: 000000000004cc40     0 FUNC    LOCAL  DEFAULT   12 _fini
+   906: 0000000000031580     3 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5flush17h1a44ae04bd6f44c0E
+   907: 00000000000170e0   571 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot10ThreadData3new17he310ca209c68f23aE
+   908: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRuntimeWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h0cf2ae104cdc07ddE
+   909: 0000000000066000     8 OBJECT  LOCAL  DEFAULT   24 DW.ref.rust_eh_personality
+   910: 0000000000012e20    34 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h220ac3815ffc2c7dE.llvm.3160907281880781123
+   911: 0000000000047fa0    14 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders9DebugList5entry17hb9fff6b0c114051bE
+   912: 00000000000174b0   150 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3vec16Vec$LT$T$C$A$GT$16into_boxed_slice17h71e443bf4e876c92E
+   913: 000000000002f030    72 FUNC    LOCAL  DEFAULT   11 __rdl_alloc
+   914: 0000000000012e90    43 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hefa1e3e3960d0478E.llvm.3160907281880781123
+   915: 000000000004cc30    15 FUNC    LOCAL  DEFAULT   11 fstat64
+   916: 0000000000016100   207 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h4057060e368158d4E.llvm.11499977999870449161
+   917: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Display$GT$3fmt17hcdf689e84d830531E
+   918: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6548821cb49f34caE
+   919: 0000000000048e50    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter15debug_upper_hex17h4ae5ad4f6f2aa1d0E
+   920: 0000000000016d30   170 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$std..io..Write..write_fmt..Adapter$LT$T$GT$$u20$as$u20$core..fmt..Write$GT$9write_str17ha9be46769c3b856fE
+   921: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyRuntimeWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h9a6e38b075e35938E
+   922: 000000000000ea30    71 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err9err_state10boxed_args17h34b781837ee78ca7E
+   923: 000000000004f265    28 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.2.llvm.8364735172703476354
+   924: 000000000004f2bb    85 OBJECT  LOCAL  DEFAULT   13 anon.e9136d4cc2f2bf733d592b5df8895207.2.llvm.17368754240468033560
+   925: 0000000000011ea0    36 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6string8PyString3new17h299959edd40321a2E
+   926: 000000000004cb50    25 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$core..alloc..layout..LayoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h05fc90456a37551fE
+   927: 00000000000466e0   355 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$$RF$str$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17h4f63cbf55da6c9bfE
+   928: 000000000000c4a0   116 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice29_$LT$impl$u20$$u5b$T$u5d$$GT$15copy_from_slice17len_mismatch_fail17h574184041027afeeE
+   929: 00000000000314b0    91 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5write17hbc541aca9a839525E
+   930: 00000000000096f0   152 FUNC    LOCAL  DEFAULT   11 _ZN4pyo34sync20GILOnceCell$LT$T$GT$4init17hf759f6fb2a9ea8d5E
+   931: 0000000000011de0   189 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil14register_owned17he07681caaf031a88E
+   932: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..types..bytearray..PyByteArray$u20$as$u20$core..fmt..Debug$GT$3fmt17h9ed6949921d7f740E
+   933: 000000000000a5f0   342 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core9word_lock8WordLock9lock_slow17ha8785b00dd2fc6d4E
+   934: 000000000002baa0   283 FUNC    LOCAL  DEFAULT   11 _ZN61_$LT$std..io..stdio..StderrLock$u20$as$u20$std..io..Write$GT$9write_all17h354a7d449f101f10E
+   935: 0000000000046950   486 FUNC    LOCAL  DEFAULT   11 _ZN5alloc3fmt6format12format_inner17hb8a7cc9ead64df92E
+   936: 0000000000047130    68 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$alloc..ffi..c_str..NulError$u20$as$u20$core..fmt..Debug$GT$3fmt17h32068101aae54749E
+   937: 0000000000047c60    77 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders11DebugStruct6finish17h2684bb4eb733b8beE
+   938: 00000000000301b0   212 FUNC    LOCAL  DEFAULT   11 rust_panic
+   939: 0000000000042ef0     9 FUNC    LOCAL  DEFAULT   11 _ZN14rustc_demangle8Demangle6as_str17h7ac9e5628dfe27b4E
+   940: 00000000000167d0    27 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$3get17h77154b0a47b02f05E
+   941: 0000000000048e30    10 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9alternate17h1a3805d113b9007fE
+   942: 0000000000016e30    11 FUNC    LOCAL  DEFAULT   11 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h3b2256eaf5b2d864E
+   943: 0000000000013cf0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.11940621367560662805
+   944: 0000000000031260   315 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix2fs12canonicalize17hbb7a977ea3596806E
+   945: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyEOFError$u20$as$u20$core..fmt..Display$GT$3fmt17h66301cdb51d144cdE
+   946: 000000000004eb1b     8 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.18.llvm.17695762341781453012
+   947: 0000000000013800   144 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types10typeobject6PyType4name17heeb35ac9933d480dE
+   948: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..asyncio..CancelledError$u20$as$u20$core..fmt..Debug$GT$3fmt17h99a04508eedb7eb2E
+   949: 000000000000f920   194 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple137_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$C$T2$C$T3$RP$$GT$7into_py17h77fc8d3e8f6025c2E
    950: 0000000000062df8    24 OBJECT  LOCAL  DEFAULT   21 anon.9e114ed5010d6253bd261129473cd188.3.llvm.8364735172703476354
    951: 000000000000c1f0    21 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking19panic_cannot_unwind17hd123d9c71473dcdaE
    952: 0000000000048de0    16 FUNC    LOCAL  DEFAULT   11 _ZN57_$LT$core..fmt..Formatter$u20$as$u20$core..fmt..Write$GT$9write_str17h317c4bebb297f401E
    953: 0000000000010b00   707 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr8new_type17had5c31a5cd10e380E
    954: 0000000000065598     0 OBJECT  LOCAL  DEFAULT   23 _GLOBAL_OFFSET_TABLE_
    955: 0000000000062778    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.32.llvm.1386185271139027476
    956: 00000000000151b0    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h14f5c75e7468b391E
@@ -1072,316 +1072,316 @@
    963: 0000000000012a40   281 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types3any5PyAny7setattr17h6b838b67a3f86361E
    964: 000000000000b600     9 FUNC    LOCAL  DEFAULT   11 _ZN3std7process5abort17h6a5731f81d82fd63E
    965: 0000000000047030   111 FUNC    LOCAL  DEFAULT   11 _ZN5alloc4sync32arcinner_layout_for_value_layout17h29ebdaf835957654E
    966: 000000000002e360    10 FUNC    LOCAL  DEFAULT   11 _ZN3std4time7Instant3now17h7b1369cc9fc453d9E
    967: 0000000000062c80    32 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.1.llvm.17695762341781453012
    968: 0000000000031850   133 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix17decode_error_kind17h2ad02d7078e49c10E
    969: 0000000000014650     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.17695762341781453012
-   970: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Display$GT$3fmt17h815d9d40959003edE
-   971: 0000000000062928    24 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.41.llvm.13238893432200692226
-   972: 00000000000116f0   197 FUNC    LOCAL  DEFAULT   11 _ZN53_$LT$T$u20$as$u20$pyo3..conversion..FromPyPointer$GT$21from_owned_ptr_or_opt17h947fb03ed62b14c7E.llvm.13238893432200692226
-   973: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRuntimeError$u20$as$u20$core..fmt..Display$GT$3fmt17h3b25ff331a9ad273E
-   974: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr76drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..string..PyString$GT$$GT$17hc3397687b30d1933E.llvm.11213889763605633493
-   975: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h02adaaea9cb2e646E
-   976: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u64$GT$3fmt17h09bd8bccf6418030E
-   977: 0000000000013d10   280 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types4list6PyList6append17h3af2694347be39efE
-   978: 000000000002d200  1013 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$std..path..Components$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17hd1f25fa4055526a5E
-   979: 000000000004efd8    45 OBJECT  LOCAL  DEFAULT   13 anon.69b6d96c8c65d794933159d5fb91439b.13.llvm.5680637462275538762
-   980: 0000000000009190   195 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription34missing_required_keyword_arguments17h9aac826a7df794c1E
-   981: 000000000000c110    83 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking14panic_nounwind17h3eb3a96bee9ee242E
-   982: 000000000002f1b0   274 FUNC    LOCAL  DEFAULT   11 __rust_drop_panic
-   983: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyNotImplementedError$u20$as$u20$core..fmt..Display$GT$3fmt17h6952e68ef879fadeE
-   984: 00000000000088c0   513 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription28multiple_values_for_argument17h1dd080a7cd5dc901E
-   985: 00000000000149c0   360 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule12add_function17hca8cf95fba3acaaeE
-   986: 000000000002d600  1503 FUNC    LOCAL  DEFAULT   11 _ZN95_$LT$std..path..Components$u20$as$u20$core..iter..traits..double_ended..DoubleEndedIterator$GT$9next_back17h08e4e96198d29623E
-   987: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyFileExistsError$u20$as$u20$core..fmt..Display$GT$3fmt17h2058f3d8f0e56f7eE
-   988: 0000000000030d70    41 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..path..StripPrefixError$u20$as$u20$core..fmt..Debug$GT$3fmt17h2e6413e98311718aE
-   989: 0000000000010130     4 FUNC    LOCAL  DEFAULT   11 _ZN120_$LT$pyo3..derive_utils..PyFunctionArguments$u20$as$u20$core..convert..From$LT$$RF$pyo3..types..module..PyModule$GT$$GT$4from17h0d1556cea2dcb696E
-   990: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyStopIteration$u20$as$u20$core..fmt..Debug$GT$3fmt17h55517876a481dea8E
-   991: 0000000000012ee0    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr111drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$alloc..string..String$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h3e9ad9d81ba2a877E.llvm.3160907281880781123
-   992: 000000000003ada0  5799 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev13Abbreviations6insert17h0a7293f5e55b3558E
-   993: 00000000000476c0     5 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo7message17h6cf5e87cd4ad4566E
-   994: 00000000000489b0  1064 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter3pad17he501b3d97feedd0fE
-   995: 0000000000012620   428 FUNC    LOCAL  DEFAULT   11 _ZN98_$LT$alloc..vec..Vec$LT$T$GT$$u20$as$u20$alloc..vec..spec_from_iter..SpecFromIter$LT$T$C$I$GT$$GT$9from_iter17hb664a7b7ebeb4d33E
-   996: 00000000000167a0    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h982eb6fb56ea8f96E.llvm.8364735172703476354
-   997: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$pyo3..exceptions..PyUnicodeTranslateError$u20$as$u20$core..fmt..Display$GT$3fmt17h107576381c9a1ccbE
-   998: 00000000000629e8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.41.llvm.3160907281880781123
-   999: 00000000000131a0   506 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err9err_state10PyErrState14into_ffi_tuple17h51d5d2e4ee753b56E
-  1000: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PySystemExit$u20$as$u20$core..fmt..Debug$GT$3fmt17h751a72fe3fa92c8aE
-  1001: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyArithmeticError$u20$as$u20$core..fmt..Display$GT$3fmt17hb38076bab35c024dE
-  1002: 000000000004c590    25 FUNC    LOCAL  DEFAULT   11 _ZN53_$LT$core..fmt..Error$u20$as$u20$core..fmt..Debug$GT$3fmt17hbf60e3f16b8e25e4E
-  1003: 000000000004c800   212 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$core..str..error..Utf8Error$u20$as$u20$core..fmt..Debug$GT$3fmt17h74aebf1ba331fe20E
-  1004: 00000000000142c0   385 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_9pymethods16extract_c_string17hd5d5fe3271ff1278E.llvm.5697929769133057476
-  1005: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyRuntimeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hf21d98e821bd5384E
-  1006: 000000000004b810   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i8$GT$3fmt17h6f0a522d3321db48E
-  1007: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..types..string..PyString$u20$as$u20$core..fmt..Debug$GT$3fmt17hea24af77f9e3a331E
-  1008: 0000000000066080    64 OBJECT  LOCAL  DEFAULT   24 _ZN4pyo33gil4POOL17h792de0d5abfbfeb7E
-  1009: 000000000004e8bd    14 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.52.llvm.13238893432200692226
-  1010: 000000000000fa00     5 FUNC    LOCAL  DEFAULT   11 __rust_dealloc
-  1011: 00000000000629c8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.39.llvm.3160907281880781123
-  1012: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..asyncio..InvalidStateError$u20$as$u20$core..fmt..Debug$GT$3fmt17h45c8f4facbb25e82E
-  1013: 00000000000629a8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.38.llvm.3160907281880781123
-  1014: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyException$u20$as$u20$core..fmt..Debug$GT$3fmt17h9b983c8017092f90E
-  1015: 000000000004e815    57 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.34.llvm.13238893432200692226
-  1016: 0000000000013d00     5 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types4list6PyList3len17h6f9dc6ce5488f412E
-  1017: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr125drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..dec2flt..ParseFloatError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h8e229d8e79308b03E.llvm.3160907281880781123
-  1018: 0000000000049000    60 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter11debug_tuple17h479b46e3552ae8c2E
-  1019: 000000000002a630    44 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$std..thread..local..AccessError$u20$as$u20$core..fmt..Debug$GT$3fmt17h3f59ec85644441edE
-  1020: 0000000000062908     8 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.37.llvm.13238893432200692226
-  1021: 0000000000011450     4 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr132drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$$GT$17h73f0eec5bca59ab3E.llvm.13238893432200692226
-  1022: 0000000000047630   128 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$core..panic..location..Location$u20$as$u20$core..fmt..Display$GT$3fmt17hfca18365adb444bcE
-  1023: 000000000000a5d0    28 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking11begin_panic17hcda3e28c4583f520E
-  1024: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyConnectionError$u20$as$u20$core..fmt..Display$GT$3fmt17h50b18681df69e02cE
-  1025: 000000000004e4d0    41 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.12.llvm.1386185271139027476
-  1026: 000000000004ade0   431 FUNC    LOCAL  DEFAULT   11 _ZN87_$LT$core..str..lossy..Utf8Chunks$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h88951ccd5ff0d88bE
-  1027: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyFloatingPointError$u20$as$u20$core..fmt..Display$GT$3fmt17h32c828dd92120ab3E
-  1028: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyOSError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd7e54f17b4011597E
-  1029: 000000000000fa20     5 FUNC    LOCAL  DEFAULT   11 __rust_alloc_zeroed
-  1030: 0000000000011670    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17h839b07d28c50dd15E.llvm.13238893432200692226
-  1031: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyAssertionError$u20$as$u20$core..fmt..Display$GT$3fmt17he05af6d1d6d66205E
-  1032: 0000000000048e60    47 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter12debug_struct17hf8dd668954fee432E
-  1033: 0000000000062eb0    24 OBJECT  LOCAL  DEFAULT   21 anon.e9136d4cc2f2bf733d592b5df8895207.5.llvm.17368754240468033560
-  1034: 000000000004ebe0    55 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.1.llvm.5697929769133057476
-  1035: 00000000000157c0   285 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$10write_char17h9723cd5765c4528dE.llvm.3041393958569974349
-  1036: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyIndexError$u20$as$u20$core..fmt..Display$GT$3fmt17h6cf9ab5498ea1509E
-  1037: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyEnvironmentError$u20$as$u20$core..fmt..Display$GT$3fmt17hcd4b69b1ee65f35fE
-  1038: 000000000004e7e8    45 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.32.llvm.13238893432200692226
-  1039: 000000000004e43e    89 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.33.llvm.18356750485614513129
-  1040: 0000000000009d30  1516 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot9raw_mutex8RawMutex9lock_slow17h0838ebc822ea02ffE
-  1041: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PySystemExit$u20$as$u20$core..fmt..Display$GT$3fmt17hdf0cb1c06b14d905E
-  1042: 0000000000011380   116 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hcde0b0035e6c8beeE.llvm.13238893432200692226
-  1043: 0000000000008090    77 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking13assert_failed17hf9a7474ff41f383eE
-  1044: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyUnicodeWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h8190e660a78b1a02E
-  1045: 000000000003a850   404 FUNC    LOCAL  DEFAULT   11 _ZN9addr2line9path_push17h2bdcb858d0f1ded9E
-  1046: 00000000000491e0    53 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter10debug_list17h9f2f28a9732ff378E
-  1047: 0000000000049100   211 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter25debug_tuple_field2_finish17h59c8a53dbdec2c27E
-  1048: 000000000004ec62    38 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.40.llvm.5697929769133057476
-  1049: 0000000000013f60     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.5697929769133057476
-  1050: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr108drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$LP$$RF$str$C$$RP$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17haa592fa5f669780dE.llvm.3160907281880781123
-  1051: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PySyntaxWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h381ade6111a6a996E
-  1052: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyAttributeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h65ccfa4cd7c9fabcE
-  1053: 0000000000031510    89 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$14write_vectored17h2791574c005661ffE
-  1054: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyLookupError$u20$as$u20$core..fmt..Debug$GT$3fmt17h81c37bf3b6d71051E
-  1055: 000000000002e1d0   183 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path7is_file17ha0f027b6f277668eE
-  1056: 000000000002b8c0   471 FUNC    LOCAL  DEFAULT   11 _ZN61_$LT$$RF$std..io..stdio..Stderr$u20$as$u20$std..io..Write$GT$9write_fmt17h53f17b64a12fa9dbE
-  1057: 000000000002fdd0   847 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking20rust_panic_with_hook17h50c09d000dc561d2E
-  1058: 000000000004c460   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$u64$GT$3fmt17hab738be73c7b7c86E
-  1059: 0000000000048270    11 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt10ArgumentV110from_usize17haeae83e6830161a1E
-  1060: 0000000000015780    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr205drop_in_place$LT$$LT$alloc..boxed..Box$LT$dyn$u20$core..error..Error$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$u20$as$u20$core..convert..From$LT$alloc..string..String$GT$$GT$..from..StringError$GT$17h44f3a8148351d138E.llvm.3041393958569974349
-  1061: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyUnicodeEncodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha130df985b5b4cdfE
-  1062: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyResourceWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hf42f32192b6bd4b9E
-  1063: 00000000000173c0   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h96843a80e7150ce9E
-  1064: 000000000004cc20    16 FUNC    LOCAL  DEFAULT   11 stat64
-  1065: 0000000000015670   190 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h8c9b1f14eb798a0aE
-  1066: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyUnicodeDecodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd42b8d22e8d91706E
-  1067: 0000000000048df0    56 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9write_fmt17ha4a884db254a61f9E
-  1068: 0000000000062790    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.33.llvm.1386185271139027476
-  1069: 000000000004b740   201 FUNC    LOCAL  DEFAULT   11 _ZN4core3num60_$LT$impl$u20$core..str..traits..FromStr$u20$for$u20$u64$GT$8from_str17h7aaa71d617ee7089E
-  1070: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr126drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..char..decode..DecodeUtf16Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h4b1d717590cb3f2fE.llvm.3160907281880781123
-  1071: 000000000004b8a0   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u8$GT$3fmt17h8bbaafe3384c2aa7E
-  1072: 00000000000157a0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.3041393958569974349
-  1073: 00000000000628b0    32 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.14.llvm.13238893432200692226
-  1074: 0000000000014ba0   411 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_8pymodule9ModuleDef11make_module17h79f24fd75a6e2c7cE
-  1075: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyIOError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha999be169e099575E
-  1076: 0000000000048de0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9write_str17h81686a833f68fc53E
-  1077: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyProcessLookupError$u20$as$u20$core..fmt..Display$GT$3fmt17h9f6b81ff388d44f7E
-  1078: 0000000000062c18    48 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.0.llvm.5697929769133057476
-  1079: 0000000000013e70   141 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple125_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$$RP$$GT$7into_py17hd6ed6ec0316f8814E
-  1080: 00000000000155a0   205 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h5fcb0d20fb31f478E
-  1081: 00000000000661a0     8 OBJECT  LOCAL  DEFAULT   25 _ZN3std9panicking11panic_count18GLOBAL_PANIC_COUNT17h491d820ed8318ec5E
-  1082: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyNameError$u20$as$u20$core..fmt..Debug$GT$3fmt17hfda1ef1177479b61E
-  1083: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$usize$GT$3fmt17hb7342dd1750dc887E
-  1084: 0000000000013d00     5 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple3len17hce77ad4c4d8ec47cE
-  1085: 0000000000062c48    24 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.3.llvm.5697929769133057476
-  1086: 0000000000013120    31 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$alloc..borrow..Cow$LT$str$GT$$GT$17hb21c8154e58f0fc6E.llvm.3160907281880781123
-  1087: 000000000002ad90   748 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5error83_$LT$impl$u20$core..fmt..Debug$u20$for$u20$std..io..error..repr_bitpacked..Repr$GT$3fmt17hdeb28f00b46858f9E
-  1088: 000000000002f2d0   274 FUNC    LOCAL  DEFAULT   11 __rust_foreign_exception
-  1089: 000000000000a850    98 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot16create_hashtable17h2c1aa79f3500842aE
-  1090: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyChildProcessError$u20$as$u20$core..fmt..Display$GT$3fmt17h37d6918dacb27ef5E
-  1091: 0000000000016de0     8 FUNC    LOCAL  DEFAULT   11 _ZN3std10sys_common9backtrace26__rust_end_short_backtrace17h9913f8d08b925a3eE
-  1092: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyKeyError$u20$as$u20$core..fmt..Display$GT$3fmt17h2001991bbfa92233E
-  1093: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyKeyboardInterrupt$u20$as$u20$core..fmt..Display$GT$3fmt17hf1cc357e67b65b8cE
-  1094: 000000000004ebad     6 OBJECT  LOCAL  DEFAULT   13 anon.a80902d6bb08773bf6743d023c7df73e.13.llvm.11940621367560662805
-  1095: 00000000000158e0    66 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$9write_fmt17h546d7a043fb85e03E.llvm.3041393958569974349
-  1096: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyConnectionResetError$u20$as$u20$core..fmt..Debug$GT$3fmt17h841dbdc13b028073E
-  1097: 00000000000476f0   350 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$core..panic..panic_info..PanicInfo$u20$as$u20$core..fmt..Display$GT$3fmt17h8e1128b839149545E
-  1098: 0000000000049660    18 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$str$u20$as$u20$core..fmt..Display$GT$3fmt17hcb04acc5244d35e3E
-  1099: 00000000000660c0    24 OBJECT  LOCAL  DEFAULT   24 _ZN4pyo35types10typeobject6PyType4name8INTERNED17hde3230b9e5fe337cE.llvm.14631431423107687823
-  1100: 0000000000062610    32 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.20.llvm.18356750485614513129
-  1101: 000000000003ad60    60 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev13Abbreviations5empty17h83512422d3c40434E
-  1102: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyReferenceError$u20$as$u20$core..fmt..Display$GT$3fmt17h6b3bd7d5f6ca7810E
-  1103: 0000000000049e30   516 FUNC    LOCAL  DEFAULT   11 _ZN4core3str8converts9from_utf817h96fe04f4c6d3f1eaE
-  1104: 0000000000015930    97 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$9write_str17hc17d7e9625b7dffaE.llvm.3041393958569974349
-  1105: 000000000004b8a0   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i8$GT$3fmt17h9510492da5a7f5f6E
-  1106: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyNotADirectoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17h11320b40b202271aE
-  1107: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyProcessLookupError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8906a46ef7b143c1E
-  1108: 000000000000fe90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.18356750485614513129
-  1109: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h025aee14bd815f41E
-  1110: 00000000000626a0    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.32.llvm.18356750485614513129
-  1111: 0000000000011690    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.13238893432200692226
-  1112: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN84_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h43f6de0dfbfa8d59E
-  1113: 000000000003c690    65 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$gimli..read..abbrev..Attributes$u20$as$u20$core..ops..deref..Deref$GT$5deref17h0e97780763d5016bE
-  1114: 00000000000466e0   355 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17hccb117dae17ea40eE
-  1115: 0000000000043140    75 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core17DecompressorOxide3new17hd62a62e63e49204eE
-  1116: 000000000000f920   194 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple137_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$C$T2$C$T3$RP$$GT$7into_py17hfbeb287d953cc89bE
+   970: 000000000000f890   142 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple127_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$RP$$GT$7into_py17h38128205453875a5E
+   971: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Display$GT$3fmt17h815d9d40959003edE
+   972: 0000000000062928    24 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.41.llvm.13238893432200692226
+   973: 00000000000116f0   197 FUNC    LOCAL  DEFAULT   11 _ZN53_$LT$T$u20$as$u20$pyo3..conversion..FromPyPointer$GT$21from_owned_ptr_or_opt17h947fb03ed62b14c7E.llvm.13238893432200692226
+   974: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyRuntimeError$u20$as$u20$core..fmt..Display$GT$3fmt17h3b25ff331a9ad273E
+   975: 0000000000012420     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr76drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..string..PyString$GT$$GT$17hc3397687b30d1933E.llvm.11213889763605633493
+   976: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h02adaaea9cb2e646E
+   977: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u64$GT$3fmt17h09bd8bccf6418030E
+   978: 0000000000013d10   280 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types4list6PyList6append17h3af2694347be39efE
+   979: 000000000002d200  1013 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$std..path..Components$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17hd1f25fa4055526a5E
+   980: 000000000004efd8    45 OBJECT  LOCAL  DEFAULT   13 anon.69b6d96c8c65d794933159d5fb91439b.13.llvm.5680637462275538762
+   981: 0000000000009190   195 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription34missing_required_keyword_arguments17h9aac826a7df794c1E
+   982: 000000000000c110    83 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking14panic_nounwind17h3eb3a96bee9ee242E
+   983: 000000000002f1b0   274 FUNC    LOCAL  DEFAULT   11 __rust_drop_panic
+   984: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyNotImplementedError$u20$as$u20$core..fmt..Display$GT$3fmt17h6952e68ef879fadeE
+   985: 00000000000088c0   513 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription28multiple_values_for_argument17h1dd080a7cd5dc901E
+   986: 00000000000149c0   360 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule12add_function17hca8cf95fba3acaaeE
+   987: 000000000002d600  1503 FUNC    LOCAL  DEFAULT   11 _ZN95_$LT$std..path..Components$u20$as$u20$core..iter..traits..double_ended..DoubleEndedIterator$GT$9next_back17h08e4e96198d29623E
+   988: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyFileExistsError$u20$as$u20$core..fmt..Display$GT$3fmt17h2058f3d8f0e56f7eE
+   989: 0000000000030d70    41 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..path..StripPrefixError$u20$as$u20$core..fmt..Debug$GT$3fmt17h2e6413e98311718aE
+   990: 0000000000010130     4 FUNC    LOCAL  DEFAULT   11 _ZN120_$LT$pyo3..derive_utils..PyFunctionArguments$u20$as$u20$core..convert..From$LT$$RF$pyo3..types..module..PyModule$GT$$GT$4from17h0d1556cea2dcb696E
+   991: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyStopIteration$u20$as$u20$core..fmt..Debug$GT$3fmt17h55517876a481dea8E
+   992: 0000000000012ee0    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr111drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$alloc..string..String$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h3e9ad9d81ba2a877E.llvm.3160907281880781123
+   993: 000000000003ada0  5799 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev13Abbreviations6insert17h0a7293f5e55b3558E
+   994: 00000000000476c0     5 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo7message17h6cf5e87cd4ad4566E
+   995: 00000000000489b0  1064 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter3pad17he501b3d97feedd0fE
+   996: 0000000000012620   428 FUNC    LOCAL  DEFAULT   11 _ZN98_$LT$alloc..vec..Vec$LT$T$GT$$u20$as$u20$alloc..vec..spec_from_iter..SpecFromIter$LT$T$C$I$GT$$GT$9from_iter17hb664a7b7ebeb4d33E
+   997: 00000000000167a0    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h982eb6fb56ea8f96E.llvm.8364735172703476354
+   998: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN80_$LT$pyo3..exceptions..PyUnicodeTranslateError$u20$as$u20$core..fmt..Display$GT$3fmt17h107576381c9a1ccbE
+   999: 00000000000629e8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.41.llvm.3160907281880781123
+  1000: 00000000000131a0   506 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err9err_state10PyErrState14into_ffi_tuple17h51d5d2e4ee753b56E
+  1001: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PySystemExit$u20$as$u20$core..fmt..Debug$GT$3fmt17h751a72fe3fa92c8aE
+  1002: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyArithmeticError$u20$as$u20$core..fmt..Display$GT$3fmt17hb38076bab35c024dE
+  1003: 000000000004c590    25 FUNC    LOCAL  DEFAULT   11 _ZN53_$LT$core..fmt..Error$u20$as$u20$core..fmt..Debug$GT$3fmt17hbf60e3f16b8e25e4E
+  1004: 000000000004c800   212 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$core..str..error..Utf8Error$u20$as$u20$core..fmt..Debug$GT$3fmt17h74aebf1ba331fe20E
+  1005: 00000000000142c0   385 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_9pymethods16extract_c_string17hd5d5fe3271ff1278E.llvm.5697929769133057476
+  1006: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyRuntimeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hf21d98e821bd5384E
+  1007: 000000000004b810   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i8$GT$3fmt17h6f0a522d3321db48E
+  1008: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..types..string..PyString$u20$as$u20$core..fmt..Debug$GT$3fmt17hea24af77f9e3a331E
+  1009: 0000000000066080    64 OBJECT  LOCAL  DEFAULT   24 _ZN4pyo33gil4POOL17h792de0d5abfbfeb7E
+  1010: 000000000004e8bd    14 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.52.llvm.13238893432200692226
+  1011: 000000000000fa00     5 FUNC    LOCAL  DEFAULT   11 __rust_dealloc
+  1012: 00000000000629c8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.39.llvm.3160907281880781123
+  1013: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..asyncio..InvalidStateError$u20$as$u20$core..fmt..Debug$GT$3fmt17h45c8f4facbb25e82E
+  1014: 00000000000629a8    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.38.llvm.3160907281880781123
+  1015: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyException$u20$as$u20$core..fmt..Debug$GT$3fmt17h9b983c8017092f90E
+  1016: 000000000004e815    57 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.34.llvm.13238893432200692226
+  1017: 0000000000013d00     5 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types4list6PyList3len17h6f9dc6ce5488f412E
+  1018: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr125drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..dec2flt..ParseFloatError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h8e229d8e79308b03E.llvm.3160907281880781123
+  1019: 0000000000049000    60 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter11debug_tuple17h479b46e3552ae8c2E
+  1020: 000000000002a630    44 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$std..thread..local..AccessError$u20$as$u20$core..fmt..Debug$GT$3fmt17h3f59ec85644441edE
+  1021: 0000000000062908     8 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.37.llvm.13238893432200692226
+  1022: 0000000000011450     4 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr132drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$$GT$17h73f0eec5bca59ab3E.llvm.13238893432200692226
+  1023: 0000000000047630   128 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$core..panic..location..Location$u20$as$u20$core..fmt..Display$GT$3fmt17hfca18365adb444bcE
+  1024: 000000000000a5d0    28 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking11begin_panic17hcda3e28c4583f520E
+  1025: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyConnectionError$u20$as$u20$core..fmt..Display$GT$3fmt17h50b18681df69e02cE
+  1026: 000000000004e4d0    41 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.12.llvm.1386185271139027476
+  1027: 000000000004ade0   431 FUNC    LOCAL  DEFAULT   11 _ZN87_$LT$core..str..lossy..Utf8Chunks$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h88951ccd5ff0d88bE
+  1028: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyFloatingPointError$u20$as$u20$core..fmt..Display$GT$3fmt17h32c828dd92120ab3E
+  1029: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyOSError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd7e54f17b4011597E
+  1030: 000000000000fa20     5 FUNC    LOCAL  DEFAULT   11 __rust_alloc_zeroed
+  1031: 0000000000011670    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17h839b07d28c50dd15E.llvm.13238893432200692226
+  1032: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyAssertionError$u20$as$u20$core..fmt..Display$GT$3fmt17he05af6d1d6d66205E
+  1033: 0000000000048e60    47 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter12debug_struct17hf8dd668954fee432E
+  1034: 0000000000062eb0    24 OBJECT  LOCAL  DEFAULT   21 anon.e9136d4cc2f2bf733d592b5df8895207.5.llvm.17368754240468033560
+  1035: 000000000004ebe0    55 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.1.llvm.5697929769133057476
+  1036: 00000000000157c0   285 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$10write_char17h9723cd5765c4528dE.llvm.3041393958569974349
+  1037: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyIndexError$u20$as$u20$core..fmt..Display$GT$3fmt17h6cf9ab5498ea1509E
+  1038: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyEnvironmentError$u20$as$u20$core..fmt..Display$GT$3fmt17hcd4b69b1ee65f35fE
+  1039: 000000000004e7e8    45 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.32.llvm.13238893432200692226
+  1040: 000000000004e43e    89 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.33.llvm.18356750485614513129
+  1041: 0000000000009d30  1516 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot9raw_mutex8RawMutex9lock_slow17h0838ebc822ea02ffE
+  1042: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PySystemExit$u20$as$u20$core..fmt..Display$GT$3fmt17hdf0cb1c06b14d905E
+  1043: 0000000000011380   116 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hcde0b0035e6c8beeE.llvm.13238893432200692226
+  1044: 0000000000008090    77 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking13assert_failed17hf9a7474ff41f383eE
+  1045: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyUnicodeWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h8190e660a78b1a02E
+  1046: 000000000003a850   404 FUNC    LOCAL  DEFAULT   11 _ZN9addr2line9path_push17h2bdcb858d0f1ded9E
+  1047: 00000000000491e0    53 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter10debug_list17h9f2f28a9732ff378E
+  1048: 0000000000049100   211 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter25debug_tuple_field2_finish17h59c8a53dbdec2c27E
+  1049: 000000000004ec62    38 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.40.llvm.5697929769133057476
+  1050: 0000000000013f60     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.5697929769133057476
+  1051: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr108drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$LP$$RF$str$C$$RP$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17haa592fa5f669780dE.llvm.3160907281880781123
+  1052: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PySyntaxWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h381ade6111a6a996E
+  1053: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyAttributeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h65ccfa4cd7c9fabcE
+  1054: 0000000000031510    89 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$14write_vectored17h2791574c005661ffE
+  1055: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyLookupError$u20$as$u20$core..fmt..Debug$GT$3fmt17h81c37bf3b6d71051E
+  1056: 000000000002e1d0   183 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path7is_file17ha0f027b6f277668eE
+  1057: 000000000002b8c0   471 FUNC    LOCAL  DEFAULT   11 _ZN61_$LT$$RF$std..io..stdio..Stderr$u20$as$u20$std..io..Write$GT$9write_fmt17h53f17b64a12fa9dbE
+  1058: 000000000002fdd0   847 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking20rust_panic_with_hook17h50c09d000dc561d2E
+  1059: 000000000004c460   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$u64$GT$3fmt17hab738be73c7b7c86E
+  1060: 0000000000048270    11 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt10ArgumentV110from_usize17haeae83e6830161a1E
+  1061: 0000000000015780    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr205drop_in_place$LT$$LT$alloc..boxed..Box$LT$dyn$u20$core..error..Error$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$u20$as$u20$core..convert..From$LT$alloc..string..String$GT$$GT$..from..StringError$GT$17h44f3a8148351d138E.llvm.3041393958569974349
+  1062: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyUnicodeEncodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha130df985b5b4cdfE
+  1063: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyResourceWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hf42f32192b6bd4b9E
+  1064: 00000000000173c0   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h96843a80e7150ce9E
+  1065: 000000000004cc20    16 FUNC    LOCAL  DEFAULT   11 stat64
+  1066: 0000000000015670   190 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h8c9b1f14eb798a0aE
+  1067: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyUnicodeDecodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hd42b8d22e8d91706E
+  1068: 0000000000048df0    56 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9write_fmt17ha4a884db254a61f9E
+  1069: 0000000000062790    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.33.llvm.1386185271139027476
+  1070: 000000000004b740   201 FUNC    LOCAL  DEFAULT   11 _ZN4core3num60_$LT$impl$u20$core..str..traits..FromStr$u20$for$u20$u64$GT$8from_str17h7aaa71d617ee7089E
+  1071: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr126drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..char..decode..DecodeUtf16Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h4b1d717590cb3f2fE.llvm.3160907281880781123
+  1072: 000000000004b8a0   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u8$GT$3fmt17h8bbaafe3384c2aa7E
+  1073: 00000000000157a0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.3041393958569974349
+  1074: 00000000000628b0    32 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.14.llvm.13238893432200692226
+  1075: 0000000000014ba0   411 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_8pymodule9ModuleDef11make_module17h79f24fd75a6e2c7cE
+  1076: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyIOError$u20$as$u20$core..fmt..Debug$GT$3fmt17ha999be169e099575E
+  1077: 0000000000048de0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter9write_str17h81686a833f68fc53E
+  1078: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyProcessLookupError$u20$as$u20$core..fmt..Display$GT$3fmt17h9f6b81ff388d44f7E
+  1079: 0000000000062c18    48 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.0.llvm.5697929769133057476
+  1080: 0000000000013e70   141 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple125_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$$RP$$GT$7into_py17hd6ed6ec0316f8814E
+  1081: 00000000000155a0   205 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h5fcb0d20fb31f478E
+  1082: 00000000000661a0     8 OBJECT  LOCAL  DEFAULT   25 _ZN3std9panicking11panic_count18GLOBAL_PANIC_COUNT17h491d820ed8318ec5E
+  1083: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyNameError$u20$as$u20$core..fmt..Debug$GT$3fmt17hfda1ef1177479b61E
+  1084: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$usize$GT$3fmt17hb7342dd1750dc887E
+  1085: 0000000000013d00     5 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple3len17hce77ad4c4d8ec47cE
+  1086: 0000000000062c48    24 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.3.llvm.5697929769133057476
+  1087: 0000000000013120    31 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$alloc..borrow..Cow$LT$str$GT$$GT$17hb21c8154e58f0fc6E.llvm.3160907281880781123
+  1088: 000000000002ad90   748 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5error83_$LT$impl$u20$core..fmt..Debug$u20$for$u20$std..io..error..repr_bitpacked..Repr$GT$3fmt17hdeb28f00b46858f9E
+  1089: 000000000002f2d0   274 FUNC    LOCAL  DEFAULT   11 __rust_foreign_exception
+  1090: 000000000000a850    98 FUNC    LOCAL  DEFAULT   11 _ZN16parking_lot_core11parking_lot16create_hashtable17h2c1aa79f3500842aE
+  1091: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyChildProcessError$u20$as$u20$core..fmt..Display$GT$3fmt17h37d6918dacb27ef5E
+  1092: 0000000000016de0     8 FUNC    LOCAL  DEFAULT   11 _ZN3std10sys_common9backtrace26__rust_end_short_backtrace17h9913f8d08b925a3eE
+  1093: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyKeyError$u20$as$u20$core..fmt..Display$GT$3fmt17h2001991bbfa92233E
+  1094: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyKeyboardInterrupt$u20$as$u20$core..fmt..Display$GT$3fmt17hf1cc357e67b65b8cE
+  1095: 000000000004ebad     6 OBJECT  LOCAL  DEFAULT   13 anon.a80902d6bb08773bf6743d023c7df73e.13.llvm.11940621367560662805
+  1096: 00000000000158e0    66 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$9write_fmt17h546d7a043fb85e03E.llvm.3041393958569974349
+  1097: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyConnectionResetError$u20$as$u20$core..fmt..Debug$GT$3fmt17h841dbdc13b028073E
+  1098: 00000000000476f0   350 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$core..panic..panic_info..PanicInfo$u20$as$u20$core..fmt..Display$GT$3fmt17h8e1128b839149545E
+  1099: 0000000000049660    18 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$str$u20$as$u20$core..fmt..Display$GT$3fmt17hcb04acc5244d35e3E
+  1100: 00000000000660c0    24 OBJECT  LOCAL  DEFAULT   24 _ZN4pyo35types10typeobject6PyType4name8INTERNED17hde3230b9e5fe337cE.llvm.14631431423107687823
+  1101: 0000000000062610    32 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.20.llvm.18356750485614513129
+  1102: 000000000003ad60    60 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev13Abbreviations5empty17h83512422d3c40434E
+  1103: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyReferenceError$u20$as$u20$core..fmt..Display$GT$3fmt17h6b3bd7d5f6ca7810E
+  1104: 0000000000049e30   516 FUNC    LOCAL  DEFAULT   11 _ZN4core3str8converts9from_utf817h96fe04f4c6d3f1eaE
+  1105: 0000000000015930    97 FUNC    LOCAL  DEFAULT   11 _ZN50_$LT$$RF$mut$u20$W$u20$as$u20$core..fmt..Write$GT$9write_str17hc17d7e9625b7dffaE.llvm.3041393958569974349
+  1106: 000000000004b8a0   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i8$GT$3fmt17h9510492da5a7f5f6E
+  1107: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyNotADirectoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17h11320b40b202271aE
+  1108: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyProcessLookupError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8906a46ef7b143c1E
+  1109: 000000000000fe90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.18356750485614513129
+  1110: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h025aee14bd815f41E
+  1111: 00000000000626a0    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.32.llvm.18356750485614513129
+  1112: 0000000000011690    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.13238893432200692226
+  1113: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN84_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h43f6de0dfbfa8d59E
+  1114: 000000000003c690    65 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$gimli..read..abbrev..Attributes$u20$as$u20$core..ops..deref..Deref$GT$5deref17h0e97780763d5016bE
+  1115: 00000000000466e0   355 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17hccb117dae17ea40eE
+  1116: 0000000000043140    75 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core17DecompressorOxide3new17hd62a62e63e49204eE
   1117: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyIOError$u20$as$u20$core..fmt..Display$GT$3fmt17h4684b863c7405c24E
   1118: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hc5aab802369a5be8E
   1119: 00000000000127d0   256 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types3any5PyAny7getattr17hcd851db43e568513E
   1120: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h2f8c1ae13caabb10E.llvm.3160907281880781123
   1121: 0000000000011430    28 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr122drop_in_place$LT$alloc..vec..into_iter..IntoIter$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$17h354e65b2c3462211E.llvm.13238893432200692226
   1122: 000000000002fa50   116 FUNC    LOCAL  DEFAULT   11 rust_begin_unwind
   1123: 0000000000062968    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.25.llvm.3160907281880781123
   1124: 00000000000114f0   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.13238893432200692226
   1125: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyInterruptedError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb72a022a7a6bd2a9E
   1126: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyBrokenPipeError$u20$as$u20$core..fmt..Display$GT$3fmt17h52e34d65bb49743aE
-  1127: 000000000000ea10    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h51bea979b21a7957E
-  1128: 00000000000313a0   271 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$std..sys..unix..os_str..Slice$u20$as$u20$core..fmt..Display$GT$3fmt17h7e6fdf932a7c0d65E
-  1129: 000000000000fca0     4 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr132drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$$GT$17h73f0eec5bca59ab3E.llvm.18356750485614513129
-  1130: 0000000000046600    75 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec17capacity_overflow17h564475d43ac0e37cE
-  1131: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyOSError$u20$as$u20$core..fmt..Display$GT$3fmt17hedaa715cc53c30a3E
-  1132: 000000000000bbe0   369 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks12futex_rwlock6RwLock14read_contended17h8d2d4f25fa7e2cffE
-  1133: 000000000004c160   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp51_$LT$impl$u20$core..fmt..Display$u20$for$u20$u8$GT$3fmt17he4918c78216b8995E
-  1134: 00000000000474b0   174 FUNC    LOCAL  DEFAULT   11 _ZN82_$LT$core..char..EscapeDebug$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h0ce4c5bc56d4349fE
-  1135: 00000000000499d0   214 FUNC    LOCAL  DEFAULT   11 _ZN43_$LT$char$u20$as$u20$core..fmt..Display$GT$3fmt17h31c4c24bbd08aa24E
-  1136: 000000000004a870  1339 FUNC    LOCAL  DEFAULT   11 _ZN4core3str7pattern11StrSearcher3new17h6336710313a3bf5bE
-  1137: 00000000000627a8    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.34.llvm.1386185271139027476
-  1138: 0000000000043120    21 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$rustc_demangle..SizeLimitExhausted$u20$as$u20$core..fmt..Debug$GT$3fmt17h14a951538888cc74E
-  1139: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyModuleNotFoundError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb90fa2e458d54cd5E
-  1140: 0000000000014170   327 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_9pymethods11PyMethodDef13as_method_def17h624dbd2bc3a5ab3aE
-  1141: 0000000000066128     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
-  1142: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySyntaxWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hbaeea78fb76cb3faE
-  1143: 0000000000014100    95 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$alloc..string..String$u20$as$u20$core..fmt..Write$GT$9write_str17hcabd3fc9f749ae30E.llvm.5697929769133057476
-  1144: 0000000000012b60   320 FUNC    LOCAL  DEFAULT   11 _ZN62_$LT$pyo3..types..any..PyAny$u20$as$u20$core..fmt..Display$GT$3fmt17h01bfd7faf5add2eaE
-  1145: 000000000004e89f    24 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.38.llvm.13238893432200692226
-  1146: 0000000000015a10   409 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string82_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$alloc..string..String$GT$7extract17h08a07395a53ed098E
-  1147: 0000000000066140     8 OBJECT  LOCAL  DEFAULT   25 _ZN16parking_lot_core11parking_lot9HASHTABLE17h9fcd6b50658d7790E
-  1148: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyArithmeticError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8d583032932d3258E
-  1149: 0000000000049680   836 FUNC    LOCAL  DEFAULT   11 _ZN41_$LT$char$u20$as$u20$core..fmt..Debug$GT$3fmt17hacca1e08548532f1E
-  1150: 0000000000009330    28 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking11begin_panic17h7a3cef7c94e375b8E
-  1151: 0000000000047ab0   424 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders11DebugStruct5field17h34ac1bbc88a79ac3E
-  1152: 00000000000380c0     8 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..rust_panic_without_hook..RewrapBox$u20$as$u20$core..panic..BoxMeUp$GT$3get17hd95878c44be69298E
-  1153: 000000000000fa50     8 FUNC    LOCAL  DEFAULT   11 _ZN3std10sys_common9backtrace26__rust_end_short_backtrace17h5152e5383956f652E
+  1127: 00000000000313a0   271 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$std..sys..unix..os_str..Slice$u20$as$u20$core..fmt..Display$GT$3fmt17h7e6fdf932a7c0d65E
+  1128: 000000000000fca0     4 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr132drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$$GT$17h73f0eec5bca59ab3E.llvm.18356750485614513129
+  1129: 0000000000046600    75 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec17capacity_overflow17h564475d43ac0e37cE
+  1130: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$pyo3..exceptions..PyOSError$u20$as$u20$core..fmt..Display$GT$3fmt17hedaa715cc53c30a3E
+  1131: 000000000000bbe0   369 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks12futex_rwlock6RwLock14read_contended17h8d2d4f25fa7e2cffE
+  1132: 000000000004c160   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp51_$LT$impl$u20$core..fmt..Display$u20$for$u20$u8$GT$3fmt17he4918c78216b8995E
+  1133: 00000000000474b0   174 FUNC    LOCAL  DEFAULT   11 _ZN82_$LT$core..char..EscapeDebug$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h0ce4c5bc56d4349fE
+  1134: 00000000000499d0   214 FUNC    LOCAL  DEFAULT   11 _ZN43_$LT$char$u20$as$u20$core..fmt..Display$GT$3fmt17h31c4c24bbd08aa24E
+  1135: 000000000004a870  1339 FUNC    LOCAL  DEFAULT   11 _ZN4core3str7pattern11StrSearcher3new17h6336710313a3bf5bE
+  1136: 00000000000627a8    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.34.llvm.1386185271139027476
+  1137: 0000000000043120    21 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$rustc_demangle..SizeLimitExhausted$u20$as$u20$core..fmt..Debug$GT$3fmt17h14a951538888cc74E
+  1138: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyModuleNotFoundError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb90fa2e458d54cd5E
+  1139: 0000000000014170   327 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_9pymethods11PyMethodDef13as_method_def17h624dbd2bc3a5ab3aE
+  1140: 0000000000066128     0 OBJECT  LOCAL  DEFAULT   24 __TMC_END__
+  1141: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySyntaxWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hbaeea78fb76cb3faE
+  1142: 0000000000014100    95 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$alloc..string..String$u20$as$u20$core..fmt..Write$GT$9write_str17hcabd3fc9f749ae30E.llvm.5697929769133057476
+  1143: 0000000000012b60   320 FUNC    LOCAL  DEFAULT   11 _ZN62_$LT$pyo3..types..any..PyAny$u20$as$u20$core..fmt..Display$GT$3fmt17h01bfd7faf5add2eaE
+  1144: 000000000004e89f    24 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.38.llvm.13238893432200692226
+  1145: 0000000000015a10   409 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string82_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$alloc..string..String$GT$7extract17h08a07395a53ed098E
+  1146: 0000000000066140     8 OBJECT  LOCAL  DEFAULT   25 _ZN16parking_lot_core11parking_lot9HASHTABLE17h9fcd6b50658d7790E
+  1147: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyArithmeticError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8d583032932d3258E
+  1148: 0000000000049680   836 FUNC    LOCAL  DEFAULT   11 _ZN41_$LT$char$u20$as$u20$core..fmt..Debug$GT$3fmt17hacca1e08548532f1E
+  1149: 0000000000009330    28 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking11begin_panic17h7a3cef7c94e375b8E
+  1150: 0000000000047ab0   424 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders11DebugStruct5field17h34ac1bbc88a79ac3E
+  1151: 00000000000380c0     8 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..rust_panic_without_hook..RewrapBox$u20$as$u20$core..panic..BoxMeUp$GT$3get17hd95878c44be69298E
+  1152: 000000000000fa50     8 FUNC    LOCAL  DEFAULT   11 _ZN3std10sys_common9backtrace26__rust_end_short_backtrace17h5152e5383956f652E
+  1153: 000000000000f880     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h762d1cc7c3d79729E.llvm.11901482343555561327
   1154: 000000000004b810   141 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u8$GT$3fmt17h61de3dd80864a2dbE
   1155: 0000000000042220  3178 FUNC    LOCAL  DEFAULT   11 _ZN14rustc_demangle8demangle17h18329d8ff3695e33E
   1156: 0000000000031d90   884 FUNC    LOCAL  DEFAULT   11 rust_eh_personality
   1157: 0000000000061e00     0 OBJECT  LOCAL  DEFAULT   21 __dso_handle
   1158: 00000000000155a0   205 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h3e8cb9f4133f7766E
   1159: 0000000000013fb0    38 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr69drop_in_place$LT$alloc..borrow..Cow$LT$core..ffi..c_str..CStr$GT$$GT$17h34733ae39e06fd32E.llvm.5697929769133057476
   1160: 000000000004b930   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i32$GT$3fmt17h734818c8fc62ec6bE
   1161: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyBufferError$u20$as$u20$core..fmt..Display$GT$3fmt17hf8c0e41fd4749031E
   1162: 0000000000047fb0    37 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders9DebugList6finish17h8df4dd32d6774c16E
   1163: 0000000000012df0    33 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h149e760258b2c034E.llvm.3160907281880781123
-  1164: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb66f591c6d124ab0E
-  1165: 000000000002fce0    11 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$std..panicking..begin_panic_handler..StrPanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hc59bdcf586fef76cE
-  1166: 000000000004c330   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$u32$GT$3fmt17he422b8199910d448E
-  1167: 000000000003ad40    30 FUNC    LOCAL  DEFAULT   11 _ZN5gimli6common9SectionId4name17hb19ecacf465758f1E
-  1168: 0000000000031d40    32 FUNC    LOCAL  DEFAULT   11 _ZN3std5alloc8rust_oom17hbb2cf487567423f9E
-  1169: 0000000000031d60     9 FUNC    LOCAL  DEFAULT   11 __rg_oom
-  1170: 0000000000016860   569 FUNC    LOCAL  DEFAULT   11 _ZN8smallvec17SmallVec$LT$A$GT$11try_reserve17h51793078cfb5e6d8E
-  1171: 000000000002e3e0    83 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$std..time..Instant$u20$as$u20$core..ops..arith..Sub$GT$3sub17hadd0cdcd8032a2daE
-  1172: 000000000004e998    45 OBJECT  LOCAL  DEFAULT   13 anon.0dba3d2caacf458fc44311757361bc3a.0.llvm.11213889763605633493
-  1173: 0000000000013e30    21 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple18get_item_unchecked17hc67f48c6e9022ebeE
-  1174: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyBlockingIOError$u20$as$u20$core..fmt..Debug$GT$3fmt17he4dd842ae4afce23E
-  1175: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyBaseException$u20$as$u20$core..fmt..Debug$GT$3fmt17hfd1e70c9b387d629E
-  1176: 00000000000117c0   408 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil8GILGuard17acquire_unchecked17h08e4ae2785a111b2E.llvm.13238893432200692226
-  1177: 0000000000012e80    15 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h7d5efb1a7bcf139bE.llvm.3160907281880781123
-  1178: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr123drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..error..TryFromIntError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h72fd27cface58d1cE.llvm.3160907281880781123
-  1179: 0000000000013a00    27 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$3get17hd87c092d9792eee0E
-  1180: 0000000000047fa0    14 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders8DebugSet5entry17h7961144ed1ba1f16E
-  1181: 0000000000066129     1 OBJECT  LOCAL  DEFAULT   25 __rust_alloc_error_handler_should_panic
-  1182: 000000000002ca30     8 FUNC    LOCAL  DEFAULT   11 _ZN3std5panic13resume_unwind17hb0d2a18c77a23de6E
-  1183: 0000000000010130     4 FUNC    LOCAL  DEFAULT   11 _ZN4pyo38instance12PyNativeType18unchecked_downcast17he38549f2166334a4E
-  1184: 0000000000031590   247 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix17thread_local_dtor13register_dtor17h13e69381fc10c4fdE
-  1185: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN107_$LT$std..sync..mpsc..RecvTimeoutError$u20$as$u20$core..convert..From$LT$std..sync..mpsc..RecvError$GT$$GT$4from17h809feae83c25aa8aE
-  1186: 000000000000c080    61 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking18panic_nounwind_fmt17h520833d1447f48e9E
-  1187: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5stdio12panic_output17h19a254038a1fde18E
-  1188: 000000000004e3b0     0 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.15.llvm.18356750485614513129
-  1189: 000000000004ec17    75 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.2.llvm.5697929769133057476
-  1190: 000000000002a780     6 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread9yield_now17h198803acc80d4229E
-  1191: 0000000000048f30   196 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter26debug_struct_field2_finish17h69061813f2b8d243E
-  1192: 0000000000014d40   584 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types8function11PyCFunction12internal_new17h535a536fc017e1c8E
-  1193: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..types..mapping..PyMapping$u20$as$u20$core..fmt..Debug$GT$3fmt17hcc81c4d9f436318dE
-  1194: 000000000000f0a0  1995 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription26extract_arguments_fastcall17hcb38e9353fbe019aE
+  1164: 000000000000ea10    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h9481a0631b61df17E
+  1165: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb66f591c6d124ab0E
+  1166: 000000000002fce0    11 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$std..panicking..begin_panic_handler..StrPanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hc59bdcf586fef76cE
+  1167: 000000000004c330   291 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$u32$GT$3fmt17he422b8199910d448E
+  1168: 000000000003ad40    30 FUNC    LOCAL  DEFAULT   11 _ZN5gimli6common9SectionId4name17hb19ecacf465758f1E
+  1169: 0000000000031d40    32 FUNC    LOCAL  DEFAULT   11 _ZN3std5alloc8rust_oom17hbb2cf487567423f9E
+  1170: 0000000000031d60     9 FUNC    LOCAL  DEFAULT   11 __rg_oom
+  1171: 0000000000016860   569 FUNC    LOCAL  DEFAULT   11 _ZN8smallvec17SmallVec$LT$A$GT$11try_reserve17h51793078cfb5e6d8E
+  1172: 000000000002e3e0    83 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$std..time..Instant$u20$as$u20$core..ops..arith..Sub$GT$3sub17hadd0cdcd8032a2daE
+  1173: 000000000004e998    45 OBJECT  LOCAL  DEFAULT   13 anon.0dba3d2caacf458fc44311757361bc3a.0.llvm.11213889763605633493
+  1174: 0000000000013e30    21 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple18get_item_unchecked17hc67f48c6e9022ebeE
+  1175: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyBlockingIOError$u20$as$u20$core..fmt..Debug$GT$3fmt17he4dd842ae4afce23E
+  1176: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyBaseException$u20$as$u20$core..fmt..Debug$GT$3fmt17hfd1e70c9b387d629E
+  1177: 00000000000117c0   408 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil8GILGuard17acquire_unchecked17h08e4ae2785a111b2E.llvm.13238893432200692226
+  1178: 0000000000012e80    15 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h7d5efb1a7bcf139bE.llvm.3160907281880781123
+  1179: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr123drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..error..TryFromIntError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h72fd27cface58d1cE.llvm.3160907281880781123
+  1180: 0000000000013a00    27 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$3get17hd87c092d9792eee0E
+  1181: 0000000000047fa0    14 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders8DebugSet5entry17h7961144ed1ba1f16E
+  1182: 0000000000066129     1 OBJECT  LOCAL  DEFAULT   25 __rust_alloc_error_handler_should_panic
+  1183: 000000000002ca30     8 FUNC    LOCAL  DEFAULT   11 _ZN3std5panic13resume_unwind17hb0d2a18c77a23de6E
+  1184: 0000000000010130     4 FUNC    LOCAL  DEFAULT   11 _ZN4pyo38instance12PyNativeType18unchecked_downcast17he38549f2166334a4E
+  1185: 0000000000031590   247 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix17thread_local_dtor13register_dtor17h13e69381fc10c4fdE
+  1186: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN107_$LT$std..sync..mpsc..RecvTimeoutError$u20$as$u20$core..convert..From$LT$std..sync..mpsc..RecvError$GT$$GT$4from17h809feae83c25aa8aE
+  1187: 000000000000c080    61 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking18panic_nounwind_fmt17h520833d1447f48e9E
+  1188: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5stdio12panic_output17h19a254038a1fde18E
+  1189: 000000000004e3b0     0 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.15.llvm.18356750485614513129
+  1190: 000000000004ec17    75 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.2.llvm.5697929769133057476
+  1191: 000000000002a780     6 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread9yield_now17h198803acc80d4229E
+  1192: 0000000000048f30   196 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter26debug_struct_field2_finish17h69061813f2b8d243E
+  1193: 0000000000014d40   584 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types8function11PyCFunction12internal_new17h535a536fc017e1c8E
+  1194: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..types..mapping..PyMapping$u20$as$u20$core..fmt..Debug$GT$3fmt17hcc81c4d9f436318dE
   1195: 0000000000012ce0   204 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h8c486a937bb733fcE.llvm.3160907281880781123
   1196: 000000000000c170   116 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking18panic_bounds_check17haf06fefb23eba82dE
   1197: 0000000000009860   190 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$7reserve21do_reserve_and_handle17ha25d0b833c1f4bc4E
   1198: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyBrokenPipeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hc70b6cd767c2469dE
   1199: 000000000004baf0   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$usize$GT$3fmt17h3b8df7f7743a0bc1E
   1200: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..asyncio..QueueFull$u20$as$u20$core..fmt..Debug$GT$3fmt17hae16bea932a6cd3cE
   1201: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyFileNotFoundError$u20$as$u20$core..fmt..Display$GT$3fmt17h58399bd2dcb22b7fE
   1202: 000000000002aa40   547 FUNC    LOCAL  DEFAULT   11 _ZN3std3env7_var_os17hca6049724bd50707E
   1203: 00000000000100b0   116 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5slice64_$LT$impl$u20$alloc..borrow..ToOwned$u20$for$u20$$u5b$T$u5d$$GT$8to_owned17hb0cd7b91de122235E
   1204: 000000000000f9f0     5 FUNC    LOCAL  DEFAULT   11 __rust_alloc
   1205: 0000000000010e90   435 FUNC    LOCAL  DEFAULT   11 _ZN53_$LT$pyo3..err..PyErr$u20$as$u20$core..fmt..Debug$GT$3fmt17h9a1a85edf39ab7abE
-  1206: 000000000000f880     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8e358dedbd9e16fcE.llvm.15555921300689576899
-  1207: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyUnicodeTranslateError$u20$as$u20$core..fmt..Debug$GT$3fmt17h69da6d7c377c0f25E
-  1208: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyBaseException$u20$as$u20$core..fmt..Display$GT$3fmt17h9f8a1f0450a82077E
-  1209: 0000000000047e00   118 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders10DebugTuple6finish17hea3a905db468af57E
-  1210: 00000000000484d0  1152 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter12pad_integral17h673ca7d29b1431dbE
-  1211: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h709d04f32567c2f1E
-  1212: 000000000002fad0   279 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h33268f84f4c6e7f6E
-  1213: 0000000000000028    24 TLS     LOCAL  DEFAULT   18 _ZN4pyo33gil9GIL_COUNT7__getit5__KEY17hbdb58542edd07274E
-  1214: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySyntaxError$u20$as$u20$core..fmt..Display$GT$3fmt17hbe0d11714156a7eeE
-  1215: 00000000000157a0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr54drop_in_place$LT$$RF$mut$u20$alloc..string..String$GT$17h9b72578629773643E.llvm.3041393958569974349
-  1216: 0000000000013a80   312 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string68_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$$RF$str$GT$7extract17he4ff01f8fbafbcb9E
-  1217: 000000000000c020     9 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc18handle_alloc_error17h07edb87aaab24c34E
-  1218: 00000000000157b0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.3041393958569974349
-  1219: 00000000000105c0   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr81drop_in_place$LT$core..option..Option$LT$pyo3..err..err_state..PyErrState$GT$$GT$17hc8079f64f31b1f10E.llvm.1386185271139027476
-  1220: 000000000004eb80    45 OBJECT  LOCAL  DEFAULT   13 anon.b4bc1e6dd908342f3bb54e6363ef7da8.20.llvm.6572068071283858929
-  1221: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyConnectionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hdaa4c97d37b97a88E
+  1206: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN78_$LT$pyo3..exceptions..PyUnicodeTranslateError$u20$as$u20$core..fmt..Debug$GT$3fmt17h69da6d7c377c0f25E
+  1207: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyBaseException$u20$as$u20$core..fmt..Display$GT$3fmt17h9f8a1f0450a82077E
+  1208: 0000000000047e00   118 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt8builders10DebugTuple6finish17hea3a905db468af57E
+  1209: 00000000000484d0  1152 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter12pad_integral17h673ca7d29b1431dbE
+  1210: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h709d04f32567c2f1E
+  1211: 000000000002fad0   279 FUNC    LOCAL  DEFAULT   11 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h33268f84f4c6e7f6E
+  1212: 0000000000000028    24 TLS     LOCAL  DEFAULT   18 _ZN4pyo33gil9GIL_COUNT7__getit5__KEY17hbdb58542edd07274E
+  1213: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PySyntaxError$u20$as$u20$core..fmt..Display$GT$3fmt17hbe0d11714156a7eeE
+  1214: 00000000000157a0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr54drop_in_place$LT$$RF$mut$u20$alloc..string..String$GT$17h9b72578629773643E.llvm.3041393958569974349
+  1215: 0000000000013a80   312 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string68_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$$RF$str$GT$7extract17he4ff01f8fbafbcb9E
+  1216: 000000000000c020     9 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc18handle_alloc_error17h07edb87aaab24c34E
+  1217: 00000000000157b0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.3041393958569974349
+  1218: 00000000000105c0   341 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr81drop_in_place$LT$core..option..Option$LT$pyo3..err..err_state..PyErrState$GT$$GT$17hc8079f64f31b1f10E.llvm.1386185271139027476
+  1219: 000000000004eb80    45 OBJECT  LOCAL  DEFAULT   13 anon.b4bc1e6dd908342f3bb54e6363ef7da8.20.llvm.6572068071283858929
+  1220: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyConnectionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hdaa4c97d37b97a88E
+  1221: 000000000000e9e0    22 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hbeb0974cf65501feE.llvm.6884769035450356670
   1222: 00000000000151d0    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17h37897d217944a43aE
   1223: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN69_$LT$pyo3..exceptions..PyUnicodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h97bee77a2f2873b8E
   1224: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyException$u20$as$u20$core..fmt..Display$GT$3fmt17h366bb6713a1d10d0E
-  1225: 000000000000e9e0    22 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hcc81d66abc17d19fE.llvm.3755404211422290406
-  1226: 000000000002ad80     6 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$std..io..error..Error$u20$as$u20$core..fmt..Debug$GT$3fmt17h68dc270ae3e9c68bE
-  1227: 0000000000013fe0   285 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$alloc..string..String$u20$as$u20$core..fmt..Write$GT$10write_char17h1b6d606d1cb1d5b7E.llvm.5697929769133057476
-  1228: 0000000000015730    11 FUNC    LOCAL  DEFAULT   11 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h1bffbf42511ceb72E
-  1229: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyZeroDivisionError$u20$as$u20$core..fmt..Display$GT$3fmt17h9f580bf69d5e5d43E
-  1230: 000000000004adc0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy9Utf8Chunk7invalid17h8adfbf091f209ce8E
-  1231: 0000000000012ca0    59 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h51e3209cb696486cE.llvm.3160907281880781123
-  1232: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PySyntaxError$u20$as$u20$core..fmt..Debug$GT$3fmt17h81c98345e8e67d0aE
-  1233: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyUnicodeDecodeError$u20$as$u20$core..fmt..Display$GT$3fmt17h21cb6c1e172b2f39E
-  1234: 00000000000175d0     9 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h8068a05dc4515173E
-  1235: 000000000004b9c0   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u32$GT$3fmt17hf4a1c53fec4ddae0E
-  1236: 0000000000016710   135 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr92drop_in_place$LT$std..io..Write..write_fmt..Adapter$LT$std..sys..unix..stdio..Stderr$GT$$GT$17hc4a130cf0ed6b183E.llvm.8364735172703476354
-  1237: 000000000000ecb0    59 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h26b53fd72e755dc5E.llvm.3109625712416505353
-  1238: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h2a3f9d42403f81a5E.llvm.13238893432200692226
-  1239: 000000000000c040    53 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking9panic_fmt17hf33a1475b4dc5c3eE
-  1240: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hde9ef4f8da514fa2E
-  1241: 00000000000476d0     5 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo8location17hbf5fdab53ce4ee25E
-  1242: 0000000000017320     9 FUNC    LOCAL  DEFAULT   11 _ZN83_$LT$parking_lot_core..parking_lot..ThreadData$u20$as$u20$core..ops..drop..Drop$GT$4drop17h2922879b2a7d20a0E
-  1243: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h559c916dc6f13dc2E
-  1244: 0000000000062868    40 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.0.llvm.13238893432200692226
-  1245: 000000000002f3f0  1027 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking12default_hook17ha3500da57aa4ac4fE
-  1246: 000000000002e290   183 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path6is_dir17h6f11f52bef130b39E
-  1247: 0000000000066180    32 OBJECT  LOCAL  DEFAULT   25 _ZN3std9panicking4HOOK17h7bb63a64ad501087E
-  1248: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr121drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..error..ParseIntError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hbb3e1eaf81b89180E.llvm.3160907281880781123
-  1249: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN82_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hc4bd6dc556cbed48E
-  1250: 000000000004e7b0    16 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.40.llvm.13238893432200692226
-  1251: 0000000000014650     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr48drop_in_place$LT$core..str..error..Utf8Error$GT$17h2ce34d3d0d92f30dE.llvm.17695762341781453012
+  1225: 000000000002ad80     6 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$std..io..error..Error$u20$as$u20$core..fmt..Debug$GT$3fmt17h68dc270ae3e9c68bE
+  1226: 0000000000013fe0   285 FUNC    LOCAL  DEFAULT   11 _ZN58_$LT$alloc..string..String$u20$as$u20$core..fmt..Write$GT$10write_char17h1b6d606d1cb1d5b7E.llvm.5697929769133057476
+  1227: 0000000000015730    11 FUNC    LOCAL  DEFAULT   11 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h1bffbf42511ceb72E
+  1228: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyZeroDivisionError$u20$as$u20$core..fmt..Display$GT$3fmt17h9f580bf69d5e5d43E
+  1229: 000000000004adc0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy9Utf8Chunk7invalid17h8adfbf091f209ce8E
+  1230: 0000000000012ca0    59 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h51e3209cb696486cE.llvm.3160907281880781123
+  1231: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PySyntaxError$u20$as$u20$core..fmt..Debug$GT$3fmt17h81c98345e8e67d0aE
+  1232: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyUnicodeDecodeError$u20$as$u20$core..fmt..Display$GT$3fmt17h21cb6c1e172b2f39E
+  1233: 00000000000175d0     9 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h8068a05dc4515173E
+  1234: 000000000004b9c0   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u32$GT$3fmt17hf4a1c53fec4ddae0E
+  1235: 0000000000016710   135 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr92drop_in_place$LT$std..io..Write..write_fmt..Adapter$LT$std..sys..unix..stdio..Stderr$GT$$GT$17hc4a130cf0ed6b183E.llvm.8364735172703476354
+  1236: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h2a3f9d42403f81a5E.llvm.13238893432200692226
+  1237: 000000000000c040    53 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking9panic_fmt17hf33a1475b4dc5c3eE
+  1238: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hde9ef4f8da514fa2E
+  1239: 00000000000476d0     5 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo8location17hbf5fdab53ce4ee25E
+  1240: 0000000000017320     9 FUNC    LOCAL  DEFAULT   11 _ZN83_$LT$parking_lot_core..parking_lot..ThreadData$u20$as$u20$core..ops..drop..Drop$GT$4drop17h2922879b2a7d20a0E
+  1241: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h559c916dc6f13dc2E
+  1242: 00000000000624b8    32 OBJECT  LOCAL  DEFAULT   21 anon.93bf4d71f312183112856023db87c3c8.0.llvm.6884769035450356670
+  1243: 0000000000062868    40 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.0.llvm.13238893432200692226
+  1244: 000000000002f3f0  1027 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking12default_hook17ha3500da57aa4ac4fE
+  1245: 000000000002e290   183 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path6is_dir17h6f11f52bef130b39E
+  1246: 0000000000066180    32 OBJECT  LOCAL  DEFAULT   25 _ZN3std9panicking4HOOK17h7bb63a64ad501087E
+  1247: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr121drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..error..ParseIntError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hbb3e1eaf81b89180E.llvm.3160907281880781123
+  1248: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN82_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hc4bd6dc556cbed48E
+  1249: 000000000004e7b0    16 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.40.llvm.13238893432200692226
+  1250: 0000000000014650     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr48drop_in_place$LT$core..str..error..Utf8Error$GT$17h2ce34d3d0d92f30dE.llvm.17695762341781453012
+  1251: 000000000000ed80    59 FUNC    LOCAL  DEFAULT   11 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h977ad689fd3c5283E.llvm.11200713541412871589
   1252: 00000000000151f0    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17hb04fa46bfea55216E
   1253: 000000000003a420   464 FUNC    LOCAL  DEFAULT   11 _ZN6memchr6memchr3x864sse26memchr17hd182aafbd6503693E
   1254: 000000000002ca40   218 FUNC    LOCAL  DEFAULT   11 _ZN3std5panic19get_backtrace_style17haa81a24714daee33E
   1255: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.13238893432200692226
   1256: 0000000000012450   449 FUNC    LOCAL  DEFAULT   11 _ZN98_$LT$alloc..vec..Vec$LT$T$GT$$u20$as$u20$alloc..vec..spec_from_iter..SpecFromIter$LT$T$C$I$GT$$GT$9from_iter17h1f8acbcf324ddd43E
-  1257: 000000000004e275     8 OBJECT  LOCAL  DEFAULT   13 anon.d19f1da36be9ba6275b9cff1cbdd3d97.0.llvm.16395832583172200221
-  1258: 0000000000000040    48 TLS     LOCAL  DEFAULT   18 _ZN4pyo33gil13OWNED_OBJECTS7__getit5__KEY17hbeed0358bb5e9986E
-  1259: 000000000002e370   101 FUNC    LOCAL  DEFAULT   11 _ZN88_$LT$std..time..Instant$u20$as$u20$core..ops..arith..Add$LT$core..time..Duration$GT$$GT$3add17h06566c3a94841a50E
-  1260: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h636b6b3f321039adE
-  1261: 0000000000062588    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.9.llvm.18356750485614513129
-  1262: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyLookupError$u20$as$u20$core..fmt..Display$GT$3fmt17hb55fb57d25dc6d97E
-  1263: 0000000000014f90     9 FUNC    LOCAL  DEFAULT   11 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h387229845c3413fbE
-  1264: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c91d92007304598E
-  1265: 0000000000062910    24 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.39.llvm.13238893432200692226
-  1266: 000000000002df10   700 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path13_strip_prefix17h9a2ea8579314a83aE
-  1267: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr155drop_in_place$LT$parking_lot..once..Once..call_once_force$LT$pyo3..gil..GILGuard..acquire..$u7b$$u7b$closure$u7d$$u7d$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h077f002e42e272c7E.llvm.13238893432200692226
-  1268: 0000000000046fa0   144 FUNC    LOCAL  DEFAULT   11 _ZN98_$LT$alloc..string..String$u20$as$u20$core..convert..From$LT$alloc..borrow..Cow$LT$str$GT$$GT$$GT$4from17h12f8e1c107e4d81eE
-  1269: 0000000000062760    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.28.llvm.1386185271139027476
-  1270: 0000000000046b40   694 FUNC    LOCAL  DEFAULT   11 _ZN5alloc6string6String15from_utf8_lossy17hf3c0139dbcedaff0E
-  1271: 000000000000fea0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$i64$C$pyo3..err..PyErr$GT$$GT$17h3d326b537301a231E.llvm.18356750485614513129
+  1257: 0000000000000040    48 TLS     LOCAL  DEFAULT   18 _ZN4pyo33gil13OWNED_OBJECTS7__getit5__KEY17hbeed0358bb5e9986E
+  1258: 000000000002e370   101 FUNC    LOCAL  DEFAULT   11 _ZN88_$LT$std..time..Instant$u20$as$u20$core..ops..arith..Add$LT$core..time..Duration$GT$$GT$3add17h06566c3a94841a50E
+  1259: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h636b6b3f321039adE
+  1260: 0000000000062588    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.9.llvm.18356750485614513129
+  1261: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyLookupError$u20$as$u20$core..fmt..Display$GT$3fmt17hb55fb57d25dc6d97E
+  1262: 0000000000014f90     9 FUNC    LOCAL  DEFAULT   11 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h387229845c3413fbE
+  1263: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN67_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c91d92007304598E
+  1264: 0000000000062910    24 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.39.llvm.13238893432200692226
+  1265: 000000000002df10   700 FUNC    LOCAL  DEFAULT   11 _ZN3std4path4Path13_strip_prefix17h9a2ea8579314a83aE
+  1266: 0000000000011460     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr155drop_in_place$LT$parking_lot..once..Once..call_once_force$LT$pyo3..gil..GILGuard..acquire..$u7b$$u7b$closure$u7d$$u7d$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h077f002e42e272c7E.llvm.13238893432200692226
+  1267: 0000000000046fa0   144 FUNC    LOCAL  DEFAULT   11 _ZN98_$LT$alloc..string..String$u20$as$u20$core..convert..From$LT$alloc..borrow..Cow$LT$str$GT$$GT$$GT$4from17h12f8e1c107e4d81eE
+  1268: 0000000000062760    24 OBJECT  LOCAL  DEFAULT   21 anon.e9eb237cf50a43b65d636b0f4770b04e.28.llvm.1386185271139027476
+  1269: 0000000000046b40   694 FUNC    LOCAL  DEFAULT   11 _ZN5alloc6string6String15from_utf8_lossy17hf3c0139dbcedaff0E
+  1270: 000000000000fea0    16 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$i64$C$pyo3..err..PyErr$GT$$GT$17h3d326b537301a231E.llvm.18356750485614513129
+  1271: 000000000000ea00     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17ha5a91e081dbb3ca6E.llvm.6884769035450356670
   1272: 000000000004c8e0    56 FUNC    LOCAL  DEFAULT   11 _ZN4core7unicode12unicode_data2cc6lookup17hee9d0af768da4b93E
   1273: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyFloatingPointError$u20$as$u20$core..fmt..Debug$GT$3fmt17haed3868103eaa2ffE
   1274: 0000000000011960   195 FUNC    LOCAL  DEFAULT   11 _ZN61_$LT$pyo3..gil..GILGuard$u20$as$u20$core..ops..drop..Drop$GT$4drop17h7715afefce27b8edE
   1275: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyZeroDivisionError$u20$as$u20$core..fmt..Debug$GT$3fmt17h28e84e86a4b46619E
   1276: 0000000000015210    26 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311type_object10PyTypeInfo11type_object17hc53719a37bf25210E
   1277: 000000000004a6c0   430 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5count23char_count_general_case17hea35bb248bd0d6b7E
   1278: 000000000004f05c    45 OBJECT  LOCAL  DEFAULT   13 anon.97ad931c54c885ca96dfd72ef10ab038.13.llvm.3041393958569974349
@@ -1390,118 +1390,118 @@
   1281: 000000000004b660   175 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$core..num..error..ParseIntError$u20$as$u20$core..fmt..Debug$GT$3fmt17hdeaa4371c344e8f0E
   1282: 000000000004e74d    22 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.51.llvm.1386185271139027476
   1283: 00000000000104e0    31 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr50drop_in_place$LT$alloc..borrow..Cow$LT$str$GT$$GT$17hb21c8154e58f0fc6E.llvm.1386185271139027476
   1284: 000000000000c210   459 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking19assert_failed_inner17haf9816227b20b6f2E
   1285: 0000000000013a20    92 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h96f1e733775c6f71E
   1286: 000000000000ba80    26 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking11panic_count17is_zero_slow_path17h1c191696d45b483bE
   1287: 000000000004c1f0   310 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$i32$GT$3fmt17hbd794a33ffeb7abcE
-  1288: 000000000000ea30    71 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err9err_state10boxed_args17hddae8416b037d705E
-  1289: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyKeyboardInterrupt$u20$as$u20$core..fmt..Debug$GT$3fmt17h3cd60c245455cf6fE
-  1290: 000000000002e590   616 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..sys_common..backtrace.._print..DisplayBacktrace$u20$as$u20$core..fmt..Display$GT$3fmt17h5779d7bf7f70cb0cE
-  1291: 000000000003a250    84 FUNC    LOCAL  DEFAULT   11 __rust_panic_cleanup
-  1292: 000000000004ef7e    83 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.63.llvm.17695762341781453012
-  1293: 0000000000031580     3 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stdout$u20$as$u20$std..io..Write$GT$5flush17h542738ef7b7c1157E
-  1294: 0000000000010760   228 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr10from_value17h7ced6e799edb8b86E
-  1295: 0000000000049040   182 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter25debug_tuple_field1_finish17h67a4669c30245344E
-  1296: 00000000000159a0   104 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string133_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$alloc..string..String$GT$7into_py17h41ab879c9698f20eE
-  1297: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyFileExistsError$u20$as$u20$core..fmt..Debug$GT$3fmt17he2a503da1e9e39e1E
-  1298: 000000000000ea00     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hc1d9325495b4a971E.llvm.3755404211422290406
-  1299: 000000000004e8b7     6 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.51.llvm.13238893432200692226
-  1300: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Display$GT$3fmt17hb0aaae081fc62cbdE
-  1301: 000000000004f281    15 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.5.llvm.8364735172703476354
-  1302: 0000000000047610    18 FUNC    LOCAL  DEFAULT   11 _ZN4core3ffi5c_str4CStr6to_str17h75b7ba7fdce42660E
-  1303: 0000000000012ee0    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr122drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$LP$alloc..string..String$C$$RP$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h5348da253c5d3d92E.llvm.3160907281880781123
-  1304: 0000000000062890    32 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.13.llvm.13238893432200692226
-  1305: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyFutureWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hb9503ca5cd1cbd79E
-  1306: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyAssertionError$u20$as$u20$core..fmt..Debug$GT$3fmt17h995bf8ba6222e07bE
-  1307: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyAttributeError$u20$as$u20$core..fmt..Display$GT$3fmt17h21f68418d0de4c17E
-  1308: 000000000004add0     7 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy10Utf8Chunks3new17hb3490ab4f1f5ca96E
-  1309: 000000000004af90  1164 FUNC    LOCAL  DEFAULT   11 _ZN4core3str19slice_error_fail_rt17hdda49bed4d7161b8E
-  1310: 0000000000013bc0    44 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types7floatob115_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$f32$GT$7into_py17h0e9b009cac360ddfE
-  1311: 00000000000121e0    17 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..types..string..PyString$u20$as$u20$pyo3..type_object..PyTypeInfo$GT$10is_type_of17h1c6e4d15a14a2e24E
-  1312: 0000000000013e50    23 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple4iter17hcf53c63543c32dccE
-  1313: 000000000004f21c    73 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.0.llvm.8364735172703476354
-  1314: 000000000003c6e0    42 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read4line7LineRow18apply_line_advance17hf21823dfca79ac86E
-  1315: 0000000000048e90   159 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter26debug_struct_field1_finish17he793dca46981e51aE
-  1316: 00000000000080e0   336 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr15make_normalized17h96eddabb722b3ec5E
-  1317: 000000000003c710    46 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read4unit20allow_section_offset17hc2bbefd95499ffe9E
-  1318: 0000000000012040    76 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil13OWNED_OBJECTS7__getit17h9da6539c1a0f70fcE.llvm.13238893432200692226
-  1319: 00000000000482c0   523 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5write17h5a4baaff1bcd3eb5E
-  1320: 0000000000062988    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.33.llvm.3160907281880781123
-  1321: 00000000000167f0    92 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17hd0c995857693f37aE
-  1322: 0000000000010140     8 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..impl_..panic..PanicTrap$u20$as$u20$core..ops..drop..Drop$GT$4drop17h45a3d64251866611E
-  1323: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..types..traceback..PyTraceback$u20$as$u20$core..fmt..Debug$GT$3fmt17h10fe0663f6f65749E
-  1324: 0000000000043c00  8765 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core10decompress17h79554d21f25e7912E
-  1325: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyGeneratorExit$u20$as$u20$core..fmt..Debug$GT$3fmt17h133d26646c5e9085E
-  1326: 000000000003e110  1334 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$rustc_demangle..v0..Ident$u20$as$u20$core..fmt..Display$GT$3fmt17h8e8326fa739edc54E
-  1327: 0000000000015740    63 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write9write_fmt17h2cce5111a71a6ebaE
-  1328: 0000000000011050   394 FUNC    LOCAL  DEFAULT   11 _ZN92_$LT$pyo3..err..PyDowncastErrorArguments$u20$as$u20$pyo3..err..err_state..PyErrArguments$GT$9arguments17hd432bbf66a2521c1E
-  1329: 000000000004e9d0    16 OBJECT  LOCAL  DEFAULT   13 anon.5105bdd79f23b1171f38742feaac5d17.19.llvm.3160907281880781123
-  1330: 00000000000100a0    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.18356750485614513129
-  1331: 0000000000009920  1034 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot4once4Once14call_once_slow17h59905be63f38861cE
-  1332: 000000000004edaa    40 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.13.llvm.17695762341781453012
-  1333: 0000000000062d20    48 OBJECT  LOCAL  DEFAULT   21 anon.97ad931c54c885ca96dfd72ef10ab038.6.llvm.3041393958569974349
-  1334: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u64$GT$3fmt17hcda7d9b11480157cE
-  1335: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..asyncio..QueueEmpty$u20$as$u20$core..fmt..Debug$GT$3fmt17h752726d8ef22a032E
-  1336: 000000000000bae0   247 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks11futex_mutex5Mutex14lock_contended17h0434addfc63ba80bE
-  1337: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN65_$LT$pyo3..exceptions..PyEOFError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8528a997d6993f2eE
-  1338: 0000000000047560     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ffi5c_str4CStr8from_ptr9strlen_rt17hba550e5ac66a3aa8E
-  1339: 0000000000030190    26 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..rust_panic_without_hook..RewrapBox$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h7e39ed90a6b8e19dE
-  1340: 0000000000013170    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.3160907281880781123
-  1341: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h4703571e8d7cec5fE
-  1342: 000000000002a880   448 FUNC    LOCAL  DEFAULT   11 _ZN3std3env11current_dir17h5fb2ee7f90e6b669E
-  1343: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyImportWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h19ec3a6b4bca8db8E
-  1344: 000000000000baa0    60 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking3try7cleanup17h0a645d549942cd31E
-  1345: 0000000000015510   135 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec11finish_grow17h7d29f884b1b0f812E.llvm.5767790764768071034
-  1346: 000000000002ac70   268 FUNC    LOCAL  DEFAULT   11 _ZN3std3env11current_exe17hf5fa6473c9e891feE
-  1347: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$isize$GT$3fmt17h8bd4cc13c521ec94E
-  1348: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyResourceWarning$u20$as$u20$core..fmt..Display$GT$3fmt17ha08a08c4e8d38825E
-  1349: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyChildProcessError$u20$as$u20$core..fmt..Debug$GT$3fmt17h15a60a7a0e07ccf5E
-  1350: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyOverflowError$u20$as$u20$core..fmt..Display$GT$3fmt17h14c0e853a055ba5cE
-  1351: 000000000004e294    70 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.7.llvm.18356750485614513129
-  1352: 000000000004f310    17 OBJECT  LOCAL  DEFAULT   13 anon.e9136d4cc2f2bf733d592b5df8895207.4.llvm.17368754240468033560
-  1353: 000000000003c530   346 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev10Attributes4push17h81b548a2e2aeb86dE
-  1354: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyGeneratorExit$u20$as$u20$core..fmt..Display$GT$3fmt17h74a330a6ef290126E
-  1355: 000000000004e5e0    85 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.23.llvm.1386185271139027476
-  1356: 00000000000116a0    69 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$core..option..Option$LT$T$GT$$u20$as$u20$core..fmt..Debug$GT$3fmt17h09bf2110bdba8a44E
-  1357: 000000000003a3a0    30 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$object..read..read_ref..ReadRef$GT$13read_bytes_at17hf3a5bc16e47a26e6E
-  1358: 0000000000013bf0   115 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types7floatob64_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$f32$GT$7extract17hf873f3f904672b10E
-  1359: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyNameError$u20$as$u20$core..fmt..Display$GT$3fmt17h82f9b6453c3cd4b7E
-  1360: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyMemoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17h59c463b37f4cf48aE
-  1361: 0000000000042f00   541 FUNC    LOCAL  DEFAULT   11 _ZN63_$LT$rustc_demangle..Demangle$u20$as$u20$core..fmt..Display$GT$3fmt17h9799d3518c621ce9E
-  1362: 000000000000c520    71 FUNC    LOCAL  DEFAULT   11 _ZN4core3str6traits23str_index_overflow_fail17h76233c99258d6957E
-  1363: 0000000000010dd0   179 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr9set_cause17h30580ef7adddef0dE
-  1364: 000000000002cb20  1074 FUNC    LOCAL  DEFAULT   11 _ZN3std4path10Components7as_path17h3cc3e688e3107704E
-  1365: 0000000000047490    25 FUNC    LOCAL  DEFAULT   11 _ZN63_$LT$core..cell..BorrowMutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8848bba7b89d3f8aE
-  1366: 000000000004b9c0   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i32$GT$3fmt17hfa81d1d5a2794b7dE
-  1367: 0000000000012f00    83 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr125drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$pyo3..err..PyDowncastErrorArguments$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h876d59fe3b130b07E.llvm.3160907281880781123
-  1368: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN103_$LT$std..sync..mpsc..TryRecvError$u20$as$u20$core..convert..From$LT$std..sync..mpsc..RecvError$GT$$GT$4from17hb2cf803f361b62e1E
-  1369: 000000000004e690    54 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.29.llvm.1386185271139027476
-  1370: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyNotADirectoryError$u20$as$u20$core..fmt..Display$GT$3fmt17h12984b10e0ebfe84E
-  1371: 000000000002b080  1258 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$std..io..error..Error$u20$as$u20$core..fmt..Display$GT$3fmt17h3e34292f6cd5fc40E
-  1372: 000000000002f090   147 FUNC    LOCAL  DEFAULT   11 __rdl_realloc
-  1373: 000000000004ec88    33 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.41.llvm.5697929769133057476
-  1374: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr123drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..net..parser..AddrParseError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hac83f5491bc17d35E.llvm.3160907281880781123
-  1375: 0000000000048280    53 FUNC    LOCAL  DEFAULT   11 _ZN59_$LT$core..fmt..Arguments$u20$as$u20$core..fmt..Display$GT$3fmt17h4175b056ed0fab26E
-  1376: 000000000000bd60   211 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks12futex_rwlock6RwLock22wake_writer_or_readers17h5ba4b7f800cbd044E
-  1377: 000000000004ee6b   235 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.61.llvm.17695762341781453012
-  1378: 0000000000062c60    32 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.11.llvm.5697929769133057476
-  1379: 000000000004b550   271 FUNC    LOCAL  DEFAULT   11 _ZN4core7unicode9printable12is_printable17h9a667342c71264f9E
-  1380: 0000000000014890   295 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule4name17h712b4c83f8428570E
-  1381: 000000000003c450   132 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev12Abbreviation3new17h18ac850b45d83fddE
-  1382: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyMemoryError$u20$as$u20$core..fmt..Display$GT$3fmt17habca19cce5afc9efE
-  1383: 0000000000048df0    56 FUNC    LOCAL  DEFAULT   11 _ZN57_$LT$core..fmt..Formatter$u20$as$u20$core..fmt..Write$GT$9write_fmt17h65d14c935cd71efbE
-  1384: 0000000000011a30   385 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil13ReferencePool13update_counts17h3487d8f570027c15E
-  1385: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..asyncio..TimeoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h5562d471cf41072dE
-  1386: 00000000000105b0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr78drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..typeobject..PyType$GT$$GT$17h2215d3a9b0be969cE.llvm.1386185271139027476
-  1387: 0000000000008480  1080 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription29too_many_positional_arguments17h79543ff9496fadb6E
-  1388: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyStopIteration$u20$as$u20$core..fmt..Display$GT$3fmt17h606efbd94856db6fE
-  1389: 0000000000012e50    43 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h73e7a97655bd7fa0E.llvm.3160907281880781123
-  1390: 000000000002bde0   297 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5stdio7_eprint17h2192cf8e233cd6aaE
-  1391: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyUnicodeEncodeError$u20$as$u20$core..fmt..Display$GT$3fmt17hfa595561278bc36fE
+  1288: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyKeyboardInterrupt$u20$as$u20$core..fmt..Debug$GT$3fmt17h3cd60c245455cf6fE
+  1289: 000000000002e590   616 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..sys_common..backtrace.._print..DisplayBacktrace$u20$as$u20$core..fmt..Display$GT$3fmt17h5779d7bf7f70cb0cE
+  1290: 000000000003a250    84 FUNC    LOCAL  DEFAULT   11 __rust_panic_cleanup
+  1291: 000000000004ef7e    83 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.63.llvm.17695762341781453012
+  1292: 0000000000031580     3 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$std..sys..unix..stdio..Stdout$u20$as$u20$std..io..Write$GT$5flush17h542738ef7b7c1157E
+  1293: 0000000000010760   228 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr10from_value17h7ced6e799edb8b86E
+  1294: 0000000000049040   182 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter25debug_tuple_field1_finish17h67a4669c30245344E
+  1295: 00000000000159a0   104 FUNC    LOCAL  DEFAULT   11 _ZN4pyo311conversions3std6string133_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$alloc..string..String$GT$7into_py17h41ab879c9698f20eE
+  1296: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyFileExistsError$u20$as$u20$core..fmt..Debug$GT$3fmt17he2a503da1e9e39e1E
+  1297: 000000000004e8b7     6 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.51.llvm.13238893432200692226
+  1298: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Display$GT$3fmt17hb0aaae081fc62cbdE
+  1299: 000000000004f281    15 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.5.llvm.8364735172703476354
+  1300: 0000000000047610    18 FUNC    LOCAL  DEFAULT   11 _ZN4core3ffi5c_str4CStr6to_str17h75b7ba7fdce42660E
+  1301: 0000000000012ee0    24 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr122drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$LP$alloc..string..String$C$$RP$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h5348da253c5d3d92E.llvm.3160907281880781123
+  1302: 0000000000062890    32 OBJECT  LOCAL  DEFAULT   21 anon.b9a0486c00a4172b7b1ac52b315aa4a3.13.llvm.13238893432200692226
+  1303: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyFutureWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hb9503ca5cd1cbd79E
+  1304: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..exceptions..PyAssertionError$u20$as$u20$core..fmt..Debug$GT$3fmt17h995bf8ba6222e07bE
+  1305: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN73_$LT$pyo3..exceptions..PyAttributeError$u20$as$u20$core..fmt..Display$GT$3fmt17h21f68418d0de4c17E
+  1306: 000000000004add0     7 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy10Utf8Chunks3new17hb3490ab4f1f5ca96E
+  1307: 000000000004af90  1164 FUNC    LOCAL  DEFAULT   11 _ZN4core3str19slice_error_fail_rt17hdda49bed4d7161b8E
+  1308: 0000000000013bc0    44 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types7floatob115_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$f32$GT$7into_py17h0e9b009cac360ddfE
+  1309: 00000000000121e0    17 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$pyo3..types..string..PyString$u20$as$u20$pyo3..type_object..PyTypeInfo$GT$10is_type_of17h1c6e4d15a14a2e24E
+  1310: 0000000000013e50    23 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple7PyTuple4iter17hcf53c63543c32dccE
+  1311: 000000000004f21c    73 OBJECT  LOCAL  DEFAULT   13 anon.9e114ed5010d6253bd261129473cd188.0.llvm.8364735172703476354
+  1312: 000000000003c6e0    42 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read4line7LineRow18apply_line_advance17hf21823dfca79ac86E
+  1313: 0000000000048e90   159 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter26debug_struct_field1_finish17he793dca46981e51aE
+  1314: 00000000000080e0   336 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr15make_normalized17h96eddabb722b3ec5E
+  1315: 000000000003c710    46 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read4unit20allow_section_offset17hc2bbefd95499ffe9E
+  1316: 0000000000012040    76 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil13OWNED_OBJECTS7__getit17h9da6539c1a0f70fcE.llvm.13238893432200692226
+  1317: 00000000000482c0   523 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5write17h5a4baaff1bcd3eb5E
+  1318: 0000000000062988    32 OBJECT  LOCAL  DEFAULT   21 anon.5105bdd79f23b1171f38742feaac5d17.33.llvm.3160907281880781123
+  1319: 00000000000167f0    92 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17hd0c995857693f37aE
+  1320: 0000000000010140     8 FUNC    LOCAL  DEFAULT   11 _ZN71_$LT$pyo3..impl_..panic..PanicTrap$u20$as$u20$core..ops..drop..Drop$GT$4drop17h45a3d64251866611E
+  1321: 0000000000012090   323 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..types..traceback..PyTraceback$u20$as$u20$core..fmt..Debug$GT$3fmt17h10fe0663f6f65749E
+  1322: 0000000000043c00  8765 FUNC    LOCAL  DEFAULT   11 _ZN11miniz_oxide7inflate4core10decompress17h79554d21f25e7912E
+  1323: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyGeneratorExit$u20$as$u20$core..fmt..Debug$GT$3fmt17h133d26646c5e9085E
+  1324: 000000000003e110  1334 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$rustc_demangle..v0..Ident$u20$as$u20$core..fmt..Display$GT$3fmt17h8e8326fa739edc54E
+  1325: 0000000000015740    63 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write9write_fmt17h2cce5111a71a6ebaE
+  1326: 0000000000011050   394 FUNC    LOCAL  DEFAULT   11 _ZN92_$LT$pyo3..err..PyDowncastErrorArguments$u20$as$u20$pyo3..err..err_state..PyErrArguments$GT$9arguments17hd432bbf66a2521c1E
+  1327: 000000000004e9d0    16 OBJECT  LOCAL  DEFAULT   13 anon.5105bdd79f23b1171f38742feaac5d17.19.llvm.3160907281880781123
+  1328: 00000000000100a0    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.18356750485614513129
+  1329: 0000000000009920  1034 FUNC    LOCAL  DEFAULT   11 _ZN11parking_lot4once4Once14call_once_slow17h59905be63f38861cE
+  1330: 000000000004edaa    40 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.13.llvm.17695762341781453012
+  1331: 0000000000062d20    48 OBJECT  LOCAL  DEFAULT   21 anon.97ad931c54c885ca96dfd72ef10ab038.6.llvm.3041393958569974349
+  1332: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u64$GT$3fmt17hcda7d9b11480157cE
+  1333: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..asyncio..QueueEmpty$u20$as$u20$core..fmt..Debug$GT$3fmt17h752726d8ef22a032E
+  1334: 000000000000bae0   247 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks11futex_mutex5Mutex14lock_contended17h0434addfc63ba80bE
+  1335: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN65_$LT$pyo3..exceptions..PyEOFError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8528a997d6993f2eE
+  1336: 0000000000047560     6 FUNC    LOCAL  DEFAULT   11 _ZN4core3ffi5c_str4CStr8from_ptr9strlen_rt17hba550e5ac66a3aa8E
+  1337: 0000000000030190    26 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$std..panicking..rust_panic_without_hook..RewrapBox$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h7e39ed90a6b8e19dE
+  1338: 0000000000013170    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.3160907281880781123
+  1339: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN64_$LT$pyo3..exceptions..PyWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h4703571e8d7cec5fE
+  1340: 000000000002a880   448 FUNC    LOCAL  DEFAULT   11 _ZN3std3env11current_dir17h5fb2ee7f90e6b669E
+  1341: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyImportWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h19ec3a6b4bca8db8E
+  1342: 000000000000baa0    60 FUNC    LOCAL  DEFAULT   11 _ZN3std9panicking3try7cleanup17h0a645d549942cd31E
+  1343: 0000000000015510   135 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec11finish_grow17h7d29f884b1b0f812E.llvm.5767790764768071034
+  1344: 000000000002ac70   268 FUNC    LOCAL  DEFAULT   11 _ZN3std3env11current_exe17hf5fa6473c9e891feE
+  1345: 000000000004ba50   146 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$isize$GT$3fmt17h8bd4cc13c521ec94E
+  1346: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyResourceWarning$u20$as$u20$core..fmt..Display$GT$3fmt17ha08a08c4e8d38825E
+  1347: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN74_$LT$pyo3..exceptions..PyChildProcessError$u20$as$u20$core..fmt..Debug$GT$3fmt17h15a60a7a0e07ccf5E
+  1348: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyOverflowError$u20$as$u20$core..fmt..Display$GT$3fmt17h14c0e853a055ba5cE
+  1349: 000000000004e294    70 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.7.llvm.18356750485614513129
+  1350: 000000000004f310    17 OBJECT  LOCAL  DEFAULT   13 anon.e9136d4cc2f2bf733d592b5df8895207.4.llvm.17368754240468033560
+  1351: 000000000003c530   346 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev10Attributes4push17h81b548a2e2aeb86dE
+  1352: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyGeneratorExit$u20$as$u20$core..fmt..Display$GT$3fmt17h74a330a6ef290126E
+  1353: 000000000004e5e0    85 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.23.llvm.1386185271139027476
+  1354: 00000000000116a0    69 FUNC    LOCAL  DEFAULT   11 _ZN66_$LT$core..option..Option$LT$T$GT$$u20$as$u20$core..fmt..Debug$GT$3fmt17h09bf2110bdba8a44E
+  1355: 000000000003a3a0    30 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$object..read..read_ref..ReadRef$GT$13read_bytes_at17hf3a5bc16e47a26e6E
+  1356: 0000000000013bf0   115 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types7floatob64_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$f32$GT$7extract17hf873f3f904672b10E
+  1357: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyNameError$u20$as$u20$core..fmt..Display$GT$3fmt17h82f9b6453c3cd4b7E
+  1358: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyMemoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17h59c463b37f4cf48aE
+  1359: 0000000000042f00   541 FUNC    LOCAL  DEFAULT   11 _ZN63_$LT$rustc_demangle..Demangle$u20$as$u20$core..fmt..Display$GT$3fmt17h9799d3518c621ce9E
+  1360: 000000000000c520    71 FUNC    LOCAL  DEFAULT   11 _ZN4core3str6traits23str_index_overflow_fail17h76233c99258d6957E
+  1361: 0000000000010dd0   179 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err5PyErr9set_cause17h30580ef7adddef0dE
+  1362: 000000000002cb20  1074 FUNC    LOCAL  DEFAULT   11 _ZN3std4path10Components7as_path17h3cc3e688e3107704E
+  1363: 0000000000047490    25 FUNC    LOCAL  DEFAULT   11 _ZN63_$LT$core..cell..BorrowMutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8848bba7b89d3f8aE
+  1364: 000000000004b9c0   143 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i32$GT$3fmt17hfa81d1d5a2794b7dE
+  1365: 0000000000012f00    83 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr125drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$pyo3..err..PyDowncastErrorArguments$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h876d59fe3b130b07E.llvm.3160907281880781123
+  1366: 000000000002e350     3 FUNC    LOCAL  DEFAULT   11 _ZN103_$LT$std..sync..mpsc..TryRecvError$u20$as$u20$core..convert..From$LT$std..sync..mpsc..RecvError$GT$$GT$4from17hb2cf803f361b62e1E
+  1367: 000000000004e690    54 OBJECT  LOCAL  DEFAULT   13 anon.e9eb237cf50a43b65d636b0f4770b04e.29.llvm.1386185271139027476
+  1368: 000000000004e275     8 OBJECT  LOCAL  DEFAULT   13 anon.aa4339ca2dbb296fa63ba57d58d55e89.0.llvm.15280094018889411062
+  1369: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyNotADirectoryError$u20$as$u20$core..fmt..Display$GT$3fmt17h12984b10e0ebfe84E
+  1370: 000000000002b080  1258 FUNC    LOCAL  DEFAULT   11 _ZN60_$LT$std..io..error..Error$u20$as$u20$core..fmt..Display$GT$3fmt17h3e34292f6cd5fc40E
+  1371: 000000000002f090   147 FUNC    LOCAL  DEFAULT   11 __rdl_realloc
+  1372: 000000000004ec88    33 OBJECT  LOCAL  DEFAULT   13 anon.682f053ba3d6d14af5b27cfcbbd16363.41.llvm.5697929769133057476
+  1373: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr123drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..net..parser..AddrParseError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hac83f5491bc17d35E.llvm.3160907281880781123
+  1374: 0000000000048280    53 FUNC    LOCAL  DEFAULT   11 _ZN59_$LT$core..fmt..Arguments$u20$as$u20$core..fmt..Display$GT$3fmt17h4175b056ed0fab26E
+  1375: 000000000000bd60   211 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix5locks12futex_rwlock6RwLock22wake_writer_or_readers17h5ba4b7f800cbd044E
+  1376: 000000000004ee6b   235 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.61.llvm.17695762341781453012
+  1377: 0000000000062c60    32 OBJECT  LOCAL  DEFAULT   21 anon.682f053ba3d6d14af5b27cfcbbd16363.11.llvm.5697929769133057476
+  1378: 000000000004b550   271 FUNC    LOCAL  DEFAULT   11 _ZN4core7unicode9printable12is_printable17h9a667342c71264f9E
+  1379: 0000000000014890   295 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6module8PyModule4name17h712b4c83f8428570E
+  1380: 000000000003c450   132 FUNC    LOCAL  DEFAULT   11 _ZN5gimli4read6abbrev12Abbreviation3new17h18ac850b45d83fddE
+  1381: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN70_$LT$pyo3..exceptions..PyMemoryError$u20$as$u20$core..fmt..Display$GT$3fmt17habca19cce5afc9efE
+  1382: 0000000000048df0    56 FUNC    LOCAL  DEFAULT   11 _ZN57_$LT$core..fmt..Formatter$u20$as$u20$core..fmt..Write$GT$9write_fmt17h65d14c935cd71efbE
+  1383: 0000000000011a30   385 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33gil13ReferencePool13update_counts17h3487d8f570027c15E
+  1384: 0000000000013890   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..asyncio..TimeoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h5562d471cf41072dE
+  1385: 00000000000105b0     9 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr78drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..typeobject..PyType$GT$$GT$17h2215d3a9b0be969cE.llvm.1386185271139027476
+  1386: 0000000000008480  1080 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription29too_many_positional_arguments17h79543ff9496fadb6E
+  1387: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN72_$LT$pyo3..exceptions..PyStopIteration$u20$as$u20$core..fmt..Display$GT$3fmt17h606efbd94856db6fE
+  1388: 0000000000012e50    43 FUNC    LOCAL  DEFAULT   11 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h73e7a97655bd7fa0E.llvm.3160907281880781123
+  1389: 000000000002bde0   297 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5stdio7_eprint17h2192cf8e233cd6aaE
+  1390: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN77_$LT$pyo3..exceptions..PyUnicodeEncodeError$u20$as$u20$core..fmt..Display$GT$3fmt17hfa595561278bc36fE
+  1391: 000000000000e5e0   662 FUNC    LOCAL  DEFAULT   11 _ZN7georgio7georgio17h17ee84be84d4a39bE
   1392: 00000000000474b0   174 FUNC    LOCAL  DEFAULT   11 _ZN84_$LT$core..char..EscapeDefault$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h85f66e8546c5bd58E
   1393: 00000000000476e0     5 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo10can_unwind17hcbb863668b6703efE
   1394: 00000000000478d0   477 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$core..fmt..builders..PadAdapter$u20$as$u20$core..fmt..Write$GT$9write_str17hb31c05454b680aa2E
   1395: 000000000004ebb3    45 OBJECT  LOCAL  DEFAULT   13 anon.a80902d6bb08773bf6743d023c7df73e.17.llvm.11940621367560662805
   1396: 0000000000062cd8    24 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.15.llvm.17695762341781453012
   1397: 0000000000047570   157 FUNC    LOCAL  DEFAULT   11 _ZN4core3ffi5c_str4CStr19from_bytes_with_nul17h60ba6b79363256ccE
   1398: 0000000000015250   345 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$pyo3..exceptions..PyBufferError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1e3fb4a30e09ed54E
@@ -1511,18 +1511,18 @@
   1402: 000000000006612a     1 OBJECT  LOCAL  DEFAULT   25 _ZN4pyo33gil5START17h58523f084b8fc918E.llvm.13238893432200692226
   1403: 000000000004e3b0    45 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.29.llvm.18356750485614513129
   1404: 0000000000008ad0   502 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription27unexpected_keyword_argument17hc2ea0316549b7cb1E
   1405: 000000000000fa40    11 FUNC    LOCAL  DEFAULT   11 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h37d3081fa7e91287E
   1406: 0000000000048240    45 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt9Formatter3new17hd94366d3ae6cbcdfE
   1407: 00000000000476b0     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5panic10panic_info9PanicInfo7payload17hb3d2134487894de8E
   1408: 000000000000fa30     5 FUNC    LOCAL  DEFAULT   11 __rust_alloc_error_handler
-  1409: 000000000000fe90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr52drop_in_place$LT$std..thread..local..AccessError$GT$17h697bd454dd3ba1fbE.llvm.18356750485614513129
-  1410: 0000000000011ed0   355 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6string8PyString15to_string_lossy17hd99f20cf0c825b2bE
-  1411: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr119drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$alloc..string..FromUtf16Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h94811fe4ace74af2E.llvm.3160907281880781123
-  1412: 000000000000f890   142 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types5tuple127_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$RP$$GT$7into_py17h20a8054c1a24cbd3E
+  1409: 000000000000e910   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h168a900aa3e0c8b8E
+  1410: 000000000000fe90     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr52drop_in_place$LT$std..thread..local..AccessError$GT$17h697bd454dd3ba1fbE.llvm.18356750485614513129
+  1411: 0000000000011ed0   355 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types6string8PyString15to_string_lossy17hd99f20cf0c825b2bE
+  1412: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr119drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$alloc..string..FromUtf16Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h94811fe4ace74af2E.llvm.3160907281880781123
   1413: 0000000000016580   244 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5Write9write_fmt17hb89612cdacf175eeE
   1414: 0000000000008cd0   524 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription33positional_only_keyword_arguments17h69d993d0b92bda9dE
   1415: 00000000000112c0    33 FUNC    LOCAL  DEFAULT   11 _ZN4pyo33err17panic_after_error17he7adfd3ac8d1d8acE
   1416: 000000000004e3ed    81 OBJECT  LOCAL  DEFAULT   13 anon.7b946ae1d3a666797e2db1f36e4cd6e7.31.llvm.18356750485614513129
   1417: 0000000000046670   107 FUNC    LOCAL  DEFAULT   11 _ZN5alloc11collections5btree4node10splitpoint17h36555320df7972deE
   1418: 000000000000fca0     4 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr91drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$std..thread..ThreadId$GT$$GT$$GT$17h669a854d11e215cbE.llvm.18356750485614513129
   1419: 0000000000010460     5 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.1386185271139027476
@@ -1535,35 +1535,35 @@
   1426: 00000000000163e0   413 FUNC    LOCAL  DEFAULT   11 _ZN3std2io5Write9write_all17h0db8d772b302f00bE
   1427: 0000000000061de8     8 OBJECT  LOCAL  DEFAULT   19 _ZN3std3sys4unix4args3imp15ARGV_INIT_ARRAY17h30412a22fc176490E
   1428: 0000000000030da0    18 FUNC    LOCAL  DEFAULT   11 _ZN3std3sys4unix4args3imp15ARGV_INIT_ARRAY12init_wrapper17h5ed71925f6470202E
   1429: 000000000003a740   267 FUNC    LOCAL  DEFAULT   11 _ZN91_$LT$addr2line..LocationRangeUnitIter$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h3269ac4174d2858bE
   1430: 0000000000012ec0     1 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr122drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..str..error..ParseBoolError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h03a7404ff8c81eb0E.llvm.3160907281880781123
   1431: 0000000000015c90    12 FUNC    LOCAL  DEFAULT   11 _ZN5alloc5alloc8box_free17h76061aca80fb3990E.llvm.11236572853509692416
   1432: 0000000000045e40  1040 FUNC    LOCAL  DEFAULT   11 _ZN5adler7Adler3211write_slice17he2404f6f27d2ef09E
-  1433: 000000000000e910   204 FUNC    LOCAL  DEFAULT   11 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h8abd4168aa07edd0E
-  1434: 00000000000128d0   354 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types3any5PyAny7setattr17h4aeef81d02f8b7faE
-  1435: 0000000000032150   224 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$std..backtrace_rs..symbolize..SymbolName$u20$as$u20$core..fmt..Display$GT$3fmt17h434acb7722c3decbE
-  1436: 000000000003a3c0    95 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$object..read..read_ref..ReadRef$GT$19read_bytes_at_until17h170b4060dbcae77aE
-  1437: 000000000004adb0     8 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy9Utf8Chunk5valid17h15d1e98cc145018bE
-  1438: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..PyConnectionRefusedError$u20$as$u20$core..fmt..Display$GT$3fmt17haa4f80e697d069f4E
-  1439: 000000000000c470     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index26slice_start_index_len_fail17h6bee405bac6d3d26E
-  1440: 00000000000626b8    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.34.llvm.18356750485614513129
-  1441: 0000000000016680   130 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$std..io..error..Error$GT$17hc48ddf2d2077febdE.llvm.8364735172703476354
-  1442: 000000000000c0c0    79 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking5panic17h9533b2fee90b999eE
-  1443: 0000000000016b80    63 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write9write_fmt17h94ac242a54e473c7E
-  1444: 0000000000065358     0 OBJECT  LOCAL  DEFAULT   22 _DYNAMIC
-  1445: 0000000000008000     0 FUNC    LOCAL  DEFAULT    9 _init
-  1446: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyIsADirectoryError$u20$as$u20$core..fmt..Display$GT$3fmt17hd344957062e6a06eE
-  1447: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyInterruptedError$u20$as$u20$core..fmt..Display$GT$3fmt17hf7a2d4ade099865dE
-  1448: 0000000000049ab0   211 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt17pointer_fmt_inner17h97b13a612a80a456E
-  1449: 0000000000062d08    24 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.64.llvm.17695762341781453012
-  1450: 0000000000046660     4 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$alloc..collections..btree..mem..replace..PanicGuard$u20$as$u20$core..ops..drop..Drop$GT$4drop17h4183f132fb648b0aE
-  1451: 0000000000013c70    83 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c580bc7d680b708E
-  1452: 000000000004e84e    81 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.35.llvm.13238893432200692226
-  1453: 000000000004ed2d    43 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.8.llvm.17695762341781453012
+  1433: 00000000000128d0   354 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35types3any5PyAny7setattr17h4aeef81d02f8b7faE
+  1434: 0000000000032150   224 FUNC    LOCAL  DEFAULT   11 _ZN79_$LT$std..backtrace_rs..symbolize..SymbolName$u20$as$u20$core..fmt..Display$GT$3fmt17h434acb7722c3decbE
+  1435: 000000000003a3c0    95 FUNC    LOCAL  DEFAULT   11 _ZN68_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$object..read..read_ref..ReadRef$GT$19read_bytes_at_until17h170b4060dbcae77aE
+  1436: 000000000004adb0     8 FUNC    LOCAL  DEFAULT   11 _ZN4core3str5lossy9Utf8Chunk5valid17h15d1e98cc145018bE
+  1437: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN81_$LT$pyo3..exceptions..PyConnectionRefusedError$u20$as$u20$core..fmt..Display$GT$3fmt17haa4f80e697d069f4E
+  1438: 000000000000c470     8 FUNC    LOCAL  DEFAULT   11 _ZN4core5slice5index26slice_start_index_len_fail17h6bee405bac6d3d26E
+  1439: 00000000000626b8    24 OBJECT  LOCAL  DEFAULT   21 anon.7b946ae1d3a666797e2db1f36e4cd6e7.34.llvm.18356750485614513129
+  1440: 0000000000016680   130 FUNC    LOCAL  DEFAULT   11 _ZN4core3ptr42drop_in_place$LT$std..io..error..Error$GT$17hc48ddf2d2077febdE.llvm.8364735172703476354
+  1441: 000000000000c0c0    79 FUNC    LOCAL  DEFAULT   11 _ZN4core9panicking5panic17h9533b2fee90b999eE
+  1442: 0000000000016b80    63 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt5Write9write_fmt17h94ac242a54e473c7E
+  1443: 0000000000065358     0 OBJECT  LOCAL  DEFAULT   22 _DYNAMIC
+  1444: 0000000000008000     0 FUNC    LOCAL  DEFAULT    9 _init
+  1445: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN76_$LT$pyo3..exceptions..PyIsADirectoryError$u20$as$u20$core..fmt..Display$GT$3fmt17hd344957062e6a06eE
+  1446: 00000000000153b0   345 FUNC    LOCAL  DEFAULT   11 _ZN75_$LT$pyo3..exceptions..PyInterruptedError$u20$as$u20$core..fmt..Display$GT$3fmt17hf7a2d4ade099865dE
+  1447: 0000000000049ab0   211 FUNC    LOCAL  DEFAULT   11 _ZN4core3fmt17pointer_fmt_inner17h97b13a612a80a456E
+  1448: 0000000000062d08    24 OBJECT  LOCAL  DEFAULT   21 anon.347d264e34eb3a0c74be5a89f895ac7e.64.llvm.17695762341781453012
+  1449: 0000000000046660     4 FUNC    LOCAL  DEFAULT   11 _ZN93_$LT$alloc..collections..btree..mem..replace..PanicGuard$u20$as$u20$core..ops..drop..Drop$GT$4drop17h4183f132fb648b0aE
+  1450: 0000000000013c70    83 FUNC    LOCAL  DEFAULT   11 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c580bc7d680b708E
+  1451: 000000000004e84e    81 OBJECT  LOCAL  DEFAULT   13 anon.b9a0486c00a4172b7b1ac52b315aa4a3.35.llvm.13238893432200692226
+  1452: 000000000004ed2d    43 OBJECT  LOCAL  DEFAULT   13 anon.347d264e34eb3a0c74be5a89f895ac7e.8.llvm.17695762341781453012
+  1453: 000000000000f0a0  1995 FUNC    LOCAL  DEFAULT   11 _ZN4pyo35impl_16extract_argument19FunctionDescription26extract_arguments_fastcall17hf57c52c8f64057f8E
   1454: 000000000004b730     5 FUNC    LOCAL  DEFAULT   11 _ZN4core3num21_$LT$impl$u20$u32$GT$14from_str_radix17h2d973af03c66c62bE
   1455: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_BaseException
   1456: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyExc_ImportError
   1457: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND pthread_getspecific@@GLIBC_2.2.5
   1458: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND sincosf@@GLIBC_2.2.5
   1459: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND PyUnicode_AsEncodedString
   1460: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND _Unwind_GetRegionStart@@GCC_3.0
```

### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: c5fc0d173a42300b6cb532d9cc8f9c7266e6cb85
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a42d05a1a7acac8e59f30a57c0655c011de6252a
```

### readelf --wide --debug-dump=frames {}

```diff
@@ -495,38 +495,38 @@
   DW_CFA_advance_loc: 1 to 000000000000ec2f
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 1 to 000000000000ec30
   DW_CFA_def_cfa_offset: 192
   DW_CFA_nop
   DW_CFA_nop
 
-00000518 0000000000000010 0000051c FDE cie=00000000 pc=000000000000ecb0..000000000000eceb
-  DW_CFA_nop
-  DW_CFA_nop
-  DW_CFA_nop
-
-0000052c 0000000000000028 00000530 FDE cie=00000000 pc=000000000000ecf0..000000000000edbc
-  DW_CFA_advance_loc: 2 to 000000000000ecf2
+00000518 0000000000000028 0000051c FDE cie=00000000 pc=000000000000ecb0..000000000000ed7c
+  DW_CFA_advance_loc: 2 to 000000000000ecb2
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 1 to 000000000000ecf3
+  DW_CFA_advance_loc: 1 to 000000000000ecb3
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 000000000000ecf4
+  DW_CFA_advance_loc: 1 to 000000000000ecb4
   DW_CFA_def_cfa_offset: 32
   DW_CFA_offset: r3 (rbx) at cfa-24
   DW_CFA_offset: r14 (r14) at cfa-16
-  DW_CFA_advance_loc1: 178 to 000000000000eda6
+  DW_CFA_advance_loc1: 178 to 000000000000ed66
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 1 to 000000000000eda7
+  DW_CFA_advance_loc: 1 to 000000000000ed67
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000eda9
+  DW_CFA_advance_loc: 2 to 000000000000ed69
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 000000000000edaa
+  DW_CFA_advance_loc: 1 to 000000000000ed6a
   DW_CFA_def_cfa_offset: 32
   DW_CFA_nop
 
+00000544 0000000000000010 00000548 FDE cie=00000000 pc=000000000000ed80..000000000000edbb
+  DW_CFA_nop
+  DW_CFA_nop
+  DW_CFA_nop
+
 00000558 0000000000000014 0000055c FDE cie=00000000 pc=000000000000edc0..000000000000edf1
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

### strings --all --bytes=8 {}

```diff
@@ -22940,56 +22940,56 @@
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.0
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
-georgio.19a0936c-cgu.0
-_ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17hd979f0f854fbeee6E
-_ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17hdc1189a9e5f867d0E
-_ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h6ba2d1048c64ea8cE
-_ZN4pyo35impl_10trampoline16trampoline_inner17hba1a064a3097ec58E
-_ZN7georgio33great_circle_distance_with_radius17hc145202091a4857fE
-_ZN7georgio1_69_$LT$impl$u20$georgio..great_circle_distance_with_radius..MakeDef$GT$3DEF10trampoline17hf46c34048437de85E
-_ZN7georgio1_46__pyfunction_great_circle_distance_with_radius17h5da6da619ffc9b9eE
-_ZN7georgio1_57_$LT$impl$u20$georgio..great_circle_distance..MakeDef$GT$3DEF10trampoline17h3d70761bf46c1bdeE
-_ZN7georgio1_34__pyfunction_great_circle_distance17h5c90bce25ae903b2E
-_ZN7georgio27line_of_bearing_with_radius17h28decf3f8d392f2cE
-_ZN7georgio1_63_$LT$impl$u20$georgio..line_of_bearing_with_radius..MakeDef$GT$3DEF10trampoline17h852bd0f2a84d3105E
-_ZN7georgio1_40__pyfunction_line_of_bearing_with_radius17h4fad95cb7369fe96E
-_ZN7georgio1_51_$LT$impl$u20$georgio..line_of_bearing..MakeDef$GT$3DEF10trampoline17ha5398f443eb6a1d7E
-_ZN7georgio1_28__pyfunction_line_of_bearing17h5d9c3860ddbdc65bE
-_ZN7georgio1_58_$LT$impl$u20$georgio..bounding_box_for_point..MakeDef$GT$3DEF10trampoline17h3a2ba0f2aa02100aE
-_ZN7georgio1_35__pyfunction_bounding_box_for_point17h2b385783bc661c36E
-_ZN7georgio1_49_$LT$impl$u20$georgio..wm_upper_left..MakeDef$GT$3DEF10trampoline17h2bc3e2c85f91dc42E
-_ZN7georgio1_26__pyfunction_wm_upper_left17h678c4ad5aeb927eeE
-_ZN7georgio1_45_$LT$impl$u20$georgio..wm_bounds..MakeDef$GT$3DEF10trampoline17h51279b711e8f239dE
-_ZN7georgio1_22__pyfunction_wm_bounds17ha50d26ff74771c55E
-_ZN7georgio1_57_$LT$impl$u20$georgio..wm_tile_expanded_bbox..MakeDef$GT$3DEF10trampoline17h6b7383039080cdd5E
-_ZN7georgio1_34__pyfunction_wm_tile_expanded_bbox17hd39bb6ecd146df9aE
-georgio.19a0936c-cgu.1
-_ZN5alloc7raw_vec11finish_grow17h0f0680c571a6bf5cE
-georgio.19a0936c-cgu.12
-georgio.19a0936c-cgu.15
-_ZN7georgio7georgio3DEF17h59ce644008367a00E
+georgio.f1a699e4-cgu.0
+_ZN4core3ptr39drop_in_place$LT$pyo3..gil..GILPool$GT$17h6064e3786872f34fE
+_ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h166ce87cbb0731a6E
+_ZN4core3ptr50drop_in_place$LT$pyo3..impl_..panic..PanicTrap$GT$17h4e05bb1de10d2a2eE
+_ZN4pyo35impl_10trampoline16trampoline_inner17he3245367a3595406E
+_ZN7georgio33great_circle_distance_with_radius17h8d204aba89340480E
+_ZN7georgio1_69_$LT$impl$u20$georgio..great_circle_distance_with_radius..MakeDef$GT$3DEF10trampoline17h4a201d4e317ca937E
+_ZN7georgio1_46__pyfunction_great_circle_distance_with_radius17h2e75ff33b4e5382eE
+_ZN7georgio1_57_$LT$impl$u20$georgio..great_circle_distance..MakeDef$GT$3DEF10trampoline17h4a3414da561c209fE
+_ZN7georgio1_34__pyfunction_great_circle_distance17hcfe48c8236a03285E
+_ZN7georgio27line_of_bearing_with_radius17h0995938e266a3069E
+_ZN7georgio1_63_$LT$impl$u20$georgio..line_of_bearing_with_radius..MakeDef$GT$3DEF10trampoline17h94e4f1c05cbe97bfE
+_ZN7georgio1_40__pyfunction_line_of_bearing_with_radius17ha25209c681204143E
+_ZN7georgio1_51_$LT$impl$u20$georgio..line_of_bearing..MakeDef$GT$3DEF10trampoline17he73f4f45ef432c00E
+_ZN7georgio1_28__pyfunction_line_of_bearing17h4bef21559472a755E
+_ZN7georgio1_58_$LT$impl$u20$georgio..bounding_box_for_point..MakeDef$GT$3DEF10trampoline17hf9c1ddf43c25a8a2E
+_ZN7georgio1_35__pyfunction_bounding_box_for_point17hc50635714e99e173E
+_ZN7georgio1_49_$LT$impl$u20$georgio..wm_upper_left..MakeDef$GT$3DEF10trampoline17hb117ff3e28b8750aE
+_ZN7georgio1_26__pyfunction_wm_upper_left17hd00bff5216eb6a99E
+_ZN7georgio1_45_$LT$impl$u20$georgio..wm_bounds..MakeDef$GT$3DEF10trampoline17ha150e425d68a517cE
+_ZN7georgio1_22__pyfunction_wm_bounds17h1a70f88d1486ff91E
+_ZN7georgio1_57_$LT$impl$u20$georgio..wm_tile_expanded_bbox..MakeDef$GT$3DEF10trampoline17hc58de32b8417dbadE
+_ZN7georgio1_34__pyfunction_wm_tile_expanded_bbox17h4bbad28f7029c966E
+georgio.f1a699e4-cgu.1
+_ZN5alloc7raw_vec11finish_grow17h8e6501fdcc414dbdE
+georgio.f1a699e4-cgu.12
+georgio.f1a699e4-cgu.15
+_ZN7georgio7georgio3DEF17h9660d3e25df670a4E
 GCC_except_table17
-georgio.19a0936c-cgu.2
-_ZN3std6thread5local4fast13destroy_value17h7e3909d473e99117E
-georgio.19a0936c-cgu.3
-_ZN4core3ptr110drop_in_place$LT$core..option..Option$LT$pyo3..instance..Py$LT$pyo3..types..traceback..PyTraceback$GT$$GT$$GT$17hb3321db519edac54E
-_ZN4core3ptr241drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..FnOnce$LT$$LP$pyo3..marker..Python$C$$RP$$GT$$u2b$Output$u20$$u3d$$u20$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$GT$17hcc6e9d403cb3a060E
-_ZN5alloc5alloc8box_free17h9f2049ced3bddf70E
-_ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17h08a08fb1d4c4bac6E
-_ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17hd5a52c4ed0c8f64dE
-_ZN4core3ptr51drop_in_place$LT$alloc..vec..Vec$LT$$RF$str$GT$$GT$17h551e62ff05915647E
-_ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17hf56cf9b9ccef5810E
+georgio.f1a699e4-cgu.2
+_ZN3std6thread5local4fast13destroy_value17h6ae8a5d519fdd9f1E
+georgio.f1a699e4-cgu.3
+_ZN4core3ptr110drop_in_place$LT$core..option..Option$LT$pyo3..instance..Py$LT$pyo3..types..traceback..PyTraceback$GT$$GT$$GT$17he12a6bc4294cbee9E
+_ZN4core3ptr241drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..FnOnce$LT$$LP$pyo3..marker..Python$C$$RP$$GT$$u2b$Output$u20$$u3d$$u20$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$u2b$core..marker..Send$u2b$core..marker..Sync$GT$$GT$17h349d6b6f36307bf4E
+_ZN5alloc5alloc8box_free17h28ba74a08386abbaE
+_ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17h1d002b062c7545f0E
+_ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17h1568be0e80b1b17fE
+_ZN4core3ptr51drop_in_place$LT$alloc..vec..Vec$LT$$RF$str$GT$$GT$17h9613fb8006255fe6E
+_ZN4core3ptr75drop_in_place$LT$core..result..Result$LT$$RF$str$C$pyo3..err..PyErr$GT$$GT$17hb0865fc31a50c987E
 GCC_except_table8
-georgio.19a0936c-cgu.4
-1f6ox68pdmgesk6m
+georgio.f1a699e4-cgu.4
+1hzwlgomd2b1nozj
 pyo3.3025e9cd-cgu.15
 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17hc70a4e410a2bfd94E
 _ZN4core3ptr106drop_in_place$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$17hfc141806601d459cE
 _ZN4core3ptr80drop_in_place$LT$pyo3..instance..Py$LT$pyo3..exceptions..PyBaseException$GT$$GT$17h42706df4c0e8214dE
 GCC_except_table18
 _ZN4core3ptr50drop_in_place$LT$alloc..borrow..Cow$LT$str$GT$$GT$17hb21c8154e58f0fc6E
 GCC_except_table51
@@ -23096,23 +23096,23 @@
 miniz_oxide.d3ca669e-cgu.0
 _ZN11miniz_oxide7inflate4core9init_tree17hcc023a30b30982f2E
 _ZN11miniz_oxide7inflate4core8transfer17hb096912a935018f7E
 _ZN11miniz_oxide7inflate4core11apply_match17h82ef3f50adbf55c1E
 adler.6e15a4ca-cgu.0
 compiler_builtins.5665bd25-cgu.118
 compiler_builtins.5665bd25-cgu.9
-georgio.19a0936c-cgu.9
-georgio.19a0936c-cgu.10
-georgio.19a0936c-cgu.11
-georgio.19a0936c-cgu.13
-georgio.19a0936c-cgu.14
-georgio.19a0936c-cgu.5
-georgio.19a0936c-cgu.6
-georgio.19a0936c-cgu.7
-georgio.19a0936c-cgu.8
+georgio.f1a699e4-cgu.9
+georgio.f1a699e4-cgu.10
+georgio.f1a699e4-cgu.11
+georgio.f1a699e4-cgu.13
+georgio.f1a699e4-cgu.14
+georgio.f1a699e4-cgu.5
+georgio.f1a699e4-cgu.6
+georgio.f1a699e4-cgu.7
+georgio.f1a699e4-cgu.8
 pyo3.3025e9cd-cgu.14
 parking_lot_core.caf4f90a-cgu.8
 pyo3_ffi.76b49c2d-cgu.0
 pyo3_ffi.76b49c2d-cgu.13
 pyo3_ffi.76b49c2d-cgu.14
 pyo3_ffi.76b49c2d-cgu.2
 pyo3_ffi.76b49c2d-cgu.3
@@ -23130,51 +23130,49 @@
 compiler_builtins.5665bd25-cgu.44
 __FRAME_END__
 _ZN60_$LT$core..cell..BorrowError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1341f40a7115bc9cE
 _ZN91_$LT$std..backtrace_rs..symbolize..gimli..mmap..Mmap$u20$as$u20$core..ops..deref..Deref$GT$5deref17h940c9d723c6fe175E
 _ZN64_$LT$core..alloc..layout..Layout$u20$as$u20$core..fmt..Debug$GT$3fmt17h3fb65d0d6c14ff92E
 anon.347d264e34eb3a0c74be5a89f895ac7e.62.llvm.17695762341781453012
 _ZN40_$LT$str$u20$as$u20$core..fmt..Debug$GT$3fmt17hbca8056dc7eead37E
-_ZN4pyo35impl_16extract_argument16extract_argument17h5aa1dd28737f6df0E
 _ZN4core6result13unwrap_failed17hdff5465d74574b44E
 _ZN11parking_lot4once4Once15call_once_force28_$u7b$$u7b$closure$u7d$$u7d$17hff0123c4ecbe695bE.llvm.13238893432200692226
 _ZN14rustc_demangle12try_demangle17ha38d067f0b56e9b4E
 _ZN71_$LT$pyo3..exceptions..PyRecursionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hbc35a11eab29e87bE
 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hb63e126ce5a19bfaE
 _ZN4pyo311type_object10PyTypeInfo11type_object17h666e3307e953261aE
 _ZN70_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Display$GT$3fmt17had475fdba9668400E
-_ZN7georgio7georgio17h1b44db711282ebdbE
 _ZN4pyo35panic14PanicException18from_panic_payload17h430c4279adfc8d88E
 _ZN60_$LT$pyo3..gil..GILPool$u20$as$u20$core..ops..drop..Drop$GT$4drop17h08e135a338916b16E
 _ZN71_$LT$pyo3..exceptions..PyReferenceError$u20$as$u20$core..fmt..Debug$GT$3fmt17h901dbbe4b250cbe8E
 _ZN11parking_lot9raw_mutex8RawMutex11unlock_slow17h103fe67ba22e95e2E
 _ZN4core3ptr233drop_in_place$LT$alloc..boxed..Box$LT$dyn$u20$core..ops..function..Fn$LT$$LP$$RF$pyo3..pyclass..create_type_object..PyTypeBuilder$C$$BP$mut$u20$pyo3_ffi..cpython..object..PyTypeObject$RP$$GT$$u2b$Output$u20$$u3d$$u20$$LP$$RP$$GT$$GT$17he316ae0b535df138E.llvm.11213889763605633493
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u32$GT$3fmt17h38717ee80e1406eeE
 _ZN5alloc5alloc8box_free17h55d6234f69ffbd67E.llvm.11213889763605633493
 _ZN71_$LT$pyo3..exceptions..PyTimeoutError$u20$as$u20$core..fmt..Display$GT$3fmt17h9712959ebdfc92a3E
 _ZN4core3ptr117drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..str..error..Utf8Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hc41583d1f0be50bbE.llvm.3160907281880781123
 _ZN4pyo35panic14PanicException15type_object_raw11TYPE_OBJECT17hb4dc0203f02f3a3dE.llvm.5697929769133057476
 _ZN5alloc3ffi5c_str7CString19_from_vec_unchecked17h62597843d8fbe120E
 anon.e9eb237cf50a43b65d636b0f4770b04e.31.llvm.1386185271139027476
 _ZN70_$LT$pyo3..exceptions..PyImportWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h3e2dbfbce7a5d844E
+_ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h4c985098722996e9E.llvm.11200713541412871589
 _ZN58_$LT$T$u20$as$u20$pyo3..err..err_state..PyErrArguments$GT$9arguments17h0f0e2e9c11d38626E
 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$u64$C$pyo3..err..PyErr$GT$$GT$17h4bf2d0703230475cE.llvm.18356750485614513129
 __rust_realloc
 anon.9e114ed5010d6253bd261129473cd188.6.llvm.8364735172703476354
 _ZN3std3sys4unix2fs4stat17h0e8d201e9293885bE
 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$isize$GT$3fmt17hc7c4a8a0b43a9cb6E
 _ZN74_$LT$pyo3..exceptions..PyIsADirectoryError$u20$as$u20$core..fmt..Debug$GT$3fmt17hfd091bbda7e13da6E
 _ZN81_$LT$pyo3..exceptions..asyncio..LimitOverrunError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1f4ebc3eec972281E
 _ZN75_$LT$pyo3..exceptions..PyStopAsyncIteration$u20$as$u20$core..fmt..Debug$GT$3fmt17hc950ec3c6ea55917E
 anon.347d264e34eb3a0c74be5a89f895ac7e.2.llvm.17695762341781453012
 _ZN70_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Display$GT$3fmt17heb24a244de2c3c3fE
 _ZN4core5slice5index22slice_index_order_fail17h1f8a4ffeb1c00eb3E
 _ZN3std6thread6Thread3new17hb785c38d161c9c58E
 _ZN4core3ptr272drop_in_place$LT$lock_api..mutex..MutexGuard$LT$parking_lot..raw_mutex..RawMutex$C$$LP$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$C$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$RP$$GT$$GT$17hfae2b136a28cfc8eE.llvm.13238893432200692226
-anon.96baa08bd4660f1c11ddd83a253e848d.0.llvm.3755404211422290406
 anon.347d264e34eb3a0c74be5a89f895ac7e.10.llvm.17695762341781453012
 __rust_start_panic
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.30.llvm.18356750485614513129
 _ZN74_$LT$pyo3..exceptions..PyFileNotFoundError$u20$as$u20$core..fmt..Debug$GT$3fmt17h7d43a138ee1eb2edE
 _ZN70_$LT$pyo3..exceptions..PyOverflowError$u20$as$u20$core..fmt..Debug$GT$3fmt17hf8ba314932d8a377E
 anon.347d264e34eb3a0c74be5a89f895ac7e.5.llvm.17695762341781453012
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i64$GT$3fmt17hadac23219b3f02f1E
@@ -23219,15 +23217,14 @@
 _ZN4core3ptr65drop_in_place$LT$core..option..Option$LT$pyo3..err..PyErr$GT$$GT$17hfb4ab78da4d292adE.llvm.1386185271139027476
 _ZN4core3ptr81drop_in_place$LT$alloc..vec..Vec$LT$parking_lot_core..parking_lot..Bucket$GT$$GT$17h306dca86cce70bcbE.llvm.11926435696733617703
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i64$GT$3fmt17hbedecd2bf46d1109E
 _ZN4core3fmt5Write10write_char17hfafc9261f4a524b3E
 _ZN5gimli4read6abbrev10Attributes3new17h1b99a887e63fcf65E
 __rdl_dealloc
 _ZN4core3ptr37drop_in_place$LT$core..fmt..Error$GT$17he20cc3a68c61bb19E.llvm.13238893432200692226
-_ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17ha6ae3d8064512259E.llvm.3109625712416505353
 __rdl_alloc_zeroed
 _ZN4core7unicode12unicode_data15grapheme_extend6lookup17hd769465f95e4f17eE
 _ZN4pyo35impl_16extract_argument19FunctionDescription37missing_required_positional_arguments17h4aaab2d80d41aa06E
 _ZN65_$LT$smallvec..CollectionAllocErr$u20$as$u20$core..fmt..Debug$GT$3fmt17h348d4076a78dfa05E
 _ZN62_$LT$std..io..error..ErrorKind$u20$as$u20$core..fmt..Debug$GT$3fmt17hc0835769217bb923E
 _ZN4pyo33err5PyErr4take17h40241a7302745234E
 _ZN74_$LT$pyo3..exceptions..PyBlockingIOError$u20$as$u20$core..fmt..Display$GT$3fmt17h1617c0cce31ee381E
@@ -23245,14 +23242,15 @@
 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h8e203ea97de01bdeE
 _ZN4core9panicking13panic_display17h0e52f2d4da7fc211E.llvm.18356750485614513129
 __rust_probestack
 _ZN76_$LT$pyo3..exceptions..PyNotImplementedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6bab9bbc77f02eb0E
 _ZN4pyo311type_object10PyTypeInfo11type_object17hcd6cdfe90aaae05dE
 _ZN69_$LT$pyo3..exceptions..PyBytesWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h21116da12387d51bE
 anon.9e114ed5010d6253bd261129473cd188.1.llvm.8364735172703476354
+_ZN4pyo35impl_16extract_argument16extract_argument17h363e3443f9534907E
 __GNU_EH_FRAME_HDR
 _ZN6object3elf12ELF_NOTE_GNU17hfa4096b3f4b71b6dE
 _ZN4core3fmt3num3imp54_$LT$impl$u20$core..fmt..Display$u20$for$u20$usize$GT$3fmt17h379f79964edced29E
 _ZN4core3ptr42drop_in_place$LT$alloc..string..String$GT$17hada97ac0ee8fd35cE.llvm.5697929769133057476
 _ZN4pyo311conversions3std3num64_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$u32$GT$7extract17he39022322b8be308E
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.8.llvm.18356750485614513129
 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5flush17h1a44ae04bd6f44c0E
@@ -23266,14 +23264,15 @@
 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hefa1e3e3960d0478E.llvm.3160907281880781123
 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h4057060e368158d4E.llvm.11499977999870449161
 _ZN81_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Display$GT$3fmt17hcdf689e84d830531E
 _ZN68_$LT$pyo3..exceptions..PySystemError$u20$as$u20$core..fmt..Debug$GT$3fmt17h6548821cb49f34caE
 _ZN4core3fmt9Formatter15debug_upper_hex17h4ae5ad4f6f2aa1d0E
 _ZN80_$LT$std..io..Write..write_fmt..Adapter$LT$T$GT$$u20$as$u20$core..fmt..Write$GT$9write_str17ha9be46769c3b856fE
 _ZN73_$LT$pyo3..exceptions..PyRuntimeWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h9a6e38b075e35938E
+_ZN4pyo33err9err_state10boxed_args17h34b781837ee78ca7E
 anon.9e114ed5010d6253bd261129473cd188.2.llvm.8364735172703476354
 anon.e9136d4cc2f2bf733d592b5df8895207.2.llvm.17368754240468033560
 _ZN4pyo35types6string8PyString3new17h299959edd40321a2E
 _ZN69_$LT$core..alloc..layout..LayoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h05fc90456a37551fE
 _ZN72_$LT$$RF$str$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17h4f63cbf55da6c9bfE
 _ZN4core5slice29_$LT$impl$u20$$u5b$T$u5d$$GT$15copy_from_slice17len_mismatch_fail17h574184041027afeeE
 _ZN64_$LT$std..sys..unix..stdio..Stderr$u20$as$u20$std..io..Write$GT$5write17hbc541aca9a839525E
@@ -23292,14 +23291,15 @@
 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h3b2256eaf5b2d864E
 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.11940621367560662805
 _ZN3std3sys4unix2fs12canonicalize17hbb7a977ea3596806E
 _ZN67_$LT$pyo3..exceptions..PyEOFError$u20$as$u20$core..fmt..Display$GT$3fmt17h66301cdb51d144cdE
 anon.347d264e34eb3a0c74be5a89f895ac7e.18.llvm.17695762341781453012
 _ZN4pyo35types10typeobject6PyType4name17heeb35ac9933d480dE
 _ZN78_$LT$pyo3..exceptions..asyncio..CancelledError$u20$as$u20$core..fmt..Debug$GT$3fmt17h99a04508eedb7eb2E
+_ZN4pyo35types5tuple137_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$C$T2$C$T3$RP$$GT$7into_py17h77fc8d3e8f6025c2E
 anon.9e114ed5010d6253bd261129473cd188.3.llvm.8364735172703476354
 _ZN4core9panicking19panic_cannot_unwind17hd123d9c71473dcdaE
 _ZN57_$LT$core..fmt..Formatter$u20$as$u20$core..fmt..Write$GT$9write_str17h317c4bebb297f401E
 _ZN4pyo33err5PyErr8new_type17had5c31a5cd10e380E
 _GLOBAL_OFFSET_TABLE_
 anon.e9eb237cf50a43b65d636b0f4770b04e.32.llvm.1386185271139027476
 _ZN4pyo311type_object10PyTypeInfo11type_object17h14f5c75e7468b391E
@@ -23312,14 +23312,15 @@
 _ZN4pyo35types3any5PyAny7setattr17h6b838b67a3f86361E
 _ZN3std7process5abort17h6a5731f81d82fd63E
 _ZN5alloc4sync32arcinner_layout_for_value_layout17h29ebdaf835957654E
 _ZN3std4time7Instant3now17h7b1369cc9fc453d9E
 anon.347d264e34eb3a0c74be5a89f895ac7e.1.llvm.17695762341781453012
 _ZN3std3sys4unix17decode_error_kind17h2ad02d7078e49c10E
 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.17695762341781453012
+_ZN4pyo35types5tuple127_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$RP$$GT$7into_py17h38128205453875a5E
 _ZN69_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Display$GT$3fmt17h815d9d40959003edE
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.41.llvm.13238893432200692226
 _ZN53_$LT$T$u20$as$u20$pyo3..conversion..FromPyPointer$GT$21from_owned_ptr_or_opt17h947fb03ed62b14c7E.llvm.13238893432200692226
 _ZN71_$LT$pyo3..exceptions..PyRuntimeError$u20$as$u20$core..fmt..Display$GT$3fmt17h3b25ff331a9ad273E
 _ZN4core3ptr76drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..string..PyString$GT$$GT$17hc3397687b30d1933E.llvm.11213889763605633493
 _ZN68_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17h02adaaea9cb2e646E
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u64$GT$3fmt17h09bd8bccf6418030E
@@ -23457,26 +23458,24 @@
 _ZN66_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h025aee14bd815f41E
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.32.llvm.18356750485614513129
 _ZN5alloc5alloc8box_free17h6d60de2e8e707bddE.llvm.13238893432200692226
 _ZN84_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h43f6de0dfbfa8d59E
 _ZN75_$LT$gimli..read..abbrev..Attributes$u20$as$u20$core..ops..deref..Deref$GT$5deref17h0e97780763d5016bE
 _ZN81_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$alloc..ffi..c_str..CString..new..SpecNewImpl$GT$13spec_new_impl17hccb117dae17ea40eE
 _ZN11miniz_oxide7inflate4core17DecompressorOxide3new17hd62a62e63e49204eE
-_ZN4pyo35types5tuple137_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$C$T2$C$T3$RP$$GT$7into_py17hfbeb287d953cc89bE
 _ZN66_$LT$pyo3..exceptions..PyIOError$u20$as$u20$core..fmt..Display$GT$3fmt17h4684b863c7405c24E
 _ZN66_$LT$pyo3..exceptions..PyWarning$u20$as$u20$core..fmt..Display$GT$3fmt17hc5aab802369a5be8E
 _ZN4pyo35types3any5PyAny7getattr17hcd851db43e568513E
 _ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h2f8c1ae13caabb10E.llvm.3160907281880781123
 _ZN4core3ptr122drop_in_place$LT$alloc..vec..into_iter..IntoIter$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$17h354e65b2c3462211E.llvm.13238893432200692226
 rust_begin_unwind
 anon.5105bdd79f23b1171f38742feaac5d17.25.llvm.3160907281880781123
 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.13238893432200692226
 _ZN73_$LT$pyo3..exceptions..PyInterruptedError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb72a022a7a6bd2a9E
 _ZN74_$LT$pyo3..exceptions..PyBrokenPipeError$u20$as$u20$core..fmt..Display$GT$3fmt17h52e34d65bb49743aE
-_ZN4pyo311type_object10PyTypeInfo11type_object17h51bea979b21a7957E
 _ZN68_$LT$std..sys..unix..os_str..Slice$u20$as$u20$core..fmt..Display$GT$3fmt17h7e6fdf932a7c0d65E
 _ZN4core3ptr132drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$core..ptr..non_null..NonNull$LT$pyo3_ffi..object..PyObject$GT$$GT$$GT$$GT$17h73f0eec5bca59ab3E.llvm.18356750485614513129
 _ZN5alloc7raw_vec17capacity_overflow17h564475d43ac0e37cE
 _ZN66_$LT$pyo3..exceptions..PyOSError$u20$as$u20$core..fmt..Display$GT$3fmt17hedaa715cc53c30a3E
 _ZN3std3sys4unix5locks12futex_rwlock6RwLock14read_contended17h8d2d4f25fa7e2cffE
 _ZN4core3fmt3num3imp51_$LT$impl$u20$core..fmt..Display$u20$for$u20$u8$GT$3fmt17he4918c78216b8995E
 _ZN82_$LT$core..char..EscapeDebug$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h0ce4c5bc56d4349fE
@@ -23495,22 +23494,24 @@
 _ZN16parking_lot_core11parking_lot9HASHTABLE17h9fcd6b50658d7790E
 _ZN72_$LT$pyo3..exceptions..PyArithmeticError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8d583032932d3258E
 _ZN41_$LT$char$u20$as$u20$core..fmt..Debug$GT$3fmt17hacca1e08548532f1E
 _ZN3std9panicking11begin_panic17h7a3cef7c94e375b8E
 _ZN4core3fmt8builders11DebugStruct5field17h34ac1bbc88a79ac3E
 _ZN91_$LT$std..panicking..rust_panic_without_hook..RewrapBox$u20$as$u20$core..panic..BoxMeUp$GT$3get17hd95878c44be69298E
 _ZN3std10sys_common9backtrace26__rust_end_short_backtrace17h5152e5383956f652E
+_ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h762d1cc7c3d79729E.llvm.11901482343555561327
 _ZN4core3fmt3num52_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$u8$GT$3fmt17h61de3dd80864a2dbE
 _ZN14rustc_demangle8demangle17h18329d8ff3695e33E
 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h3e8cb9f4133f7766E
 _ZN4core3ptr69drop_in_place$LT$alloc..borrow..Cow$LT$core..ffi..c_str..CStr$GT$$GT$17h34733ae39e06fd32E.llvm.5697929769133057476
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..LowerHex$u20$for$u20$i32$GT$3fmt17h734818c8fc62ec6bE
 _ZN70_$LT$pyo3..exceptions..PyBufferError$u20$as$u20$core..fmt..Display$GT$3fmt17hf8c0e41fd4749031E
 _ZN4core3fmt8builders9DebugList6finish17h8df4dd32d6774c16E
 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h149e760258b2c034E.llvm.3160907281880781123
+_ZN4pyo311type_object10PyTypeInfo11type_object17h9481a0631b61df17E
 _ZN68_$LT$pyo3..exceptions..PyImportError$u20$as$u20$core..fmt..Debug$GT$3fmt17hb66f591c6d124ab0E
 _ZN93_$LT$std..panicking..begin_panic_handler..StrPanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$3get17hc59bdcf586fef76cE
 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$u32$GT$3fmt17he422b8199910d448E
 _ZN5gimli6common9SectionId4name17hb19ecacf465758f1E
 _ZN3std5alloc8rust_oom17hbb2cf487567423f9E
 __rg_oom
 _ZN8smallvec17SmallVec$LT$A$GT$11try_reserve17h51793078cfb5e6d8E
@@ -23533,27 +23534,25 @@
 _ZN3std3sys4unix5stdio12panic_output17h19a254038a1fde18E
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.15.llvm.18356750485614513129
 anon.682f053ba3d6d14af5b27cfcbbd16363.2.llvm.5697929769133057476
 _ZN3std6thread9yield_now17h198803acc80d4229E
 _ZN4core3fmt9Formatter26debug_struct_field2_finish17h69061813f2b8d243E
 _ZN4pyo35types8function11PyCFunction12internal_new17h535a536fc017e1c8E
 _ZN68_$LT$pyo3..types..mapping..PyMapping$u20$as$u20$core..fmt..Debug$GT$3fmt17hcc81c4d9f436318dE
-_ZN4pyo35impl_16extract_argument19FunctionDescription26extract_arguments_fastcall17hcb38e9353fbe019aE
 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h8c486a937bb733fcE.llvm.3160907281880781123
 _ZN4core9panicking18panic_bounds_check17haf06fefb23eba82dE
 _ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$7reserve21do_reserve_and_handle17ha25d0b833c1f4bc4E
 _ZN72_$LT$pyo3..exceptions..PyBrokenPipeError$u20$as$u20$core..fmt..Debug$GT$3fmt17hc70b6cd767c2469dE
 _ZN4core3fmt3num55_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$usize$GT$3fmt17h3b8df7f7743a0bc1E
 _ZN73_$LT$pyo3..exceptions..asyncio..QueueFull$u20$as$u20$core..fmt..Debug$GT$3fmt17hae16bea932a6cd3cE
 _ZN76_$LT$pyo3..exceptions..PyFileNotFoundError$u20$as$u20$core..fmt..Display$GT$3fmt17h58399bd2dcb22b7fE
 _ZN3std3env7_var_os17hca6049724bd50707E
 _ZN5alloc5slice64_$LT$impl$u20$alloc..borrow..ToOwned$u20$for$u20$$u5b$T$u5d$$GT$8to_owned17hb0cd7b91de122235E
 __rust_alloc
 _ZN53_$LT$pyo3..err..PyErr$u20$as$u20$core..fmt..Debug$GT$3fmt17h9a1a85edf39ab7abE
-_ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8e358dedbd9e16fcE.llvm.15555921300689576899
 _ZN78_$LT$pyo3..exceptions..PyUnicodeTranslateError$u20$as$u20$core..fmt..Debug$GT$3fmt17h69da6d7c377c0f25E
 _ZN72_$LT$pyo3..exceptions..PyBaseException$u20$as$u20$core..fmt..Display$GT$3fmt17h9f8a1f0450a82077E
 _ZN4core3fmt8builders10DebugTuple6finish17hea3a905db468af57E
 _ZN4core3fmt9Formatter12pad_integral17h673ca7d29b1431dbE
 _ZN70_$LT$pyo3..exceptions..PyUserWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h709d04f32567c2f1E
 _ZN90_$LT$std..panicking..begin_panic_handler..PanicPayload$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h33268f84f4c6e7f6E
 _ZN4pyo33gil9GIL_COUNT7__getit5__KEY17hbdb58542edd07274E
@@ -23561,64 +23560,65 @@
 _ZN4core3ptr54drop_in_place$LT$$RF$mut$u20$alloc..string..String$GT$17h9b72578629773643E.llvm.3041393958569974349
 _ZN4pyo311conversions3std6string68_$LT$impl$u20$pyo3..conversion..FromPyObject$u20$for$u20$$RF$str$GT$7extract17he4ff01f8fbafbcb9E
 _ZN5alloc5alloc18handle_alloc_error17h07edb87aaab24c34E
 _ZN4core3ptr70drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$17h8ceba62dbb084e8aE.llvm.3041393958569974349
 _ZN4core3ptr81drop_in_place$LT$core..option..Option$LT$pyo3..err..err_state..PyErrState$GT$$GT$17hc8079f64f31b1f10E.llvm.1386185271139027476
 anon.b4bc1e6dd908342f3bb54e6363ef7da8.20.llvm.6572068071283858929
 _ZN72_$LT$pyo3..exceptions..PyConnectionError$u20$as$u20$core..fmt..Debug$GT$3fmt17hdaa4c97d37b97a88E
+_ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hbeb0974cf65501feE.llvm.6884769035450356670
 _ZN4pyo311type_object10PyTypeInfo11type_object17h37897d217944a43aE
 _ZN69_$LT$pyo3..exceptions..PyUnicodeError$u20$as$u20$core..fmt..Debug$GT$3fmt17h97bee77a2f2873b8E
 _ZN68_$LT$pyo3..exceptions..PyException$u20$as$u20$core..fmt..Display$GT$3fmt17h366bb6713a1d10d0E
-_ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17hcc81d66abc17d19fE.llvm.3755404211422290406
 _ZN58_$LT$std..io..error..Error$u20$as$u20$core..fmt..Debug$GT$3fmt17h68dc270ae3e9c68bE
 _ZN58_$LT$alloc..string..String$u20$as$u20$core..fmt..Write$GT$10write_char17h1b6d606d1cb1d5b7E.llvm.5697929769133057476
 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h1bffbf42511ceb72E
 _ZN76_$LT$pyo3..exceptions..PyZeroDivisionError$u20$as$u20$core..fmt..Display$GT$3fmt17h9f580bf69d5e5d43E
 _ZN4core3str5lossy9Utf8Chunk7invalid17h8adfbf091f209ce8E
 _ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h51e3209cb696486cE.llvm.3160907281880781123
 _ZN68_$LT$pyo3..exceptions..PySyntaxError$u20$as$u20$core..fmt..Debug$GT$3fmt17h81c98345e8e67d0aE
 _ZN77_$LT$pyo3..exceptions..PyUnicodeDecodeError$u20$as$u20$core..fmt..Display$GT$3fmt17h21cb6c1e172b2f39E
 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h8068a05dc4515173E
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$u32$GT$3fmt17hf4a1c53fec4ddae0E
 _ZN4core3ptr92drop_in_place$LT$std..io..Write..write_fmt..Adapter$LT$std..sys..unix..stdio..Stderr$GT$$GT$17hc4a130cf0ed6b183E.llvm.8364735172703476354
-_ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h26b53fd72e755dc5E.llvm.3109625712416505353
 _ZN4core3ptr44drop_in_place$LT$core..cell..BorrowError$GT$17h2a3f9d42403f81a5E.llvm.13238893432200692226
 _ZN4core9panicking9panic_fmt17hf33a1475b4dc5c3eE
 _ZN75_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hde9ef4f8da514fa2E
 _ZN4core5panic10panic_info9PanicInfo8location17hbf5fdab53ce4ee25E
 _ZN83_$LT$parking_lot_core..parking_lot..ThreadData$u20$as$u20$core..ops..drop..Drop$GT$4drop17h2922879b2a7d20a0E
 _ZN79_$LT$pyo3..exceptions..PyConnectionAbortedError$u20$as$u20$core..fmt..Debug$GT$3fmt17h559c916dc6f13dc2E
+anon.93bf4d71f312183112856023db87c3c8.0.llvm.6884769035450356670
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.0.llvm.13238893432200692226
 _ZN3std9panicking12default_hook17ha3500da57aa4ac4fE
 _ZN3std4path4Path6is_dir17h6f11f52bef130b39E
 _ZN3std9panicking4HOOK17h7bb63a64ad501087E
 _ZN4core3ptr121drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..num..error..ParseIntError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hbb3e1eaf81b89180E.llvm.3160907281880781123
 _ZN82_$LT$pyo3..exceptions..PyPendingDeprecationWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hc4bd6dc556cbed48E
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.40.llvm.13238893432200692226
 _ZN4core3ptr48drop_in_place$LT$core..str..error..Utf8Error$GT$17h2ce34d3d0d92f30dE.llvm.17695762341781453012
+_ZN3std6thread5local4fast12Key$LT$T$GT$14try_initialize17h977ad689fd3c5283E.llvm.11200713541412871589
 _ZN4pyo311type_object10PyTypeInfo11type_object17hb04fa46bfea55216E
 _ZN6memchr6memchr3x864sse26memchr17hd182aafbd6503693E
 _ZN3std5panic19get_backtrace_style17haa81a24714daee33E
 _ZN4core3ptr47drop_in_place$LT$core..cell..BorrowMutError$GT$17hbde80eafcb7ec02bE.llvm.13238893432200692226
 _ZN98_$LT$alloc..vec..Vec$LT$T$GT$$u20$as$u20$alloc..vec..spec_from_iter..SpecFromIter$LT$T$C$I$GT$$GT$9from_iter17h1f8acbcf324ddd43E
-anon.d19f1da36be9ba6275b9cff1cbdd3d97.0.llvm.16395832583172200221
 _ZN4pyo33gil13OWNED_OBJECTS7__getit5__KEY17hbeed0358bb5e9986E
 _ZN88_$LT$std..time..Instant$u20$as$u20$core..ops..arith..Add$LT$core..time..Duration$GT$$GT$3add17h06566c3a94841a50E
 _ZN77_$LT$pyo3..exceptions..PyDeprecationWarning$u20$as$u20$core..fmt..Display$GT$3fmt17h636b6b3f321039adE
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.9.llvm.18356750485614513129
 _ZN70_$LT$pyo3..exceptions..PyLookupError$u20$as$u20$core..fmt..Display$GT$3fmt17hb55fb57d25dc6d97E
 _ZN44_$LT$$RF$T$u20$as$u20$core..fmt..Display$GT$3fmt17h387229845c3413fbE
 _ZN67_$LT$pyo3..exceptions..PyValueError$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c91d92007304598E
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.39.llvm.13238893432200692226
 _ZN3std4path4Path13_strip_prefix17h9a2ea8579314a83aE
 _ZN4core3ptr155drop_in_place$LT$parking_lot..once..Once..call_once_force$LT$pyo3..gil..GILGuard..acquire..$u7b$$u7b$closure$u7d$$u7d$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h077f002e42e272c7E.llvm.13238893432200692226
 _ZN98_$LT$alloc..string..String$u20$as$u20$core..convert..From$LT$alloc..borrow..Cow$LT$str$GT$$GT$$GT$4from17h12f8e1c107e4d81eE
 anon.e9eb237cf50a43b65d636b0f4770b04e.28.llvm.1386185271139027476
 _ZN5alloc6string6String15from_utf8_lossy17hf3c0139dbcedaff0E
 _ZN4core3ptr71drop_in_place$LT$core..result..Result$LT$i64$C$pyo3..err..PyErr$GT$$GT$17h3d326b537301a231E.llvm.18356750485614513129
+_ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17ha5a91e081dbb3ca6E.llvm.6884769035450356670
 _ZN4core7unicode12unicode_data2cc6lookup17hee9d0af768da4b93E
 _ZN75_$LT$pyo3..exceptions..PyFloatingPointError$u20$as$u20$core..fmt..Debug$GT$3fmt17haed3868103eaa2ffE
 _ZN61_$LT$pyo3..gil..GILGuard$u20$as$u20$core..ops..drop..Drop$GT$4drop17h7715afefce27b8edE
 _ZN74_$LT$pyo3..exceptions..PyZeroDivisionError$u20$as$u20$core..fmt..Debug$GT$3fmt17h28e84e86a4b46619E
 _ZN4pyo311type_object10PyTypeInfo11type_object17hc53719a37bf25210E
 _ZN4core3str5count23char_count_general_case17hea35bb248bd0d6b7E
 anon.97ad931c54c885ca96dfd72ef10ab038.13.llvm.3041393958569974349
@@ -23627,25 +23627,23 @@
 _ZN68_$LT$core..num..error..ParseIntError$u20$as$u20$core..fmt..Debug$GT$3fmt17hdeaa4371c344e8f0E
 anon.e9eb237cf50a43b65d636b0f4770b04e.51.llvm.1386185271139027476
 _ZN4core3ptr50drop_in_place$LT$alloc..borrow..Cow$LT$str$GT$$GT$17hb21c8154e58f0fc6E.llvm.1386185271139027476
 _ZN4core9panicking19assert_failed_inner17haf9816227b20b6f2E
 _ZN91_$LT$std..panicking..begin_panic..PanicPayload$LT$A$GT$$u20$as$u20$core..panic..BoxMeUp$GT$8take_box17h96f1e733775c6f71E
 _ZN3std9panicking11panic_count17is_zero_slow_path17h1c191696d45b483bE
 _ZN4core3fmt3num3imp52_$LT$impl$u20$core..fmt..Display$u20$for$u20$i32$GT$3fmt17hbd794a33ffeb7abcE
-_ZN4pyo33err9err_state10boxed_args17hddae8416b037d705E
 _ZN74_$LT$pyo3..exceptions..PyKeyboardInterrupt$u20$as$u20$core..fmt..Debug$GT$3fmt17h3cd60c245455cf6fE
 _ZN91_$LT$std..sys_common..backtrace.._print..DisplayBacktrace$u20$as$u20$core..fmt..Display$GT$3fmt17h5779d7bf7f70cb0cE
 __rust_panic_cleanup
 anon.347d264e34eb3a0c74be5a89f895ac7e.63.llvm.17695762341781453012
 _ZN64_$LT$std..sys..unix..stdio..Stdout$u20$as$u20$std..io..Write$GT$5flush17h542738ef7b7c1157E
 _ZN4pyo33err5PyErr10from_value17h7ced6e799edb8b86E
 _ZN4core3fmt9Formatter25debug_tuple_field1_finish17h67a4669c30245344E
 _ZN4pyo311conversions3std6string133_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$alloc..string..String$GT$7into_py17h41ab879c9698f20eE
 _ZN72_$LT$pyo3..exceptions..PyFileExistsError$u20$as$u20$core..fmt..Debug$GT$3fmt17he2a503da1e9e39e1E
-_ZN4core3ptr97drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$RF$str$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hc1d9325495b4a971E.llvm.3755404211422290406
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.51.llvm.13238893432200692226
 _ZN68_$LT$pyo3..exceptions..PyTypeError$u20$as$u20$core..fmt..Display$GT$3fmt17hb0aaae081fc62cbdE
 anon.9e114ed5010d6253bd261129473cd188.5.llvm.8364735172703476354
 _ZN4core3ffi5c_str4CStr6to_str17h75b7ba7fdce42660E
 _ZN4core3ptr122drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$$LP$alloc..string..String$C$$RP$$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h5348da253c5d3d92E.llvm.3160907281880781123
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.13.llvm.13238893432200692226
 _ZN70_$LT$pyo3..exceptions..PyFutureWarning$u20$as$u20$core..fmt..Debug$GT$3fmt17hb9503ca5cd1cbd79E
@@ -23709,14 +23707,15 @@
 _ZN4pyo33err5PyErr9set_cause17h30580ef7adddef0dE
 _ZN3std4path10Components7as_path17h3cc3e688e3107704E
 _ZN63_$LT$core..cell..BorrowMutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h8848bba7b89d3f8aE
 _ZN4core3fmt3num53_$LT$impl$u20$core..fmt..UpperHex$u20$for$u20$i32$GT$3fmt17hfa81d1d5a2794b7dE
 _ZN4core3ptr125drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$pyo3..err..PyDowncastErrorArguments$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h876d59fe3b130b07E.llvm.3160907281880781123
 _ZN103_$LT$std..sync..mpsc..TryRecvError$u20$as$u20$core..convert..From$LT$std..sync..mpsc..RecvError$GT$$GT$4from17hb2cf803f361b62e1E
 anon.e9eb237cf50a43b65d636b0f4770b04e.29.llvm.1386185271139027476
+anon.aa4339ca2dbb296fa63ba57d58d55e89.0.llvm.15280094018889411062
 _ZN77_$LT$pyo3..exceptions..PyNotADirectoryError$u20$as$u20$core..fmt..Display$GT$3fmt17h12984b10e0ebfe84E
 _ZN60_$LT$std..io..error..Error$u20$as$u20$core..fmt..Display$GT$3fmt17h3e34292f6cd5fc40E
 __rdl_realloc
 anon.682f053ba3d6d14af5b27cfcbbd16363.41.llvm.5697929769133057476
 _ZN4core3ptr123drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..net..parser..AddrParseError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17hac83f5491bc17d35E.llvm.3160907281880781123
 _ZN59_$LT$core..fmt..Arguments$u20$as$u20$core..fmt..Display$GT$3fmt17h4175b056ed0fab26E
 _ZN3std3sys4unix5locks12futex_rwlock6RwLock22wake_writer_or_readers17h5ba4b7f800cbd044E
@@ -23731,14 +23730,15 @@
 _ZN76_$LT$pyo3..exceptions..asyncio..TimeoutError$u20$as$u20$core..fmt..Debug$GT$3fmt17h5562d471cf41072dE
 _ZN4core3ptr78drop_in_place$LT$pyo3..instance..Py$LT$pyo3..types..typeobject..PyType$GT$$GT$17h2215d3a9b0be969cE.llvm.1386185271139027476
 _ZN4pyo35impl_16extract_argument19FunctionDescription29too_many_positional_arguments17h79543ff9496fadb6E
 _ZN72_$LT$pyo3..exceptions..PyStopIteration$u20$as$u20$core..fmt..Display$GT$3fmt17h606efbd94856db6fE
 _ZN4core3ops8function6FnOnce40call_once$u7b$$u7b$vtable.shim$u7d$$u7d$17h73e7a97655bd7fa0E.llvm.3160907281880781123
 _ZN3std2io5stdio7_eprint17h2192cf8e233cd6aaE
 _ZN77_$LT$pyo3..exceptions..PyUnicodeEncodeError$u20$as$u20$core..fmt..Display$GT$3fmt17hfa595561278bc36fE
+_ZN7georgio7georgio17h17ee84be84d4a39bE
 _ZN84_$LT$core..char..EscapeDefault$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h85f66e8546c5bd58E
 _ZN4core5panic10panic_info9PanicInfo10can_unwind17hcbb863668b6703efE
 _ZN68_$LT$core..fmt..builders..PadAdapter$u20$as$u20$core..fmt..Write$GT$9write_str17hb31c05454b680aa2E
 anon.a80902d6bb08773bf6743d023c7df73e.17.llvm.11940621367560662805
 anon.347d264e34eb3a0c74be5a89f895ac7e.15.llvm.17695762341781453012
 _ZN4core3ffi5c_str4CStr19from_bytes_with_nul17h60ba6b79363256ccE
 _ZN68_$LT$pyo3..exceptions..PyBufferError$u20$as$u20$core..fmt..Debug$GT$3fmt17h1e3fb4a30e09ed54E
@@ -23748,18 +23748,18 @@
 _ZN4pyo33gil5START17h58523f084b8fc918E.llvm.13238893432200692226
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.29.llvm.18356750485614513129
 _ZN4pyo35impl_16extract_argument19FunctionDescription27unexpected_keyword_argument17hc2ea0316549b7cb1E
 _ZN36_$LT$T$u20$as$u20$core..any..Any$GT$7type_id17h37d3081fa7e91287E
 _ZN4core3fmt9Formatter3new17hd94366d3ae6cbcdfE
 _ZN4core5panic10panic_info9PanicInfo7payload17hb3d2134487894de8E
 __rust_alloc_error_handler
+_ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h168a900aa3e0c8b8E
 _ZN4core3ptr52drop_in_place$LT$std..thread..local..AccessError$GT$17h697bd454dd3ba1fbE.llvm.18356750485614513129
 _ZN4pyo35types6string8PyString15to_string_lossy17hd99f20cf0c825b2bE
 _ZN4core3ptr119drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$alloc..string..FromUtf16Error$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h94811fe4ace74af2E.llvm.3160907281880781123
-_ZN4pyo35types5tuple127_$LT$impl$u20$pyo3..conversion..IntoPy$LT$pyo3..instance..Py$LT$pyo3..types..any..PyAny$GT$$GT$$u20$for$u20$$LP$T0$C$T1$RP$$GT$7into_py17h20a8054c1a24cbd3E
 _ZN3std2io5Write9write_fmt17hb89612cdacf175eeE
 _ZN4pyo35impl_16extract_argument19FunctionDescription33positional_only_keyword_arguments17h69d993d0b92bda9dE
 _ZN4pyo33err17panic_after_error17he7adfd3ac8d1d8acE
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.31.llvm.18356750485614513129
 _ZN5alloc11collections5btree4node10splitpoint17h36555320df7972deE
 _ZN4core3ptr91drop_in_place$LT$core..cell..RefMut$LT$alloc..vec..Vec$LT$std..thread..ThreadId$GT$$GT$$GT$17h669a854d11e215cbE.llvm.18356750485614513129
 _ZN4core3ptr37drop_in_place$LT$pyo3..err..PyErr$GT$17hbd7457b020573d1bE.llvm.1386185271139027476
@@ -23772,15 +23772,14 @@
 _ZN3std2io5Write9write_all17h0db8d772b302f00bE
 _ZN3std3sys4unix4args3imp15ARGV_INIT_ARRAY17h30412a22fc176490E
 _ZN3std3sys4unix4args3imp15ARGV_INIT_ARRAY12init_wrapper17h5ed71925f6470202E
 _ZN91_$LT$addr2line..LocationRangeUnitIter$u20$as$u20$core..iter..traits..iterator..Iterator$GT$4next17h3269ac4174d2858bE
 _ZN4core3ptr122drop_in_place$LT$pyo3..err..err_state..boxed_args$LT$core..str..error..ParseBoolError$GT$..$u7b$$u7b$closure$u7d$$u7d$$GT$17h03a7404ff8c81eb0E.llvm.3160907281880781123
 _ZN5alloc5alloc8box_free17h76061aca80fb3990E.llvm.11236572853509692416
 _ZN5adler7Adler3211write_slice17he2404f6f27d2ef09E
-_ZN5alloc7raw_vec19RawVec$LT$T$C$A$GT$16reserve_for_push17h8abd4168aa07edd0E
 _ZN4pyo35types3any5PyAny7setattr17h4aeef81d02f8b7faE
 _ZN79_$LT$std..backtrace_rs..symbolize..SymbolName$u20$as$u20$core..fmt..Display$GT$3fmt17h434acb7722c3decbE
 _ZN68_$LT$$RF$$u5b$u8$u5d$$u20$as$u20$object..read..read_ref..ReadRef$GT$19read_bytes_at_until17h170b4060dbcae77aE
 _ZN4core3str5lossy9Utf8Chunk5valid17h15d1e98cc145018bE
 _ZN81_$LT$pyo3..exceptions..PyConnectionRefusedError$u20$as$u20$core..fmt..Display$GT$3fmt17haa4f80e697d069f4E
 _ZN4core5slice5index26slice_start_index_len_fail17h6bee405bac6d3d26E
 anon.7b946ae1d3a666797e2db1f36e4cd6e7.34.llvm.18356750485614513129
@@ -23792,14 +23791,15 @@
 _ZN75_$LT$pyo3..exceptions..PyInterruptedError$u20$as$u20$core..fmt..Display$GT$3fmt17hf7a2d4ade099865dE
 _ZN4core3fmt17pointer_fmt_inner17h97b13a612a80a456E
 anon.347d264e34eb3a0c74be5a89f895ac7e.64.llvm.17695762341781453012
 _ZN93_$LT$alloc..collections..btree..mem..replace..PanicGuard$u20$as$u20$core..ops..drop..Drop$GT$4drop17h4183f132fb648b0aE
 _ZN42_$LT$$RF$T$u20$as$u20$core..fmt..Debug$GT$3fmt17h4c580bc7d680b708E
 anon.b9a0486c00a4172b7b1ac52b315aa4a3.35.llvm.13238893432200692226
 anon.347d264e34eb3a0c74be5a89f895ac7e.8.llvm.17695762341781453012
+_ZN4pyo35impl_16extract_argument19FunctionDescription26extract_arguments_fastcall17hf57c52c8f64057f8E
 _ZN4core3num21_$LT$impl$u20$u32$GT$14from_str_radix17h2d973af03c66c62bE
 PyExc_BaseException
 PyExc_ImportError
 pthread_getspecific@@GLIBC_2.2.5
 sincosf@@GLIBC_2.2.5
 PyUnicode_AsEncodedString
 _Unwind_GetRegionStart@@GCC_3.0
```

### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -5445,29 +5445,29 @@
 	je     c6ac <pyo3::impl_::trampoline::trampoline_inner+0x3c>
 	add    $0x8,%rax
 	jmp    c6c6 <pyo3::impl_::trampoline::trampoline_inner+0x56>
 	data16 lea 0x5952c(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	mov    %rax,%rdi
 	xor    %esi,%esi
-	call   ecb0 <std::thread::local::fast::Key<T>::try_initialize>
+	call   ed80 <std::thread::local::fast::Key<T>::try_initialize>
 	incq   (%rax)
 	lea    0x599b0(%rip),%rdi        
 	call   *0x597e2(%rip)        
 	data16 lea 0x595aa(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	cmpq   $0x0,(%rax)
 	je     c6f2 <pyo3::impl_::trampoline::trampoline_inner+0x82>
 	add    $0x8,%rax
 	jmp    c715 <pyo3::impl_::trampoline::trampoline_inner+0xa5>
 	data16 lea 0x5958e(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	mov    %rax,%rdi
 	xor    %esi,%esi
-	call   ecf0 <std::thread::local::fast::Key<T>::try_initialize>
+	call   ecb0 <std::thread::local::fast::Key<T>::try_initialize>
 	test   %rax,%rax
 	je     c799 <pyo3::impl_::trampoline::trampoline_inner+0x129>
 	movabs $0x7fffffffffffffff,%rcx
 	cmp    %rcx,(%rax)
 	jae    c79d <pyo3::impl_::trampoline::trampoline_inner+0x12d>
 	mov    0x18(%rax),%rcx
 	mov    $0x1,%edx
@@ -7398,29 +7398,29 @@
 	je     eae9 <PyInit_georgio+0x39>
 	add    $0x8,%rax
 	jmp    eb03 <PyInit_georgio+0x53>
 	data16 lea 0x570ef(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	mov    %rax,%rdi
 	xor    %esi,%esi
-	call   ecb0 <std::thread::local::fast::Key<T>::try_initialize>
+	call   ed80 <std::thread::local::fast::Key<T>::try_initialize>
 	incq   (%rax)
 	lea    0x57573(%rip),%rdi        
 	call   *0x573a5(%rip)        
 	data16 lea 0x5716d(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	cmpq   $0x0,(%rax)
 	je     eb2f <PyInit_georgio+0x7f>
 	add    $0x8,%rax
 	jmp    eb52 <PyInit_georgio+0xa2>
 	data16 lea 0x57151(%rip),%rdi        
 	data16 data16 rex.W call 8060 <__tls_get_addr@plt>
 	mov    %rax,%rdi
 	xor    %esi,%esi
-	call   ecf0 <std::thread::local::fast::Key<T>::try_initialize>
+	call   ecb0 <std::thread::local::fast::Key<T>::try_initialize>
 	test   %rax,%rax
 	je     ec30 <PyInit_georgio+0x180>
 	movabs $0x7fffffffffffffff,%rcx
 	cmp    %rcx,(%rax)
 	jae    ec37 <PyInit_georgio+0x187>
 	mov    0x18(%rax),%rcx
 	mov    $0x1,%edx
@@ -7489,92 +7489,92 @@
 	ud2
 	call   *0x56b97(%rip)        
 	ud2
 	nopl   0x0(%rax,%rax,1)
 
 000000000000ecb0 <std::thread::local::fast::Key<T>::try_initialize>:
 std::thread::local::fast::Key<T>::try_initialize:
-	test   %rsi,%rsi
-	je     ecd9 <std::thread::local::fast::Key<T>::try_initialize+0x29>
-	mov    (%rsi),%rax
-	movq   $0x0,(%rsi)
-	cmp    $0x1,%rax
-	jne    ecd9 <std::thread::local::fast::Key<T>::try_initialize+0x29>
-	mov    0x8(%rsi),%rcx
-	lea    0x8(%rdi),%rax
-	movq   $0x1,(%rdi)
-	mov    %rcx,0x8(%rdi)
-	ret
-	xor    %ecx,%ecx
-	lea    0x8(%rdi),%rax
-	movq   $0x1,(%rdi)
-	mov    %rcx,0x8(%rdi)
-	ret
-	nopl   0x0(%rax,%rax,1)
-
-000000000000ecf0 <std::thread::local::fast::Key<T>::try_initialize>:
-std::thread::local::fast::Key<T>::try_initialize:
 	push   %r14
 	push   %rbx
 	push   %rax
 	mov    %rsi,%r14
 	mov    %rdi,%rbx
 	movzbl 0x28(%rdi),%eax
 	test   %rax,%rax
-	je     ed10 <std::thread::local::fast::Key<T>::try_initialize+0x20>
+	je     ecd0 <std::thread::local::fast::Key<T>::try_initialize+0x20>
 	cmp    $0x1,%eax
-	je     ed24 <std::thread::local::fast::Key<T>::try_initialize+0x34>
+	je     ece4 <std::thread::local::fast::Key<T>::try_initialize+0x34>
 	xor    %r14d,%r14d
-	jmp    ed9f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
-	lea    0xa9(%rip),%rsi        
+	jmp    ed5f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
+	lea    0xe9(%rip),%rsi        
 	mov    %rbx,%rdi
-	call   *0x56e50(%rip)        
+	call   *0x56e90(%rip)        
 	movb   $0x1,0x28(%rbx)
 	test   %r14,%r14
-	je     ed48 <std::thread::local::fast::Key<T>::try_initialize+0x58>
+	je     ed08 <std::thread::local::fast::Key<T>::try_initialize+0x58>
 	mov    (%r14),%rax
 	movq   $0x0,(%r14)
 	cmp    $0x1,%rax
-	jne    ed48 <std::thread::local::fast::Key<T>::try_initialize+0x58>
+	jne    ed08 <std::thread::local::fast::Key<T>::try_initialize+0x58>
 	movups 0x8(%r14),%xmm0
 	mov    0x18(%r14),%rax
 	mov    0x20(%r14),%rcx
-	jmp    ed66 <std::thread::local::fast::Key<T>::try_initialize+0x76>
+	jmp    ed26 <std::thread::local::fast::Key<T>::try_initialize+0x76>
 	mov    $0x800,%edi
 	mov    $0x8,%esi
-	call   *0x56e70(%rip)        
+	call   *0x56eb0(%rip)        
 	test   %rax,%rax
-	je     edaa <std::thread::local::fast::Key<T>::try_initialize+0xba>
-	movaps 0x3f45c(%rip),%xmm0        
+	je     ed6a <std::thread::local::fast::Key<T>::try_initialize+0xba>
+	movaps 0x3f49c(%rip),%xmm0        
 	xor    %ecx,%ecx
 	lea    0x8(%rbx),%r14
 	mov    0x10(%rbx),%rsi
 	mov    0x18(%rbx),%rdi
 	cmpq   $0x0,(%rbx)
 	movq   $0x1,(%rbx)
 	movups %xmm0,0x8(%rbx)
 	mov    %rax,0x18(%rbx)
 	mov    %rcx,0x20(%rbx)
-	je     ed9f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
+	je     ed5f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
 	test   %rsi,%rsi
-	je     ed9f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
+	je     ed5f <std::thread::local::fast::Key<T>::try_initialize+0xaf>
 	shl    $0x3,%rsi
 	mov    $0x8,%edx
-	call   *0x56b91(%rip)        
+	call   *0x56bd1(%rip)        
 	mov    %r14,%rax
 	add    $0x8,%rsp
 	pop    %rbx
 	pop    %r14
 	ret
 	mov    $0x800,%edi
 	mov    $0x8,%esi
-	call   *0x56e46(%rip)        
+	call   *0x56e86(%rip)        
 	ud2
 	nopl   0x0(%rax)
 
+000000000000ed80 <std::thread::local::fast::Key<T>::try_initialize>:
+std::thread::local::fast::Key<T>::try_initialize:
+	test   %rsi,%rsi
+	je     eda9 <std::thread::local::fast::Key<T>::try_initialize+0x29>
+	mov    (%rsi),%rax
+	movq   $0x0,(%rsi)
+	cmp    $0x1,%rax
+	jne    eda9 <std::thread::local::fast::Key<T>::try_initialize+0x29>
+	mov    0x8(%rsi),%rcx
+	lea    0x8(%rdi),%rax
+	movq   $0x1,(%rdi)
+	mov    %rcx,0x8(%rdi)
+	ret
+	xor    %ecx,%ecx
+	lea    0x8(%rdi),%rax
+	movq   $0x1,(%rdi)
+	mov    %rcx,0x8(%rdi)
+	ret
+	nopl   0x0(%rax,%rax,1)
+
 000000000000edc0 <std::thread::local::fast::destroy_value>:
 std::thread::local::fast::destroy_value:
 	mov    %rdi,%rax
 	mov    0x10(%rdi),%rsi
 	mov    0x18(%rdi),%rdi
 	cmpq   $0x0,(%rax)
 	movq   $0x0,(%rax)
```

### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -44,16 +44,16 @@
   0x000544b0 0c1d0000 c09bfbff 241d0000 709efbff ........$...p...
   0x000544c0 6c1d0000 e09efbff 841d0000 c0a3fbff l...............
   0x000544d0 cc1d0000 60a6fbff 481e0000 f0a6fbff ....`...H.......
   0x000544e0 781e0000 c0a7fbff b01e0000 e0a7fbff x...............
   0x000544f0 c81e0000 f0a7fbff dc1e0000 10a8fbff ................
   0x00054500 f81e0000 60a8fbff 281f0000 70a8fbff ....`...(...p...
   0x00054510 3c1f0000 80a8fbff 501f0000 90a8fbff <.......P.......
-  0x00054520 641f0000 90aafbff 901f0000 d0aafbff d...............
-  0x00054530 a41f0000 a0abfbff d01f0000 e0abfbff ................
+  0x00054520 641f0000 90aafbff 901f0000 60abfbff d...........`...
+  0x00054530 bc1f0000 a0abfbff d01f0000 e0abfbff ................
   0x00054540 e81f0000 f0abfbff 80200000 50acfbff ......... ..P...
   0x00054550 bc200000 b0adfbff fc1f0000 d0adfbff . ..............
   0x00054560 10200000 e0adfbff 24200000 f0adfbff . ......$ ......
   0x00054570 38200000 80aefbff 20210000 50b6fbff 8 ...... !..P...
   0x00054580 6c200000 60b6fbff 78210000 70b6fbff l ..`...x!..p...
   0x00054590 8c210000 00b7fbff b4210000 d0b7fbff .!.......!......
   0x000545a0 e8210000 e0b7fbff fc210000 f0b7fbff .!.......!......
```

### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -77,19 +77,19 @@
   0x00056138 18410e10 420e0841 0e200000 00000000 .A..B..A. ......
   0x00056148 10000000 b4040000 3089fbff 06000000 ........0.......
   0x00056158 00000000 10000000 c8040000 2c89fbff ............,...
   0x00056168 01000000 00000000 10000000 dc040000 ................
   0x00056178 2889fbff 06000000 00000000 28000000 (...........(...
   0x00056188 70010000 2489fbff fb010000 04ef8b00 p...$...........
   0x00056198 00410e10 470ec001 83020376 010e1041 .A..G......v...A
-  0x000561a8 0e08410e c0010000 10000000 1c050000 ..A.............
-  0x000561b8 f88afbff 3b000000 00000000 28000000 ....;.......(...
-  0x000561c8 30050000 248bfbff cc000000 00420e10 0...$........B..
-  0x000561d8 410e1841 0e208303 8e0202b2 0e18410e A..A. ........A.
-  0x000561e8 10420e08 410e2000 14000000 5c050000 .B..A. .....\...
+  0x000561a8 0e08410e c0010000 28000000 1c050000 ..A.....(.......
+  0x000561b8 f88afbff cc000000 00420e10 410e1841 .........B..A..A
+  0x000561c8 0e208303 8e0202b2 0e18410e 10420e08 . ........A..B..
+  0x000561d8 410e2000 10000000 48050000 9c8bfbff A. .....H.......
+  0x000561e8 3b000000 00000000 14000000 5c050000 ;...........\...
   0x000561f8 c88bfbff 31000000 00000000 00000000 ....1...........
   0x00056208 10000000 74050000 f08bfbff 0c000000 ....t...........
   0x00056218 00000000 10000000 88050000 ac8dfbff ................
   0x00056228 1e000000 00000000 10000000 9c050000 ................
   0x00056238 b88dfbff 10000000 00000000 10000000 ................
   0x00056248 b0050000 b48dfbff 06000000 00000000 ................
   0x00056258 30000000 c4050000 b08dfbff 86000000 0...............
```

### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -2262,159 +2262,159 @@
   0x00008d30 6573005f 5f646f5f 676c6f62 616c5f64 es.__do_global_d
   0x00008d40 746f7273 5f617578 00636f6d 706c6574 tors_aux.complet
   0x00008d50 65642e30 005f5f64 6f5f676c 6f62616c ed.0.__do_global
   0x00008d60 5f64746f 72735f61 75785f66 696e695f _dtors_aux_fini_
   0x00008d70 61727261 795f656e 74727900 6672616d array_entry.fram
   0x00008d80 655f6475 6d6d7900 5f5f6672 616d655f e_dummy.__frame_
   0x00008d90 64756d6d 795f696e 69745f61 72726179 dummy_init_array
-  0x00008da0 5f656e74 72790067 656f7267 696f2e31 _entry.georgio.1
-  0x00008db0 39613039 3336632d 6367752e 30005f5a 9a0936c-cgu.0._Z
+  0x00008da0 5f656e74 72790067 656f7267 696f2e66 _entry.georgio.f
+  0x00008db0 31613639 3965342d 6367752e 30005f5a 1a699e4-cgu.0._Z
   0x00008dc0 4e34636f 72653370 74723339 64726f70 N4core3ptr39drop
   0x00008dd0 5f696e5f 706c6163 65244c54 2470796f _in_place$LT$pyo
   0x00008de0 332e2e67 696c2e2e 47494c50 6f6f6c24 3..gil..GILPool$
-  0x00008df0 47542431 37686439 37396630 66383534 GT$17hd979f0f854
-  0x00008e00 66626565 65364500 5f5a4e34 636f7265 fbeee6E._ZN4core
+  0x00008df0 47542431 37683630 36346533 37383638 GT$17h6064e37868
+  0x00008e00 37326633 34664500 5f5a4e34 636f7265 72f34fE._ZN4core
   0x00008e10 33707472 34346472 6f705f69 6e5f706c 3ptr44drop_in_pl
   0x00008e20 61636524 4c542463 6f72652e 2e63656c ace$LT$core..cel
   0x00008e30 6c2e2e42 6f72726f 77457272 6f722447 l..BorrowError$G
-  0x00008e40 54243137 68646331 31383961 39653566 T$17hdc1189a9e5f
-  0x00008e50 38363764 3045005f 5a4e3463 6f726533 867d0E._ZN4core3
+  0x00008e40 54243137 68313636 63653837 63626230 T$17h166ce87cbb0
+  0x00008e50 37333161 3645005f 5a4e3463 6f726533 731a6E._ZN4core3
   0x00008e60 70747235 3064726f 705f696e 5f706c61 ptr50drop_in_pla
   0x00008e70 6365244c 54247079 6f332e2e 696d706c ce$LT$pyo3..impl
   0x00008e80 5f2e2e70 616e6963 2e2e5061 6e696354 _..panic..PanicT
-  0x00008e90 72617024 47542431 37683662 61326431 rap$GT$17h6ba2d1
-  0x00008ea0 30343863 36346561 38634500 5f5a4e34 048c64ea8cE._ZN4
+  0x00008e90 72617024 47542431 37683465 30356262 rap$GT$17h4e05bb
+  0x00008ea0 31646531 30643261 32654500 5f5a4e34 1de10d2a2eE._ZN4
   0x00008eb0 70796f33 35696d70 6c5f3130 7472616d pyo35impl_10tram
   0x00008ec0 706f6c69 6e653136 7472616d 706f6c69 poline16trampoli
-  0x00008ed0 6e655f69 6e6e6572 31376862 61316130 ne_inner17hba1a0
-  0x00008ee0 36346133 30393765 63353845 005f5a4e 64a3097ec58E._ZN
+  0x00008ed0 6e655f69 6e6e6572 31376865 33323435 ne_inner17he3245
+  0x00008ee0 33363761 33353935 34303645 005f5a4e 367a3595406E._ZN
   0x00008ef0 3767656f 7267696f 33336772 6561745f 7georgio33great_
   0x00008f00 63697263 6c655f64 69737461 6e63655f circle_distance_
-  0x00008f10 77697468 5f726164 69757331 37686331 with_radius17hc1
-  0x00008f20 34353230 32303931 61343835 37664500 45202091a4857fE.
+  0x00008f10 77697468 5f726164 69757331 37683864 with_radius17h8d
+  0x00008f20 32303461 62613839 33343034 38304500 204aba89340480E.
   0x00008f30 5f5a4e37 67656f72 67696f31 5f36395f _ZN7georgio1_69_
   0x00008f40 244c5424 696d706c 24753230 2467656f $LT$impl$u20$geo
   0x00008f50 7267696f 2e2e6772 6561745f 63697263 rgio..great_circ
   0x00008f60 6c655f64 69737461 6e63655f 77697468 le_distance_with
   0x00008f70 5f726164 6975732e 2e4d616b 65446566 _radius..MakeDef
   0x00008f80 24475424 33444546 31307472 616d706f $GT$3DEF10trampo
-  0x00008f90 6c696e65 31376866 34366333 34303438 line17hf46c34048
-  0x00008fa0 34333764 65383545 005f5a4e 3767656f 437de85E._ZN7geo
+  0x00008f90 6c696e65 31376834 61323031 64346533 line17h4a201d4e3
+  0x00008fa0 31376361 39333745 005f5a4e 3767656f 17ca937E._ZN7geo
   0x00008fb0 7267696f 315f3436 5f5f7079 66756e63 rgio1_46__pyfunc
   0x00008fc0 74696f6e 5f677265 61745f63 6972636c tion_great_circl
   0x00008fd0 655f6469 7374616e 63655f77 6974685f e_distance_with_
-  0x00008fe0 72616469 75733137 68356461 36646136 radius17h5da6da6
-  0x00008ff0 31396666 63396239 6545005f 5a4e3767 19ffc9b9eE._ZN7g
+  0x00008fe0 72616469 75733137 68326537 35666633 radius17h2e75ff3
+  0x00008ff0 33623465 35333832 6545005f 5a4e3767 3b4e5382eE._ZN7g
   0x00009000 656f7267 696f315f 35375f24 4c542469 eorgio1_57_$LT$i
   0x00009010 6d706c24 75323024 67656f72 67696f2e mpl$u20$georgio.
   0x00009020 2e677265 61745f63 6972636c 655f6469 .great_circle_di
   0x00009030 7374616e 63652e2e 4d616b65 44656624 stance..MakeDef$
   0x00009040 47542433 44454631 30747261 6d706f6c GT$3DEF10trampol
-  0x00009050 696e6531 37683364 37303736 31626634 ine17h3d70761bf4
-  0x00009060 36633162 64654500 5f5a4e37 67656f72 6c1bdeE._ZN7geor
+  0x00009050 696e6531 37683461 33343134 64613536 ine17h4a3414da56
+  0x00009060 31633230 39664500 5f5a4e37 67656f72 1c209fE._ZN7geor
   0x00009070 67696f31 5f33345f 5f707966 756e6374 gio1_34__pyfunct
   0x00009080 696f6e5f 67726561 745f6369 72636c65 ion_great_circle
-  0x00009090 5f646973 74616e63 65313768 35633930 _distance17h5c90
-  0x000090a0 62636532 35616539 30336232 45005f5a bce25ae903b2E._Z
+  0x00009090 5f646973 74616e63 65313768 63666534 _distance17hcfe4
+  0x000090a0 38633832 33366130 33323835 45005f5a 8c8236a03285E._Z
   0x000090b0 4e376765 6f726769 6f32376c 696e655f N7georgio27line_
   0x000090c0 6f665f62 65617269 6e675f77 6974685f of_bearing_with_
-  0x000090d0 72616469 75733137 68323864 65636633 radius17h28decf3
-  0x000090e0 66386433 39326632 6345005f 5a4e3767 f8d392f2cE._ZN7g
+  0x000090d0 72616469 75733137 68303939 35393338 radius17h0995938
+  0x000090e0 65323636 61333036 3945005f 5a4e3767 e266a3069E._ZN7g
   0x000090f0 656f7267 696f315f 36335f24 4c542469 eorgio1_63_$LT$i
   0x00009100 6d706c24 75323024 67656f72 67696f2e mpl$u20$georgio.
   0x00009110 2e6c696e 655f6f66 5f626561 72696e67 .line_of_bearing
   0x00009120 5f776974 685f7261 64697573 2e2e4d61 _with_radius..Ma
   0x00009130 6b654465 66244754 24334445 46313074 keDef$GT$3DEF10t
-  0x00009140 72616d70 6f6c696e 65313768 38353262 rampoline17h852b
-  0x00009150 64306632 61383464 33313035 45005f5a d0f2a84d3105E._Z
+  0x00009140 72616d70 6f6c696e 65313768 39346534 rampoline17h94e4
+  0x00009150 66316330 35636265 39376266 45005f5a f1c05cbe97bfE._Z
   0x00009160 4e376765 6f726769 6f315f34 305f5f70 N7georgio1_40__p
   0x00009170 7966756e 6374696f 6e5f6c69 6e655f6f yfunction_line_o
   0x00009180 665f6265 6172696e 675f7769 74685f72 f_bearing_with_r
-  0x00009190 61646975 73313768 34666164 39356362 adius17h4fad95cb
-  0x000091a0 37333639 66653936 45005f5a 4e376765 7369fe96E._ZN7ge
+  0x00009190 61646975 73313768 61323532 30396336 adius17ha25209c6
+  0x000091a0 38313230 34313433 45005f5a 4e376765 81204143E._ZN7ge
   0x000091b0 6f726769 6f315f35 315f244c 5424696d orgio1_51_$LT$im
   0x000091c0 706c2475 32302467 656f7267 696f2e2e pl$u20$georgio..
   0x000091d0 6c696e65 5f6f665f 62656172 696e672e line_of_bearing.
   0x000091e0 2e4d616b 65446566 24475424 33444546 .MakeDef$GT$3DEF
-  0x000091f0 31307472 616d706f 6c696e65 31376861 10trampoline17ha
-  0x00009200 35333938 66343433 65623661 31643745 5398f443eb6a1d7E
+  0x000091f0 31307472 616d706f 6c696e65 31376865 10trampoline17he
+  0x00009200 37336634 66343565 66343332 63303045 73f4f45ef432c00E
   0x00009210 005f5a4e 3767656f 7267696f 315f3238 ._ZN7georgio1_28
   0x00009220 5f5f7079 66756e63 74696f6e 5f6c696e __pyfunction_lin
-  0x00009230 655f6f66 5f626561 72696e67 31376835 e_of_bearing17h5
-  0x00009240 64396333 38363064 64626463 36356245 d9c3860ddbdc65bE
+  0x00009230 655f6f66 5f626561 72696e67 31376834 e_of_bearing17h4
+  0x00009240 62656632 31353539 34373261 37353545 bef21559472a755E
   0x00009250 005f5a4e 3767656f 7267696f 315f3538 ._ZN7georgio1_58
   0x00009260 5f244c54 24696d70 6c247532 30246765 _$LT$impl$u20$ge
   0x00009270 6f726769 6f2e2e62 6f756e64 696e675f orgio..bounding_
   0x00009280 626f785f 666f725f 706f696e 742e2e4d box_for_point..M
   0x00009290 616b6544 65662447 54243344 45463130 akeDef$GT$3DEF10
-  0x000092a0 7472616d 706f6c69 6e653137 68336132 trampoline17h3a2
-  0x000092b0 62613066 32616130 32313030 6145005f ba0f2aa02100aE._
+  0x000092a0 7472616d 706f6c69 6e653137 68663963 trampoline17hf9c
+  0x000092b0 31646466 34336332 35613861 3245005f 1ddf43c25a8a2E._
   0x000092c0 5a4e3767 656f7267 696f315f 33355f5f ZN7georgio1_35__
   0x000092d0 70796675 6e637469 6f6e5f62 6f756e64 pyfunction_bound
   0x000092e0 696e675f 626f785f 666f725f 706f696e ing_box_for_poin
-  0x000092f0 74313768 32623338 35373833 62633636 t17h2b385783bc66
-  0x00009300 31633336 45005f5a 4e376765 6f726769 1c36E._ZN7georgi
+  0x000092f0 74313768 63353036 33353731 34653939 t17hc50635714e99
+  0x00009300 65313733 45005f5a 4e376765 6f726769 e173E._ZN7georgi
   0x00009310 6f315f34 395f244c 5424696d 706c2475 o1_49_$LT$impl$u
   0x00009320 32302467 656f7267 696f2e2e 776d5f75 20$georgio..wm_u
   0x00009330 70706572 5f6c6566 742e2e4d 616b6544 pper_left..MakeD
   0x00009340 65662447 54243344 45463130 7472616d ef$GT$3DEF10tram
-  0x00009350 706f6c69 6e653137 68326263 33653263 poline17h2bc3e2c
-  0x00009360 38356639 31646334 3245005f 5a4e3767 85f91dc42E._ZN7g
+  0x00009350 706f6c69 6e653137 68623131 37666633 poline17hb117ff3
+  0x00009360 65323862 38373530 6145005f 5a4e3767 e28b8750aE._ZN7g
   0x00009370 656f7267 696f315f 32365f5f 70796675 eorgio1_26__pyfu
   0x00009380 6e637469 6f6e5f77 6d5f7570 7065725f nction_wm_upper_
-  0x00009390 6c656674 31376836 37386334 61643561 left17h678c4ad5a
-  0x000093a0 65623932 37656545 005f5a4e 3767656f eb927eeE._ZN7geo
+  0x00009390 6c656674 31376864 30306266 66353231 left17hd00bff521
+  0x000093a0 36656236 61393945 005f5a4e 3767656f 6eb6a99E._ZN7geo
   0x000093b0 7267696f 315f3435 5f244c54 24696d70 rgio1_45_$LT$imp
   0x000093c0 6c247532 30246765 6f726769 6f2e2e77 l$u20$georgio..w
   0x000093d0 6d5f626f 756e6473 2e2e4d61 6b654465 m_bounds..MakeDe
   0x000093e0 66244754 24334445 46313074 72616d70 f$GT$3DEF10tramp
-  0x000093f0 6f6c696e 65313768 35313237 39623731 oline17h51279b71
-  0x00009400 31653866 32333964 45005f5a 4e376765 1e8f239dE._ZN7ge
+  0x000093f0 6f6c696e 65313768 61313530 65343235 oline17ha150e425
+  0x00009400 64363861 35313763 45005f5a 4e376765 d68a517cE._ZN7ge
   0x00009410 6f726769 6f315f32 325f5f70 7966756e orgio1_22__pyfun
   0x00009420 6374696f 6e5f776d 5f626f75 6e647331 ction_wm_bounds1
-  0x00009430 37686135 30643236 66663734 37373163 7ha50d26ff74771c
-  0x00009440 35354500 5f5a4e37 67656f72 67696f31 55E._ZN7georgio1
+  0x00009430 37683161 37306638 38643134 38366666 7h1a70f88d1486ff
+  0x00009440 39314500 5f5a4e37 67656f72 67696f31 91E._ZN7georgio1
   0x00009450 5f35375f 244c5424 696d706c 24753230 _57_$LT$impl$u20
   0x00009460 2467656f 7267696f 2e2e776d 5f74696c $georgio..wm_til
   0x00009470 655f6578 70616e64 65645f62 626f782e e_expanded_bbox.
   0x00009480 2e4d616b 65446566 24475424 33444546 .MakeDef$GT$3DEF
-  0x00009490 31307472 616d706f 6c696e65 31376836 10trampoline17h6
-  0x000094a0 62373338 33303339 30383063 64643545 b7383039080cdd5E
+  0x00009490 31307472 616d706f 6c696e65 31376863 10trampoline17hc
+  0x000094a0 35386465 33326238 34313764 62616445 58de32b8417dbadE
   0x000094b0 005f5a4e 3767656f 7267696f 315f3334 ._ZN7georgio1_34
   0x000094c0 5f5f7079 66756e63 74696f6e 5f776d5f __pyfunction_wm_
   0x000094d0 74696c65 5f657870 616e6465 645f6262 tile_expanded_bb
-  0x000094e0 6f783137 68643339 62623665 63643134 ox17hd39bb6ecd14
-  0x000094f0 36646639 61450067 656f7267 696f2e31 6df9aE.georgio.1
-  0x00009500 39613039 3336632d 6367752e 31005f5a 9a0936c-cgu.1._Z
+  0x000094e0 6f783137 68346262 61643238 66373032 ox17h4bbad28f702
+  0x000094f0 39633936 36450067 656f7267 696f2e66 9c966E.georgio.f
+  0x00009500 31613639 3965342d 6367752e 31005f5a 1a699e4-cgu.1._Z
   0x00009510 4e35616c 6c6f6337 7261775f 76656331 N5alloc7raw_vec1
-  0x00009520 3166696e 6973685f 67726f77 31376830 1finish_grow17h0
-  0x00009530 66303638 30633537 31613662 66356345 f0680c571a6bf5cE
-  0x00009540 0067656f 7267696f 2e313961 30393336 .georgio.19a0936
-  0x00009550 632d6367 752e3132 0067656f 7267696f c-cgu.12.georgio
-  0x00009560 2e313961 30393336 632d6367 752e3135 .19a0936c-cgu.15
+  0x00009520 3166696e 6973685f 67726f77 31376838 1finish_grow17h8
+  0x00009530 65363530 31666463 63343134 64626445 e6501fdcc414dbdE
+  0x00009540 0067656f 7267696f 2e663161 36393965 .georgio.f1a699e
+  0x00009550 342d6367 752e3132 0067656f 7267696f 4-cgu.12.georgio
+  0x00009560 2e663161 36393965 342d6367 752e3135 .f1a699e4-cgu.15
   0x00009570 005f5a4e 3767656f 7267696f 3767656f ._ZN7georgio7geo
-  0x00009580 7267696f 33444546 31376835 39636536 rgio3DEF17h59ce6
-  0x00009590 34343030 38333637 61303045 00474343 44008367a00E.GCC
+  0x00009580 7267696f 33444546 31376839 36363064 rgio3DEF17h9660d
+  0x00009590 33653235 64663637 30613445 00474343 3e25df670a4E.GCC
   0x000095a0 5f657863 6570745f 7461626c 65313700 _except_table17.
-  0x000095b0 67656f72 67696f2e 31396130 39333663 georgio.19a0936c
+  0x000095b0 67656f72 67696f2e 66316136 39396534 georgio.f1a699e4
   0x000095c0 2d636775 2e32005f 5a4e3373 74643674 -cgu.2._ZN3std6t
   0x000095d0 68726561 64356c6f 63616c34 66617374 hread5local4fast
   0x000095e0 31336465 7374726f 795f7661 6c756531 13destroy_value1
-  0x000095f0 37683765 33393039 64343733 65393931 7h7e3909d473e991
-  0x00009600 31374500 67656f72 67696f2e 31396130 17E.georgio.19a0
-  0x00009610 39333663 2d636775 2e33005f 5a4e3463 936c-cgu.3._ZN4c
+  0x000095f0 37683661 65386135 64353139 66646439 7h6ae8a5d519fdd9
+  0x00009600 66314500 67656f72 67696f2e 66316136 f1E.georgio.f1a6
+  0x00009610 39396534 2d636775 2e33005f 5a4e3463 99e4-cgu.3._ZN4c
   0x00009620 6f726533 70747231 31306472 6f705f69 ore3ptr110drop_i
   0x00009630 6e5f706c 61636524 4c542463 6f72652e n_place$LT$core.
   0x00009640 2e6f7074 696f6e2e 2e4f7074 696f6e24 .option..Option$
   0x00009650 4c542470 796f332e 2e696e73 74616e63 LT$pyo3..instanc
   0x00009660 652e2e50 79244c54 2470796f 332e2e74 e..Py$LT$pyo3..t
   0x00009670 79706573 2e2e7472 61636562 61636b2e ypes..traceback.
   0x00009680 2e507954 72616365 6261636b 24475424 .PyTraceback$GT$
-  0x00009690 24475424 24475424 31376862 33333231 $GT$$GT$17hb3321
-  0x000096a0 64623531 39656461 63353445 005f5a4e db519edac54E._ZN
+  0x00009690 24475424 24475424 31376865 31326136 $GT$$GT$17he12a6
+  0x000096a0 62633432 39346362 65653945 005f5a4e bc4294cbee9E._ZN
   0x000096b0 34636f72 65337074 72323431 64726f70 4core3ptr241drop
   0x000096c0 5f696e5f 706c6163 65244c54 24616c6c _in_place$LT$all
   0x000096d0 6f632e2e 626f7865 642e2e42 6f78244c oc..boxed..Box$L
   0x000096e0 54246479 6e247532 3024636f 72652e2e T$dyn$u20$core..
   0x000096f0 6f70732e 2e66756e 6374696f 6e2e2e46 ops..function..F
   0x00009700 6e4f6e63 65244c54 24244c50 2470796f nOnce$LT$$LP$pyo
   0x00009710 332e2e6d 61726b65 722e2e50 7974686f 3..marker..Pytho
@@ -2423,46 +2423,46 @@
   0x00009740 24247532 30247079 6f332e2e 696e7374 $$u20$pyo3..inst
   0x00009750 616e6365 2e2e5079 244c5424 70796f33 ance..Py$LT$pyo3
   0x00009760 2e2e7479 7065732e 2e616e79 2e2e5079 ..types..any..Py
   0x00009770 416e7924 47542424 75326224 636f7265 Any$GT$$u2b$core
   0x00009780 2e2e6d61 726b6572 2e2e5365 6e642475 ..marker..Send$u
   0x00009790 32622463 6f72652e 2e6d6172 6b65722e 2b$core..marker.
   0x000097a0 2e53796e 63244754 24244754 24313768 .Sync$GT$$GT$17h
-  0x000097b0 63633665 39643430 33636233 61303630 cc6e9d403cb3a060
+  0x000097b0 33343964 36623666 33363330 37626634 349d6b6f36307bf4
   0x000097c0 45005f5a 4e35616c 6c6f6335 616c6c6f E._ZN5alloc5allo
-  0x000097d0 6338626f 785f6672 65653137 68396632 c8box_free17h9f2
-  0x000097e0 30343963 65643362 64646637 3045005f 049ced3bddf70E._
+  0x000097d0 6338626f 785f6672 65653137 68323862 c8box_free17h28b
+  0x000097e0 61373461 30383338 36616262 6145005f a74a08386abbaE._
   0x000097f0 5a4e3463 6f726533 70747233 3764726f ZN4core3ptr37dro
   0x00009800 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
   0x00009810 6f332e2e 6572722e 2e507945 72722447 o3..err..PyErr$G
-  0x00009820 54243137 68303861 30386662 31643463 T$17h08a08fb1d4c
-  0x00009830 34626163 3645005f 5a4e3463 6f726533 4bac6E._ZN4core3
+  0x00009820 54243137 68316430 30326230 36326337 T$17h1d002b062c7
+  0x00009830 35343566 3045005f 5a4e3463 6f726533 545f0E._ZN4core3
   0x00009840 70747238 3064726f 705f696e 5f706c61 ptr80drop_in_pla
   0x00009850 6365244c 54247079 6f332e2e 696e7374 ce$LT$pyo3..inst
   0x00009860 616e6365 2e2e5079 244c5424 70796f33 ance..Py$LT$pyo3
   0x00009870 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
   0x00009880 42617365 45786365 7074696f 6e244754 BaseException$GT
-  0x00009890 24244754 24313768 64356135 32633465 $$GT$17hd5a52c4e
-  0x000098a0 64306338 66363464 45005f5a 4e34636f d0c8f64dE._ZN4co
+  0x00009890 24244754 24313768 31353638 62653065 $$GT$17h1568be0e
+  0x000098a0 38306231 62313766 45005f5a 4e34636f 80b1b17fE._ZN4co
   0x000098b0 72653370 74723531 64726f70 5f696e5f re3ptr51drop_in_
   0x000098c0 706c6163 65244c54 24616c6c 6f632e2e place$LT$alloc..
   0x000098d0 7665632e 2e566563 244c5424 24524624 vec..Vec$LT$$RF$
-  0x000098e0 73747224 47542424 47542431 37683535 str$GT$$GT$17h55
-  0x000098f0 31653632 66663035 39313536 34374500 1e62ff05915647E.
+  0x000098e0 73747224 47542424 47542431 37683936 str$GT$$GT$17h96
+  0x000098f0 31336662 38303036 32353566 65364500 13fb8006255fe6E.
   0x00009900 5f5a4e34 636f7265 33707472 37356472 _ZN4core3ptr75dr
   0x00009910 6f705f69 6e5f706c 61636524 4c542463 op_in_place$LT$c
   0x00009920 6f72652e 2e726573 756c742e 2e526573 ore..result..Res
   0x00009930 756c7424 4c542424 52462473 74722443 ult$LT$$RF$str$C
   0x00009940 2470796f 332e2e65 72722e2e 50794572 $pyo3..err..PyEr
-  0x00009950 72244754 24244754 24313768 66353663 r$GT$$GT$17hf56c
-  0x00009960 66396239 63636566 35383130 45004743 f9b9ccef5810E.GC
+  0x00009950 72244754 24244754 24313768 62303836 r$GT$$GT$17hb086
+  0x00009960 35666333 31613530 63393837 45004743 5fc31a50c987E.GC
   0x00009970 435f6578 63657074 5f746162 6c653800 C_except_table8.
-  0x00009980 67656f72 67696f2e 31396130 39333663 georgio.19a0936c
-  0x00009990 2d636775 2e340031 66366f78 36387064 -cgu.4.1f6ox68pd
-  0x000099a0 6d676573 6b366d00 70796f33 2e333032 mgesk6m.pyo3.302
+  0x00009980 67656f72 67696f2e 66316136 39396534 georgio.f1a699e4
+  0x00009990 2d636775 2e340031 687a776c 676f6d64 -cgu.4.1hzwlgomd
+  0x000099a0 3262316e 6f7a6a00 70796f33 2e333032 2b1nozj.pyo3.302
   0x000099b0 35653963 642d6367 752e3135 005f5a4e 5e9cd-cgu.15._ZN
   0x000099c0 34325f24 4c542424 52462454 24753230 42_$LT$$RF$T$u20
   0x000099d0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
   0x000099e0 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
   0x000099f0 31376863 37306134 65343130 61326266 17hc70a4e410a2bf
   0x00009a00 64393445 005f5a4e 34636f72 65337074 d94E._ZN4core3pt
   0x00009a10 72313036 64726f70 5f696e5f 706c6163 r106drop_in_plac
@@ -2868,27 +2868,27 @@
   0x0000b310 63683137 68383265 66336635 30616462 ch17h82ef3f50adb
   0x0000b320 66353563 31450061 646c6572 2e366531 f55c1E.adler.6e1
   0x0000b330 35613463 612d6367 752e3000 636f6d70 5a4ca-cgu.0.comp
   0x0000b340 696c6572 5f627569 6c74696e 732e3536 iler_builtins.56
   0x0000b350 36356264 32352d63 67752e31 31380063 65bd25-cgu.118.c
   0x0000b360 6f6d7069 6c65725f 6275696c 74696e73 ompiler_builtins
   0x0000b370 2e353636 35626432 352d6367 752e3900 .5665bd25-cgu.9.
-  0x0000b380 67656f72 67696f2e 31396130 39333663 georgio.19a0936c
-  0x0000b390 2d636775 2e390067 656f7267 696f2e31 -cgu.9.georgio.1
-  0x0000b3a0 39613039 3336632d 6367752e 31300067 9a0936c-cgu.10.g
-  0x0000b3b0 656f7267 696f2e31 39613039 3336632d eorgio.19a0936c-
-  0x0000b3c0 6367752e 31310067 656f7267 696f2e31 cgu.11.georgio.1
-  0x0000b3d0 39613039 3336632d 6367752e 31330067 9a0936c-cgu.13.g
-  0x0000b3e0 656f7267 696f2e31 39613039 3336632d eorgio.19a0936c-
-  0x0000b3f0 6367752e 31340067 656f7267 696f2e31 cgu.14.georgio.1
-  0x0000b400 39613039 3336632d 6367752e 35006765 9a0936c-cgu.5.ge
-  0x0000b410 6f726769 6f2e3139 61303933 36632d63 orgio.19a0936c-c
-  0x0000b420 67752e36 0067656f 7267696f 2e313961 gu.6.georgio.19a
-  0x0000b430 30393336 632d6367 752e3700 67656f72 0936c-cgu.7.geor
-  0x0000b440 67696f2e 31396130 39333663 2d636775 gio.19a0936c-cgu
+  0x0000b380 67656f72 67696f2e 66316136 39396534 georgio.f1a699e4
+  0x0000b390 2d636775 2e390067 656f7267 696f2e66 -cgu.9.georgio.f
+  0x0000b3a0 31613639 3965342d 6367752e 31300067 1a699e4-cgu.10.g
+  0x0000b3b0 656f7267 696f2e66 31613639 3965342d eorgio.f1a699e4-
+  0x0000b3c0 6367752e 31310067 656f7267 696f2e66 cgu.11.georgio.f
+  0x0000b3d0 31613639 3965342d 6367752e 31330067 1a699e4-cgu.13.g
+  0x0000b3e0 656f7267 696f2e66 31613639 3965342d eorgio.f1a699e4-
+  0x0000b3f0 6367752e 31340067 656f7267 696f2e66 cgu.14.georgio.f
+  0x0000b400 31613639 3965342d 6367752e 35006765 1a699e4-cgu.5.ge
+  0x0000b410 6f726769 6f2e6631 61363939 65342d63 orgio.f1a699e4-c
+  0x0000b420 67752e36 0067656f 7267696f 2e663161 gu.6.georgio.f1a
+  0x0000b430 36393965 342d6367 752e3700 67656f72 699e4-cgu.7.geor
+  0x0000b440 67696f2e 66316136 39396534 2d636775 gio.f1a699e4-cgu
   0x0000b450 2e380070 796f332e 33303235 65396364 .8.pyo3.3025e9cd
   0x0000b460 2d636775 2e313400 7061726b 696e675f -cgu.14.parking_
   0x0000b470 6c6f745f 636f7265 2e636166 34663930 lot_core.caf4f90
   0x0000b480 612d6367 752e3800 70796f33 5f666669 a-cgu.8.pyo3_ffi
   0x0000b490 2e373662 34396332 642d6367 752e3000 .76b49c2d-cgu.0.
   0x0000b4a0 70796f33 5f666669 2e373662 34396332 pyo3_ffi.76b49c2
   0x0000b4b0 642d6367 752e3133 0070796f 335f6666 d-cgu.13.pyo3_ff
@@ -2940,3745 +2940,3746 @@
   0x0000b790 65356138 39663839 35616337 652e3632 e5a89f895ac7e.62
   0x0000b7a0 2e6c6c76 6d2e3137 36393537 36323334 .llvm.1769576234
   0x0000b7b0 31373831 34353330 3132005f 5a4e3430 1781453012._ZN40
   0x0000b7c0 5f244c54 24737472 24753230 24617324 _$LT$str$u20$as$
   0x0000b7d0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
   0x0000b7e0 65627567 24475424 33666d74 31376862 ebug$GT$3fmt17hb
   0x0000b7f0 63613830 35366463 37656561 64333745 ca8056dc7eead37E
-  0x0000b800 005f5a4e 3470796f 3335696d 706c5f31 ._ZN4pyo35impl_1
-  0x0000b810 36657874 72616374 5f617267 756d656e 6extract_argumen
-  0x0000b820 74313665 78747261 63745f61 7267756d t16extract_argum
-  0x0000b830 656e7431 37683561 61316464 32383733 ent17h5aa1dd2873
-  0x0000b840 37663664 66304500 5f5a4e34 636f7265 7f6df0E._ZN4core
-  0x0000b850 36726573 756c7431 33756e77 7261705f 6result13unwrap_
-  0x0000b860 6661696c 65643137 68646666 35343635 failed17hdff5465
-  0x0000b870 64373435 37346234 3445005f 5a4e3131 d74574b44E._ZN11
-  0x0000b880 7061726b 696e675f 6c6f7434 6f6e6365 parking_lot4once
-  0x0000b890 344f6e63 65313563 616c6c5f 6f6e6365 4Once15call_once
-  0x0000b8a0 5f666f72 63653238 5f247537 62242475 _force28_$u7b$$u
-  0x0000b8b0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x0000b8c0 75376424 31376866 66303132 33633465 u7d$17hff0123c4e
-  0x0000b8d0 63626536 39356245 2e6c6c76 6d2e3133 cbe695bE.llvm.13
-  0x0000b8e0 32333838 39333433 32323030 36393232 2388934322006922
-  0x0000b8f0 3236005f 5a4e3134 72757374 635f6465 26._ZN14rustc_de
-  0x0000b900 6d616e67 6c653132 7472795f 64656d61 mangle12try_dema
-  0x0000b910 6e676c65 31376861 33386430 36376630 ngle17ha38d067f0
-  0x0000b920 62353665 39623445 005f5a4e 37315f24 b56e9b4E._ZN71_$
-  0x0000b930 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000b940 6f6e732e 2e507952 65637572 73696f6e ons..PyRecursion
-  0x0000b950 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x0000b960 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x0000b970 67244754 2433666d 74313768 62633335 g$GT$3fmt17hbc35
-  0x0000b980 61313165 61623239 65383762 45005f5a a11eab29e87bE._Z
-  0x0000b990 4e39305f 244c5424 7374642e 2e70616e N90_$LT$std..pan
-  0x0000b9a0 69636b69 6e672e2e 62656769 6e5f7061 icking..begin_pa
-  0x0000b9b0 6e69635f 68616e64 6c65722e 2e50616e nic_handler..Pan
-  0x0000b9c0 69635061 796c6f61 64247532 30246173 icPayload$u20$as
-  0x0000b9d0 24753230 24636f72 652e2e70 616e6963 $u20$core..panic
-  0x0000b9e0 2e2e426f 784d6555 70244754 24336765 ..BoxMeUp$GT$3ge
-  0x0000b9f0 74313768 62363365 31323663 65356131 t17hb63e126ce5a1
-  0x0000ba00 39626661 45005f5a 4e347079 6f333131 9bfaE._ZN4pyo311
-  0x0000ba10 74797065 5f6f626a 65637431 30507954 type_object10PyT
-  0x0000ba20 79706549 6e666f31 31747970 655f6f62 ypeInfo11type_ob
-  0x0000ba30 6a656374 31376836 36366533 33303765 ject17h666e3307e
-  0x0000ba40 39353332 36316145 005f5a4e 37305f24 953261aE._ZN70_$
-  0x0000ba50 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000ba60 6f6e732e 2e507949 6d706f72 74457272 ons..PyImportErr
-  0x0000ba70 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
-  0x0000ba80 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x0000ba90 24475424 33666d74 31376861 64343735 $GT$3fmt17had475
-  0x0000baa0 66646261 39363638 34303045 005f5a4e fdba9668400E._ZN
-  0x0000bab0 3767656f 7267696f 3767656f 7267696f 7georgio7georgio
-  0x0000bac0 31376831 62343464 62373131 32383265 17h1b44db711282e
-  0x0000bad0 62646245 005f5a4e 3470796f 33357061 bdbE._ZN4pyo35pa
-  0x0000bae0 6e696331 3450616e 69634578 63657074 nic14PanicExcept
-  0x0000baf0 696f6e31 3866726f 6d5f7061 6e69635f ion18from_panic_
-  0x0000bb00 7061796c 6f616431 37683433 30633432 payload17h430c42
-  0x0000bb10 37396164 66633864 38384500 5f5a4e36 79adfc8d88E._ZN6
-  0x0000bb20 305f244c 54247079 6f332e2e 67696c2e 0_$LT$pyo3..gil.
-  0x0000bb30 2e47494c 506f6f6c 24753230 24617324 .GILPool$u20$as$
-  0x0000bb40 75323024 636f7265 2e2e6f70 732e2e64 u20$core..ops..d
-  0x0000bb50 726f702e 2e44726f 70244754 24346472 rop..Drop$GT$4dr
-  0x0000bb60 6f703137 68303865 31333561 33333839 op17h08e135a3389
-  0x0000bb70 31366231 3645005f 5a4e3731 5f244c54 16b16E._ZN71_$LT
-  0x0000bb80 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x0000bb90 732e2e50 79526566 6572656e 63654572 s..PyReferenceEr
-  0x0000bba0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x0000bbb0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x0000bbc0 47542433 666d7431 37683930 31646262 GT$3fmt17h901dbb
-  0x0000bbd0 65346232 35306362 65384500 5f5a4e31 e4b250cbe8E._ZN1
-  0x0000bbe0 31706172 6b696e67 5f6c6f74 39726177 1parking_lot9raw
-  0x0000bbf0 5f6d7574 65783852 61774d75 74657831 _mutex8RawMutex1
-  0x0000bc00 31756e6c 6f636b5f 736c6f77 31376831 1unlock_slow17h1
-  0x0000bc10 30336665 36376261 32326539 35653245 03fe67ba22e95e2E
-  0x0000bc20 005f5a4e 34636f72 65337074 72323333 ._ZN4core3ptr233
-  0x0000bc30 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
-  0x0000bc40 24616c6c 6f632e2e 626f7865 642e2e42 $alloc..boxed..B
-  0x0000bc50 6f78244c 54246479 6e247532 3024636f ox$LT$dyn$u20$co
-  0x0000bc60 72652e2e 6f70732e 2e66756e 6374696f re..ops..functio
-  0x0000bc70 6e2e2e46 6e244c54 24244c50 24245246 n..Fn$LT$$LP$$RF
-  0x0000bc80 2470796f 332e2e70 79636c61 73732e2e $pyo3..pyclass..
-  0x0000bc90 63726561 74655f74 7970655f 6f626a65 create_type_obje
-  0x0000bca0 63742e2e 50795479 70654275 696c6465 ct..PyTypeBuilde
-  0x0000bcb0 72244324 24425024 6d757424 75323024 r$C$$BP$mut$u20$
-  0x0000bcc0 70796f33 5f666669 2e2e6370 7974686f pyo3_ffi..cpytho
-  0x0000bcd0 6e2e2e6f 626a6563 742e2e50 79547970 n..object..PyTyp
-  0x0000bce0 654f626a 65637424 52502424 47542424 eObject$RP$$GT$$
-  0x0000bcf0 75326224 4f757470 75742475 32302424 u2b$Output$u20$$
-  0x0000bd00 75336424 24753230 24244c50 24245250 u3d$$u20$$LP$$RP
-  0x0000bd10 24244754 24244754 24313768 65333136 $$GT$$GT$17he316
-  0x0000bd20 61653062 35333564 66313338 452e6c6c ae0b535df138E.ll
-  0x0000bd30 766d2e31 31323133 38383937 36333630 vm.1121388976360
-  0x0000bd40 35363333 34393300 5f5a4e34 636f7265 5633493._ZN4core
-  0x0000bd50 33666d74 336e756d 35335f24 4c542469 3fmt3num53_$LT$i
-  0x0000bd60 6d706c24 75323024 636f7265 2e2e666d mpl$u20$core..fm
-  0x0000bd70 742e2e4c 6f776572 48657824 75323024 t..LowerHex$u20$
-  0x0000bd80 666f7224 75323024 75333224 47542433 for$u20$u32$GT$3
-  0x0000bd90 666d7431 37683338 37313765 65383065 fmt17h38717ee80e
-  0x0000bda0 31343036 65654500 5f5a4e35 616c6c6f 1406eeE._ZN5allo
-  0x0000bdb0 6335616c 6c6f6338 626f785f 66726565 c5alloc8box_free
-  0x0000bdc0 31376835 35643632 33346636 39666662 17h55d6234f69ffb
-  0x0000bdd0 64363745 2e6c6c76 6d2e3131 32313338 d67E.llvm.112138
-  0x0000bde0 38393736 33363035 36333334 3933005f 89763605633493._
-  0x0000bdf0 5a4e3731 5f244c54 2470796f 332e2e65 ZN71_$LT$pyo3..e
-  0x0000be00 78636570 74696f6e 732e2e50 7954696d xceptions..PyTim
-  0x0000be10 656f7574 4572726f 72247532 30246173 eoutError$u20$as
-  0x0000be20 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x0000be30 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x0000be40 37683937 31323935 39656264 66633932 7h9712959ebdfc92
-  0x0000be50 61334500 5f5a4e34 636f7265 33707472 a3E._ZN4core3ptr
-  0x0000be60 31313764 726f705f 696e5f70 6c616365 117drop_in_place
-  0x0000be70 244c5424 70796f33 2e2e6572 722e2e65 $LT$pyo3..err..e
-  0x0000be80 72725f73 74617465 2e2e626f 7865645f rr_state..boxed_
-  0x0000be90 61726773 244c5424 636f7265 2e2e7374 args$LT$core..st
-  0x0000bea0 722e2e65 72726f72 2e2e5574 66384572 r..error..Utf8Er
-  0x0000beb0 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
-  0x0000bec0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x0000bed0 75376424 24475424 31376863 34313538 u7d$$GT$17hc4158
-  0x0000bee0 33643166 30626535 30626245 2e6c6c76 3d1f0be50bbE.llv
-  0x0000bef0 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x0000bf00 38313132 33005f5a 4e347079 6f333570 81123._ZN4pyo35p
-  0x0000bf10 616e6963 31345061 6e696345 78636570 anic14PanicExcep
-  0x0000bf20 74696f6e 31357479 70655f6f 626a6563 tion15type_objec
-  0x0000bf30 745f7261 77313154 5950455f 4f424a45 t_raw11TYPE_OBJE
-  0x0000bf40 43543137 68623464 63303230 33663032 CT17hb4dc0203f02
-  0x0000bf50 66336133 64452e6c 6c766d2e 35363937 f3a3dE.llvm.5697
-  0x0000bf60 39323937 36393133 33303537 34373600 929769133057476.
-  0x0000bf70 5f5a4e35 616c6c6f 63336666 6935635f _ZN5alloc3ffi5c_
-  0x0000bf80 73747237 43537472 696e6731 395f6672 str7CString19_fr
-  0x0000bf90 6f6d5f76 65635f75 6e636865 636b6564 om_vec_unchecked
-  0x0000bfa0 31376836 32353937 38343364 38666265 17h62597843d8fbe
-  0x0000bfb0 31323045 00616e6f 6e2e6539 65623233 120E.anon.e9eb23
-  0x0000bfc0 37636635 30613433 62363564 36333662 7cf50a43b65d636b
-  0x0000bfd0 30663437 37306230 34652e33 312e6c6c 0f4770b04e.31.ll
-  0x0000bfe0 766d2e31 33383631 38353237 31313339 vm.1386185271139
-  0x0000bff0 30323734 3736005f 5a4e3730 5f244c54 027476._ZN70_$LT
-  0x0000c000 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x0000c010 732e2e50 79496d70 6f727457 61726e69 s..PyImportWarni
-  0x0000c020 6e672475 32302461 73247532 3024636f ng$u20$as$u20$co
-  0x0000c030 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
-  0x0000c040 54243366 6d743137 68336532 64626662 T$3fmt17h3e2dbfb
-  0x0000c050 63653761 35643834 3445005f 5a4e3538 ce7a5d844E._ZN58
-  0x0000c060 5f244c54 24542475 32302461 73247532 _$LT$T$u20$as$u2
-  0x0000c070 30247079 6f332e2e 6572722e 2e657272 0$pyo3..err..err
-  0x0000c080 5f737461 74652e2e 50794572 72417267 _state..PyErrArg
-  0x0000c090 756d656e 74732447 54243961 7267756d uments$GT$9argum
-  0x0000c0a0 656e7473 31376830 66306532 65396331 ents17h0f0e2e9c1
-  0x0000c0b0 31643338 36323645 005f5a4e 34636f72 1d38626E._ZN4cor
-  0x0000c0c0 65337074 72373164 726f705f 696e5f70 e3ptr71drop_in_p
-  0x0000c0d0 6c616365 244c5424 636f7265 2e2e7265 lace$LT$core..re
-  0x0000c0e0 73756c74 2e2e5265 73756c74 244c5424 sult..Result$LT$
-  0x0000c0f0 75363424 43247079 6f332e2e 6572722e u64$C$pyo3..err.
-  0x0000c100 2e507945 72722447 54242447 54243137 .PyErr$GT$$GT$17
-  0x0000c110 68346266 32643037 30333233 30343735 h4bf2d0703230475
-  0x0000c120 63452e6c 6c766d2e 31383335 36373530 cE.llvm.18356750
-  0x0000c130 34383536 31343531 33313239 005f5f72 485614513129.__r
-  0x0000c140 7573745f 7265616c 6c6f6300 616e6f6e ust_realloc.anon
-  0x0000c150 2e396531 31346564 35303130 64363235 .9e114ed5010d625
-  0x0000c160 33626432 36313132 39343733 63643138 3bd261129473cd18
-  0x0000c170 382e362e 6c6c766d 2e383336 34373335 8.6.llvm.8364735
-  0x0000c180 31373237 30333437 36333534 005f5a4e 172703476354._ZN
-  0x0000c190 33737464 33737973 34756e69 78326673 3std3sys4unix2fs
-  0x0000c1a0 34737461 74313768 30653864 32303165 4stat17h0e8d201e
-  0x0000c1b0 39323933 38383562 45005f5a 4e34636f 9293885bE._ZN4co
-  0x0000c1c0 72653366 6d74336e 756d3535 5f244c54 re3fmt3num55_$LT
-  0x0000c1d0 24696d70 6c247532 3024636f 72652e2e $impl$u20$core..
-  0x0000c1e0 666d742e 2e557070 65724865 78247532 fmt..UpperHex$u2
-  0x0000c1f0 3024666f 72247532 30246973 697a6524 0$for$u20$isize$
-  0x0000c200 47542433 666d7431 37686337 63346138 GT$3fmt17hc7c4a8
-  0x0000c210 61306234 33613963 62364500 5f5a4e37 a0b43a9cb6E._ZN7
-  0x0000c220 345f244c 54247079 6f332e2e 65786365 4_$LT$pyo3..exce
-  0x0000c230 7074696f 6e732e2e 50794973 41446972 ptions..PyIsADir
-  0x0000c240 6563746f 72794572 726f7224 75323024 ectoryError$u20$
-  0x0000c250 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x0000c260 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
-  0x0000c270 37686664 30393162 62646137 65313364 7hfd091bbda7e13d
-  0x0000c280 61364500 5f5a4e38 315f244c 54247079 a6E._ZN81_$LT$py
-  0x0000c290 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x0000c2a0 6173796e 63696f2e 2e4c696d 69744f76 asyncio..LimitOv
-  0x0000c2b0 65727275 6e457272 6f722475 32302461 errunError$u20$a
-  0x0000c2c0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x0000c2d0 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x0000c2e0 68316634 65626333 65656339 37323238 h1f4ebc3eec97228
-  0x0000c2f0 3145005f 5a4e3735 5f244c54 2470796f 1E._ZN75_$LT$pyo
-  0x0000c300 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x0000c310 7953746f 70417379 6e634974 65726174 yStopAsyncIterat
-  0x0000c320 696f6e24 75323024 61732475 32302463 ion$u20$as$u20$c
-  0x0000c330 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x0000c340 47542433 666d7431 37686339 35306563 GT$3fmt17hc950ec
-  0x0000c350 33633665 61353539 31374500 616e6f6e 3c6ea55917E.anon
-  0x0000c360 2e333437 64323634 65333465 62336130 .347d264e34eb3a0
-  0x0000c370 63373462 65356138 39663839 35616337 c74be5a89f895ac7
-  0x0000c380 652e322e 6c6c766d 2e313736 39353736 e.2.llvm.1769576
-  0x0000c390 32333431 37383134 35333031 32005f5a 2341781453012._Z
-  0x0000c3a0 4e37305f 244c5424 70796f33 2e2e6578 N70_$LT$pyo3..ex
-  0x0000c3b0 63657074 696f6e73 2e2e5079 53797374 ceptions..PySyst
-  0x0000c3c0 656d4572 726f7224 75323024 61732475 emError$u20$as$u
-  0x0000c3d0 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
-  0x0000c3e0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
-  0x0000c3f0 65623234 61323434 64653263 33633366 eb24a244de2c3c3f
-  0x0000c400 45005f5a 4e34636f 72653573 6c696365 E._ZN4core5slice
-  0x0000c410 35696e64 65783232 736c6963 655f696e 5index22slice_in
-  0x0000c420 6465785f 6f726465 725f6661 696c3137 dex_order_fail17
-  0x0000c430 68316638 61346666 65623163 30306562 h1f8a4ffeb1c00eb
-  0x0000c440 3345005f 5a4e3373 74643674 68726561 3E._ZN3std6threa
-  0x0000c450 64365468 72656164 336e6577 31376862 d6Thread3new17hb
-  0x0000c460 37383563 33386431 36316339 63353845 785c38d161c9c58E
-  0x0000c470 005f5a4e 34636f72 65337074 72323732 ._ZN4core3ptr272
-  0x0000c480 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
-  0x0000c490 246c6f63 6b5f6170 692e2e6d 75746578 $lock_api..mutex
-  0x0000c4a0 2e2e4d75 74657847 75617264 244c5424 ..MutexGuard$LT$
-  0x0000c4b0 7061726b 696e675f 6c6f742e 2e726177 parking_lot..raw
-  0x0000c4c0 5f6d7574 65782e2e 5261774d 75746578 _mutex..RawMutex
-  0x0000c4d0 24432424 4c502461 6c6c6f63 2e2e7665 $C$$LP$alloc..ve
-  0x0000c4e0 632e2e56 6563244c 5424636f 72652e2e c..Vec$LT$core..
-  0x0000c4f0 7074722e 2e6e6f6e 5f6e756c 6c2e2e4e ptr..non_null..N
-  0x0000c500 6f6e4e75 6c6c244c 54247079 6f335f66 onNull$LT$pyo3_f
-  0x0000c510 66692e2e 6f626a65 63742e2e 50794f62 fi..object..PyOb
-  0x0000c520 6a656374 24475424 24475424 24432461 ject$GT$$GT$$C$a
-  0x0000c530 6c6c6f63 2e2e7665 632e2e56 6563244c lloc..vec..Vec$L
-  0x0000c540 5424636f 72652e2e 7074722e 2e6e6f6e T$core..ptr..non
-  0x0000c550 5f6e756c 6c2e2e4e 6f6e4e75 6c6c244c _null..NonNull$L
-  0x0000c560 54247079 6f335f66 66692e2e 6f626a65 T$pyo3_ffi..obje
-  0x0000c570 63742e2e 50794f62 6a656374 24475424 ct..PyObject$GT$
-  0x0000c580 24475424 24525024 24475424 24475424 $GT$$RP$$GT$$GT$
-  0x0000c590 31376866 61653262 31333661 32386366 17hfae2b136a28cf
-  0x0000c5a0 63386545 2e6c6c76 6d2e3133 32333838 c8eE.llvm.132388
-  0x0000c5b0 39333433 32323030 36393232 32360061 93432200692226.a
-  0x0000c5c0 6e6f6e2e 39366261 61303862 64343636 non.96baa08bd466
-  0x0000c5d0 30663163 31316464 64383361 32353365 0f1c11ddd83a253e
-  0x0000c5e0 38343864 2e302e6c 6c766d2e 33373535 848d.0.llvm.3755
-  0x0000c5f0 34303432 31313432 32323930 34303600 404211422290406.
-  0x0000c600 616e6f6e 2e333437 64323634 65333465 anon.347d264e34e
-  0x0000c610 62336130 63373462 65356138 39663839 b3a0c74be5a89f89
-  0x0000c620 35616337 652e3130 2e6c6c76 6d2e3137 5ac7e.10.llvm.17
-  0x0000c630 36393537 36323334 31373831 34353330 6957623417814530
-  0x0000c640 3132005f 5f727573 745f7374 6172745f 12.__rust_start_
-  0x0000c650 70616e69 6300616e 6f6e2e37 62393436 panic.anon.7b946
-  0x0000c660 61653164 33613636 36373937 65326462 ae1d3a666797e2db
-  0x0000c670 31663336 65346364 3665372e 33302e6c 1f36e4cd6e7.30.l
-  0x0000c680 6c766d2e 31383335 36373530 34383536 lvm.183567504856
-  0x0000c690 31343531 33313239 005f5a4e 37345f24 14513129._ZN74_$
-  0x0000c6a0 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000c6b0 6f6e732e 2e507946 696c654e 6f74466f ons..PyFileNotFo
-  0x0000c6c0 756e6445 72726f72 24753230 24617324 undError$u20$as$
-  0x0000c6d0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x0000c6e0 65627567 24475424 33666d74 31376837 ebug$GT$3fmt17h7
-  0x0000c6f0 64343361 31333865 65316562 32656445 d43a138ee1eb2edE
-  0x0000c700 005f5a4e 37305f24 4c542470 796f332e ._ZN70_$LT$pyo3.
-  0x0000c710 2e657863 65707469 6f6e732e 2e50794f .exceptions..PyO
-  0x0000c720 76657266 6c6f7745 72726f72 24753230 verflowError$u20
-  0x0000c730 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x0000c740 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
-  0x0000c750 31376866 38626133 31343933 32643861 17hf8ba314932d8a
-  0x0000c760 33373745 00616e6f 6e2e3334 37643236 377E.anon.347d26
-  0x0000c770 34653334 65623361 30633734 62653561 4e34eb3a0c74be5a
-  0x0000c780 38396638 39356163 37652e35 2e6c6c76 89f895ac7e.5.llv
-  0x0000c790 6d2e3137 36393537 36323334 31373831 m.17695762341781
-  0x0000c7a0 34353330 3132005f 5a4e3463 6f726533 453012._ZN4core3
-  0x0000c7b0 666d7433 6e756d35 335f244c 5424696d fmt3num53_$LT$im
-  0x0000c7c0 706c2475 32302463 6f72652e 2e666d74 pl$u20$core..fmt
-  0x0000c7d0 2e2e4c6f 77657248 65782475 32302466 ..LowerHex$u20$f
-  0x0000c7e0 6f722475 32302469 36342447 54243366 or$u20$i64$GT$3f
-  0x0000c7f0 6d743137 68616461 63323332 31396233 mt17hadac23219b3
-  0x0000c800 66303266 3145005f 5a4e3470 796f3335 f02f1E._ZN4pyo35
-  0x0000c810 74797065 73366d6f 64756c65 3850794d types6module8PyM
-  0x0000c820 6f64756c 6535696e 64657831 37686565 odule5index17hee
-  0x0000c830 65643636 61323466 32633137 64644500 ed66a24f2c17ddE.
-  0x0000c840 5f5a4e37 315f244c 54247079 6f332e2e _ZN71_$LT$pyo3..
-  0x0000c850 65786365 7074696f 6e732e2e 50794279 exceptions..PyBy
-  0x0000c860 74657357 61726e69 6e672475 32302461 tesWarning$u20$a
-  0x0000c870 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x0000c880 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x0000c890 31376862 37323031 30363532 62313261 17hb72010652b12a
-  0x0000c8a0 65636145 005f5a4e 37335f24 4c542470 ecaE._ZN73_$LT$p
-  0x0000c8b0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x0000c8c0 2e507952 65637572 73696f6e 4572726f .PyRecursionErro
-  0x0000c8d0 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x0000c8e0 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
-  0x0000c8f0 47542433 666d7431 37686530 39366461 GT$3fmt17he096da
-  0x0000c900 38633562 31663662 35384500 5f5a4e35 8c5b1f6b58E._ZN5
-  0x0000c910 616c6c6f 63377261 775f7665 63313952 alloc7raw_vec19R
-  0x0000c920 61775665 63244c54 24542443 24412447 awVec$LT$T$C$A$G
-  0x0000c930 54243772 65736572 76653231 646f5f72 T$7reserve21do_r
-  0x0000c940 65736572 76655f61 6e645f68 616e646c eserve_and_handl
-  0x0000c950 65313768 35666437 33653539 39656335 e17h5fd73e599ec5
-  0x0000c960 31666264 45005f5a 4e34636f 72653370 1fbdE._ZN4core3p
-  0x0000c970 74723730 64726f70 5f696e5f 706c6163 tr70drop_in_plac
-  0x0000c980 65244c54 2470796f 332e2e69 6e737461 e$LT$pyo3..insta
-  0x0000c990 6e63652e 2e507924 4c542470 796f332e nce..Py$LT$pyo3.
-  0x0000c9a0 2e747970 65732e2e 616e792e 2e507941 .types..any..PyA
-  0x0000c9b0 6e792447 54242447 54243137 68386365 ny$GT$$GT$17h8ce
-  0x0000c9c0 62613632 64626230 38346538 61452e6c ba62dbb084e8aE.l
-  0x0000c9d0 6c766d2e 31313231 33383839 37363336 lvm.112138897636
-  0x0000c9e0 30353633 33343933 005f5a4e 35616c6c 05633493._ZN5all
-  0x0000c9f0 6f633561 6c6c6f63 31386861 6e646c65 oc5alloc18handle
-  0x0000ca00 5f616c6c 6f635f65 72726f72 3872745f _alloc_error8rt_
-  0x0000ca10 6572726f 72313768 34623739 66386137 error17h4b79f8a7
-  0x0000ca20 31373734 31623763 45005f5a 4e337374 17741b7cE._ZN3st
-  0x0000ca30 64367468 72656164 356c6f63 616c3137 d6thread5local17
-  0x0000ca40 4c6f6361 6c4b6579 244c5424 54244754 LocalKey$LT$T$GT
-  0x0000ca50 24347769 74683137 68373731 64306664 $4with17h771d0fd
-  0x0000ca60 32623232 38306333 6145005f 5a4e3463 2b2280c3aE._ZN4c
-  0x0000ca70 6f726533 70747237 3464726f 705f696e ore3ptr74drop_in
-  0x0000ca80 5f706c61 6365244c 54247079 6f332e2e _place$LT$pyo3..
-  0x0000ca90 696e7374 616e6365 2e2e5079 244c5424 instance..Py$LT$
-  0x0000caa0 70796f33 2e2e7479 7065732e 2e747570 pyo3..types..tup
-  0x0000cab0 6c652e2e 50795475 706c6524 47542424 le..PyTuple$GT$$
-  0x0000cac0 47542431 37683631 38323431 32663838 GT$17h6182412f88
-  0x0000cad0 35656263 3333452e 6c6c766d 2e313132 5ebc33E.llvm.112
-  0x0000cae0 31333838 39373633 36303536 33333439 1388976360563349
-  0x0000caf0 33005f5a 4e36375f 244c5424 70796f33 3._ZN67_$LT$pyo3
-  0x0000cb00 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
-  0x0000cb10 496e6465 78457272 6f722475 32302461 IndexError$u20$a
-  0x0000cb20 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x0000cb30 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x0000cb40 68323064 63616562 31303835 36323530 h20dcaeb10856250
-  0x0000cb50 3845005f 5a4e3463 6f726533 666d7439 8E._ZN4core3fmt9
-  0x0000cb60 466f726d 61747465 72313564 65627567 Formatter15debug
-  0x0000cb70 5f6c6f77 65725f68 65783137 68656235 _lower_hex17heb5
-  0x0000cb80 66623036 34363837 63316233 6345005f fb064687c1b3cE._
-  0x0000cb90 5a4e3739 5f244c54 2470796f 332e2e65 ZN79_$LT$pyo3..e
-  0x0000cba0 78636570 74696f6e 732e2e50 79436f6e xceptions..PyCon
-  0x0000cbb0 6e656374 696f6e52 65667573 65644572 nectionRefusedEr
-  0x0000cbc0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x0000cbd0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x0000cbe0 47542433 666d7431 37686537 62653636 GT$3fmt17he7be66
-  0x0000cbf0 39323566 38396334 33354500 616e6f6e 925f89c435E.anon
-  0x0000cc00 2e653965 62323337 63663530 61343362 .e9eb237cf50a43b
-  0x0000cc10 36356436 33366230 66343737 30623034 65d636b0f4770b04
-  0x0000cc20 652e3532 2e6c6c76 6d2e3133 38363138 e.52.llvm.138618
-  0x0000cc30 35323731 31333930 32373437 36005f5a 5271139027476._Z
-  0x0000cc40 4e37325f 244c5424 70796f33 2e2e6578 N72_$LT$pyo3..ex
-  0x0000cc50 63657074 696f6e73 2e2e5079 46757475 ceptions..PyFutu
-  0x0000cc60 72655761 726e696e 67247532 30246173 reWarning$u20$as
-  0x0000cc70 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x0000cc80 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x0000cc90 37686232 63323463 30346436 32626564 7hb2c24c04d62bed
-  0x0000cca0 36354500 5f5a4e37 375f244c 54247079 65E._ZN77_$LT$py
-  0x0000ccb0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x0000ccc0 50795374 6f704173 796e6349 74657261 PyStopAsyncItera
-  0x0000ccd0 74696f6e 24753230 24617324 75323024 tion$u20$as$u20$
-  0x0000cce0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x0000ccf0 61792447 54243366 6d743137 68626564 ay$GT$3fmt17hbed
-  0x0000cd00 39313762 30356235 62336463 3945005f 917b05b5b3dc9E._
-  0x0000cd10 5a4e3463 6f726533 70747234 3264726f ZN4core3ptr42dro
-  0x0000cd20 705f696e 5f706c61 6365244c 5424616c p_in_place$LT$al
-  0x0000cd30 6c6f632e 2e737472 696e672e 2e537472 loc..string..Str
-  0x0000cd40 696e6724 47542431 37686164 61393761 ing$GT$17hada97a
-  0x0000cd50 63306565 38666433 3563452e 6c6c766d c0ee8fd35cE.llvm
-  0x0000cd60 2e333034 31333933 39353835 36393937 .304139395856997
-  0x0000cd70 34333439 005f5a4e 37345f24 4c542470 4349._ZN74_$LT$p
-  0x0000cd80 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x0000cd90 2e507950 65726d69 7373696f 6e457272 .PyPermissionErr
-  0x0000cda0 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
-  0x0000cdb0 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x0000cdc0 24475424 33666d74 31376865 61633461 $GT$3fmt17heac4a
-  0x0000cdd0 66363364 39646138 65306345 005f5a4e f63d9da8e0cE._ZN
-  0x0000cde0 36395f24 4c542470 796f332e 2e657863 69_$LT$pyo3..exc
-  0x0000cdf0 65707469 6f6e732e 2e507954 696d656f eptions..PyTimeo
-  0x0000ce00 75744572 726f7224 75323024 61732475 utError$u20$as$u
-  0x0000ce10 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x0000ce20 62756724 47542433 666d7431 37683433 bug$GT$3fmt17h43
-  0x0000ce30 62656163 63653237 30656639 62304500 beacce270ef9b0E.
-  0x0000ce40 5f5a4e34 636f7265 35736c69 6365366d _ZN4core5slice6m
-  0x0000ce50 656d6368 7231346d 656d6368 725f616c emchr14memchr_al
-  0x0000ce60 69676e65 64313768 30343235 64633533 igned17h0425dc53
-  0x0000ce70 35323832 66303031 45005f5a 4e34636f 5282f001E._ZN4co
-  0x0000ce80 7265366f 7074696f 6e313365 78706563 re6option13expec
-  0x0000ce90 745f6661 696c6564 31376830 39623938 t_failed17h09b98
-  0x0000cea0 32363339 33333665 37656145 005f5a4e 2639336e7eaE._ZN
-  0x0000ceb0 37345f24 4c542470 796f332e 2e657863 74_$LT$pyo3..exc
-  0x0000cec0 65707469 6f6e732e 2e507955 6e626f75 eptions..PyUnbou
-  0x0000ced0 6e644c6f 63616c45 72726f72 24753230 ndLocalError$u20
-  0x0000cee0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x0000cef0 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
-  0x0000cf00 31376864 36663836 32333561 62616361 17hd6f86235abaca
-  0x0000cf10 35373745 005f5a4e 34636f72 6533666d 577E._ZN4core3fm
-  0x0000cf20 74386275 696c6465 72733130 44656275 t8builders10Debu
-  0x0000cf30 67547570 6c653566 69656c64 31376862 gTuple5field17hb
-  0x0000cf40 63306430 36323439 33373963 32623045 c0d06249379c2b0E
-  0x0000cf50 005f5a4e 31367061 726b696e 675f6c6f ._ZN16parking_lo
-  0x0000cf60 745f636f 72653977 6f72645f 6c6f636b t_core9word_lock
-  0x0000cf70 38576f72 644c6f63 6b313175 6e6c6f63 8WordLock11unloc
-  0x0000cf80 6b5f736c 6f773137 68613264 37663538 k_slow17ha2d7f58
-  0x0000cf90 34336531 63326130 3445005f 5a4e3463 43e1c2a04E._ZN4c
-  0x0000cfa0 6f726533 70747231 32306472 6f705f69 ore3ptr120drop_i
-  0x0000cfb0 6e5f706c 61636524 4c542470 796f332e n_place$LT$pyo3.
-  0x0000cfc0 2e657272 2e2e6572 725f7374 6174652e .err..err_state.
-  0x0000cfd0 2e626f78 65645f61 72677324 4c542463 .boxed_args$LT$c
-  0x0000cfe0 6f72652e 2e617272 61792e2e 54727946 ore..array..TryF
-  0x0000cff0 726f6d53 6c696365 4572726f 72244754 romSliceError$GT
-  0x0000d000 242e2e24 75376224 24753762 24636c6f $..$u7b$$u7b$clo
-  0x0000d010 73757265 24753764 24247537 64242447 sure$u7d$$u7d$$G
-  0x0000d020 54243137 68353234 61333262 33333038 T$17h524a32b3308
-  0x0000d030 62326434 32452e6c 6c766d2e 33313630 b2d42E.llvm.3160
-  0x0000d040 39303732 38313838 30373831 31323300 907281880781123.
-  0x0000d050 616e6f6e 2e376239 34366165 31643361 anon.7b946ae1d3a
-  0x0000d060 36363637 39376532 64623166 33366534 666797e2db1f36e4
-  0x0000d070 63643665 372e3231 2e6c6c76 6d2e3138 cd6e7.21.llvm.18
-  0x0000d080 33353637 35303438 35363134 35313331 3567504856145131
-  0x0000d090 32390061 6e6f6e2e 39653131 34656435 29.anon.9e114ed5
-  0x0000d0a0 30313064 36323533 62643236 31313239 010d6253bd261129
-  0x0000d0b0 34373363 64313838 2e342e6c 6c766d2e 473cd188.4.llvm.
-  0x0000d0c0 38333634 37333531 37323730 33343736 8364735172703476
-  0x0000d0d0 33353400 5f5a4e37 315f244c 54247079 354._ZN71_$LT$py
-  0x0000d0e0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x0000d0f0 5079556e 69636f64 65457272 6f722475 PyUnicodeError$u
-  0x0000d100 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x0000d110 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x0000d120 33666d74 31376837 38653335 38613432 3fmt17h78e358a42
-  0x0000d130 62393735 33326445 005f5a4e 37335f24 b97532dE._ZN73_$
-  0x0000d140 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000d150 6f6e732e 2e507945 6e766972 6f6e6d65 ons..PyEnvironme
-  0x0000d160 6e744572 726f7224 75323024 61732475 ntError$u20$as$u
-  0x0000d170 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x0000d180 62756724 47542433 666d7431 37686137 bug$GT$3fmt17ha7
-  0x0000d190 61376437 35616433 66346361 33364500 a7d75ad3f4ca36E.
-  0x0000d1a0 5f5a4e37 385f244c 54247079 6f332e2e _ZN78_$LT$pyo3..
-  0x0000d1b0 65786365 7074696f 6e732e2e 50794d6f exceptions..PyMo
-  0x0000d1c0 64756c65 4e6f7446 6f756e64 4572726f duleNotFoundErro
-  0x0000d1d0 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x0000d1e0 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
-  0x0000d1f0 47542433 666d7431 37686234 32656130 GT$3fmt17hb42ea0
-  0x0000d200 36653630 62363463 64334500 5f5a4e34 6e60b64cd3E._ZN4
-  0x0000d210 70796f33 3473796e 63323047 494c4f6e pyo34sync20GILOn
-  0x0000d220 63654365 6c6c244c 54245424 47542434 ceCell$LT$T$GT$4
-  0x0000d230 696e6974 31376863 31383931 62626165 init17hc1891bbae
-  0x0000d240 31393938 32306145 005f5a4e 38335f24 199820aE._ZN83_$
-  0x0000d250 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000d260 6f6e732e 2e617379 6e63696f 2e2e496e ons..asyncio..In
-  0x0000d270 636f6d70 6c657465 52656164 4572726f completeReadErro
-  0x0000d280 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x0000d290 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x0000d2a0 2433666d 74313768 32373738 64333731 $3fmt17h2778d371
-  0x0000d2b0 34376434 30346531 45005f5a 4e34636f 47d404e1E._ZN4co
-  0x0000d2c0 72653370 74723337 64726f70 5f696e5f re3ptr37drop_in_
-  0x0000d2d0 706c6163 65244c54 2470796f 332e2e65 place$LT$pyo3..e
-  0x0000d2e0 72722e2e 50794572 72244754 24313768 rr..PyErr$GT$17h
-  0x0000d2f0 62643734 35376230 32303537 33643162 bd7457b020573d1b
-  0x0000d300 452e6c6c 766d2e31 37363935 37363233 E.llvm.176957623
-  0x0000d310 34313738 31343533 30313200 5f5a4e36 41781453012._ZN6
-  0x0000d320 365f244c 54247079 6f332e2e 74797065 6_$LT$pyo3..type
-  0x0000d330 732e2e70 79737570 65722e2e 50795375 s..pysuper..PySu
-  0x0000d340 70657224 75323024 61732475 32302463 per$u20$as$u20$c
-  0x0000d350 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x0000d360 47542433 666d7431 37686661 37363931 GT$3fmt17hfa7691
-  0x0000d370 62316231 37306338 35614500 5f5a4e35 b1b170c85aE._ZN5
-  0x0000d380 616c6c6f 6335616c 6c6f6338 626f785f alloc5alloc8box_
-  0x0000d390 66726565 31376865 38306164 65323565 free17he80ade25e
-  0x0000d3a0 37373561 34646345 2e6c6c76 6d2e3833 775a4dcE.llvm.83
-  0x0000d3b0 36343733 35313732 37303334 37363335 6473517270347635
-  0x0000d3c0 34005f5a 4e39305f 244c5424 70796f33 4._ZN90_$LT$pyo3
-  0x0000d3d0 2e2e6572 722e2e50 79457272 24753230 ..err..PyErr$u20
-  0x0000d3e0 24617324 75323024 636f7265 2e2e636f $as$u20$core..co
-  0x0000d3f0 6e766572 742e2e46 726f6d24 4c542470 nvert..From$LT$p
-  0x0000d400 796f332e 2e657272 2e2e5079 446f776e yo3..err..PyDown
-  0x0000d410 63617374 4572726f 72244754 24244754 castError$GT$$GT
-  0x0000d420 24346672 6f6d3137 68376266 36303633 $4from17h7bf6063
-  0x0000d430 61346461 63626635 3445005f 5a4e3636 a4dacbf54E._ZN66
-  0x0000d440 5f244c54 24616c6c 6f632e2e 626f7272 _$LT$alloc..borr
-  0x0000d450 6f772e2e 436f7724 4c542442 24475424 ow..Cow$LT$B$GT$
-  0x0000d460 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000d470 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x0000d480 54243366 6d743137 68613138 36623363 T$3fmt17ha186b3c
-  0x0000d490 30663762 37326564 6145005f 5a4e3136 0f7b72edaE._ZN16
-  0x0000d4a0 7061726b 696e675f 6c6f745f 636f7265 parking_lot_core
-  0x0000d4b0 31317061 726b696e 675f6c6f 74313677 11parking_lot16w
-  0x0000d4c0 6974685f 74687265 61645f64 61746131 ith_thread_data1
-  0x0000d4d0 31544852 4541445f 44415441 375f5f67 1THREAD_DATA7__g
-  0x0000d4e0 65746974 355f5f4b 45593137 68666332 etit5__KEY17hfc2
-  0x0000d4f0 34616564 61653533 30336161 6545005f 4aedae5303aaeE._
-  0x0000d500 5a4e3463 6f726533 70747233 3764726f ZN4core3ptr37dro
-  0x0000d510 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
-  0x0000d520 6f332e2e 6572722e 2e507945 72722447 o3..err..PyErr$G
-  0x0000d530 54243137 68626437 34353762 30323035 T$17hbd7457b0205
-  0x0000d540 37336431 62452e6c 6c766d2e 31383335 73d1bE.llvm.1835
-  0x0000d550 36373530 34383536 31343531 33313239 6750485614513129
-  0x0000d560 00616e6f 6e2e3334 37643236 34653334 .anon.347d264e34
-  0x0000d570 65623361 30633734 62653561 38396638 eb3a0c74be5a89f8
-  0x0000d580 39356163 37652e39 2e6c6c76 6d2e3137 95ac7e.9.llvm.17
-  0x0000d590 36393537 36323334 31373831 34353330 6957623417814530
-  0x0000d5a0 3132005f 5a4e3463 6f726533 70747236 12._ZN4core3ptr6
-  0x0000d5b0 3564726f 705f696e 5f706c61 6365244c 5drop_in_place$L
-  0x0000d5c0 5424636f 72652e2e 6f707469 6f6e2e2e T$core..option..
-  0x0000d5d0 4f707469 6f6e244c 54247079 6f332e2e Option$LT$pyo3..
-  0x0000d5e0 6572722e 2e507945 72722447 54242447 err..PyErr$GT$$G
-  0x0000d5f0 54243137 68666234 61623738 64613464 T$17hfb4ab78da4d
-  0x0000d600 32393261 64452e6c 6c766d2e 31333836 292adE.llvm.1386
-  0x0000d610 31383532 37313133 39303237 34373600 185271139027476.
-  0x0000d620 5f5a4e34 636f7265 33707472 38316472 _ZN4core3ptr81dr
-  0x0000d630 6f705f69 6e5f706c 61636524 4c542461 op_in_place$LT$a
-  0x0000d640 6c6c6f63 2e2e7665 632e2e56 6563244c lloc..vec..Vec$L
-  0x0000d650 54247061 726b696e 675f6c6f 745f636f T$parking_lot_co
-  0x0000d660 72652e2e 7061726b 696e675f 6c6f742e re..parking_lot.
-  0x0000d670 2e427563 6b657424 47542424 47542431 .Bucket$GT$$GT$1
-  0x0000d680 37683330 36646361 38366363 65373062 7h306dca86cce70b
-  0x0000d690 6362452e 6c6c766d 2e313139 32363433 cbE.llvm.1192643
-  0x0000d6a0 35363936 37333336 31373730 33005f5a 5696733617703._Z
-  0x0000d6b0 4e34636f 72653366 6d74336e 756d3533 N4core3fmt3num53
-  0x0000d6c0 5f244c54 24696d70 6c247532 3024636f _$LT$impl$u20$co
-  0x0000d6d0 72652e2e 666d742e 2e557070 65724865 re..fmt..UpperHe
-  0x0000d6e0 78247532 3024666f 72247532 30246936 x$u20$for$u20$i6
-  0x0000d6f0 34244754 2433666d 74313768 62656465 4$GT$3fmt17hbede
-  0x0000d700 63643262 66343664 31313039 45005f5a cd2bf46d1109E._Z
-  0x0000d710 4e34636f 72653366 6d743557 72697465 N4core3fmt5Write
-  0x0000d720 31307772 6974655f 63686172 31376866 10write_char17hf
-  0x0000d730 61666339 32363166 34613532 34623345 afc9261f4a524b3E
-  0x0000d740 005f5a4e 3567696d 6c693472 65616436 ._ZN5gimli4read6
-  0x0000d750 61626272 65763130 41747472 69627574 abbrev10Attribut
-  0x0000d760 6573336e 65773137 68316239 39613838 es3new17h1b99a88
-  0x0000d770 37653633 66636636 3545005f 5f72646c 7e63fcf65E.__rdl
-  0x0000d780 5f646561 6c6c6f63 005f5a4e 34636f72 _dealloc._ZN4cor
-  0x0000d790 65337074 72333764 726f705f 696e5f70 e3ptr37drop_in_p
-  0x0000d7a0 6c616365 244c5424 636f7265 2e2e666d lace$LT$core..fm
-  0x0000d7b0 742e2e45 72726f72 24475424 31376865 t..Error$GT$17he
-  0x0000d7c0 32306363 33613638 63363162 62313945 20cc3a68c61bb19E
-  0x0000d7d0 2e6c6c76 6d2e3133 32333838 39333433 .llvm.1323889343
-  0x0000d7e0 32323030 36393232 3236005f 5a4e3373 2200692226._ZN3s
-  0x0000d7f0 74643674 68726561 64356c6f 63616c34 td6thread5local4
-  0x0000d800 66617374 31324b65 79244c54 24542447 fast12Key$LT$T$G
-  0x0000d810 54243134 7472795f 696e6974 69616c69 T$14try_initiali
-  0x0000d820 7a653137 68613661 65336438 30363435 ze17ha6ae3d80645
-  0x0000d830 31323235 39452e6c 6c766d2e 33313039 12259E.llvm.3109
-  0x0000d840 36323537 31323431 36353035 33353300 625712416505353.
-  0x0000d850 5f5f7264 6c5f616c 6c6f635f 7a65726f __rdl_alloc_zero
-  0x0000d860 6564005f 5a4e3463 6f726537 756e6963 ed._ZN4core7unic
-  0x0000d870 6f646531 32756e69 636f6465 5f646174 ode12unicode_dat
-  0x0000d880 61313567 72617068 656d655f 65787465 a15grapheme_exte
-  0x0000d890 6e64366c 6f6f6b75 70313768 64373639 nd6lookup17hd769
-  0x0000d8a0 34363566 39356534 66313765 45005f5a 465f95e4f17eE._Z
-  0x0000d8b0 4e347079 6f333569 6d706c5f 31366578 N4pyo35impl_16ex
-  0x0000d8c0 74726163 745f6172 67756d65 6e743139 tract_argument19
-  0x0000d8d0 46756e63 74696f6e 44657363 72697074 FunctionDescript
-  0x0000d8e0 696f6e33 376d6973 73696e67 5f726571 ion37missing_req
-  0x0000d8f0 75697265 645f706f 73697469 6f6e616c uired_positional
-  0x0000d900 5f617267 756d656e 74733137 68346161 _arguments17h4aa
-  0x0000d910 61623264 38306434 31616130 3645005f ab2d80d41aa06E._
-  0x0000d920 5a4e3635 5f244c54 24736d61 6c6c7665 ZN65_$LT$smallve
-  0x0000d930 632e2e43 6f6c6c65 6374696f 6e416c6c c..CollectionAll
-  0x0000d940 6f634572 72247532 30246173 24753230 ocErr$u20$as$u20
-  0x0000d950 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x0000d960 67244754 2433666d 74313768 33343864 g$GT$3fmt17h348d
-  0x0000d970 34303736 61373864 66613035 45005f5a 4076a78dfa05E._Z
-  0x0000d980 4e36325f 244c5424 7374642e 2e696f2e N62_$LT$std..io.
-  0x0000d990 2e657272 6f722e2e 4572726f 724b696e .error..ErrorKin
-  0x0000d9a0 64247532 30246173 24753230 24636f72 d$u20$as$u20$cor
-  0x0000d9b0 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x0000d9c0 2433666d 74313768 63303833 35373639 $3fmt17hc0835769
-  0x0000d9d0 32313762 62393233 45005f5a 4e347079 217bb923E._ZN4py
-  0x0000d9e0 6f333365 72723550 79457272 3474616b o33err5PyErr4tak
-  0x0000d9f0 65313768 34303234 31613733 30323734 e17h40241a730274
-  0x0000da00 35323334 45005f5a 4e37345f 244c5424 5234E._ZN74_$LT$
-  0x0000da10 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x0000da20 2e2e5079 426c6f63 6b696e67 494f4572 ..PyBlockingIOEr
-  0x0000da30 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x0000da40 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
-  0x0000da50 79244754 2433666d 74313768 31363137 y$GT$3fmt17h1617
-  0x0000da60 63306363 65333165 65333831 45005f5a c0cce31ee381E._Z
-  0x0000da70 4e39335f 244c5424 7374642e 2e70616e N93_$LT$std..pan
-  0x0000da80 69636b69 6e672e2e 62656769 6e5f7061 icking..begin_pa
-  0x0000da90 6e69635f 68616e64 6c65722e 2e537472 nic_handler..Str
-  0x0000daa0 50616e69 63506179 6c6f6164 24753230 PanicPayload$u20
-  0x0000dab0 24617324 75323024 636f7265 2e2e7061 $as$u20$core..pa
-  0x0000dac0 6e69632e 2e426f78 4d655570 24475424 nic..BoxMeUp$GT$
-  0x0000dad0 3874616b 655f626f 78313768 62353336 8take_box17hb536
-  0x0000dae0 65383165 63303661 66363864 4500616e e81ec06af68dE.an
-  0x0000daf0 6f6e2e65 39656232 33376366 35306134 on.e9eb237cf50a4
-  0x0000db00 33623635 64363336 62306634 37373062 3b65d636b0f4770b
-  0x0000db10 3034652e 33302e6c 6c766d2e 31333836 04e.30.llvm.1386
-  0x0000db20 31383532 37313133 39303237 34373600 185271139027476.
-  0x0000db30 5f5a4e34 636f7265 35736c69 63653569 _ZN4core5slice5i
-  0x0000db40 6e646578 3234736c 6963655f 656e645f ndex24slice_end_
-  0x0000db50 696e6465 785f6c65 6e5f6661 696c3137 index_len_fail17
-  0x0000db60 68393534 61633837 63636461 35346336 h954ac87ccda54c6
-  0x0000db70 3245005f 5a4e3136 7061726b 696e675f 2E._ZN16parking_
-  0x0000db80 6c6f745f 636f7265 31317061 726b696e lot_core11parkin
-  0x0000db90 675f6c6f 74313146 61697254 696d656f g_lot11FairTimeo
-  0x0000dba0 75743767 656e5f75 33323137 68613962 ut7gen_u3217ha9b
-  0x0000dbb0 39326666 35346563 34373738 3645005f 92ff54ec47786E._
-  0x0000dbc0 5a4e3733 5f244c54 2470796f 332e2e65 ZN73_$LT$pyo3..e
-  0x0000dbd0 78636570 74696f6e 732e2e50 79556e69 xceptions..PyUni
-  0x0000dbe0 636f6465 5761726e 696e6724 75323024 codeWarning$u20$
-  0x0000dbf0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x0000dc00 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
-  0x0000dc10 74313768 33343065 64386563 33353465 t17h340ed8ec354e
-  0x0000dc20 64366138 45005f5a 4e37395f 244c5424 d6a8E._ZN79_$LT$
-  0x0000dc30 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x0000dc40 2e2e5079 436f6e6e 65637469 6f6e5265 ..PyConnectionRe
-  0x0000dc50 73657445 72726f72 24753230 24617324 setError$u20$as$
-  0x0000dc60 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x0000dc70 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
-  0x0000dc80 68383937 36643538 37393336 62363730 h8976d587936b670
-  0x0000dc90 3345005f 5a4e3470 796f3335 696d706c 3E._ZN4pyo35impl
-  0x0000dca0 5f313665 78747261 63745f61 7267756d _16extract_argum
-  0x0000dcb0 656e7432 35617267 756d656e 745f6578 ent25argument_ex
-  0x0000dcc0 74726163 74696f6e 5f657272 6f723137 traction_error17
-  0x0000dcd0 68636335 38343665 39623833 36396162 hcc5846e9b8369ab
-  0x0000dce0 6345005f 5a4e3463 6f726533 73747235 cE._ZN4core3str5
-  0x0000dcf0 636f756e 74313464 6f5f636f 756e745f count14do_count_
-  0x0000dd00 63686172 73313768 37656130 32656666 chars17h7ea02eff
-  0x0000dd10 66653362 32613165 4500616e 6f6e2e65 fe3b2a1eE.anon.e
-  0x0000dd20 39656232 33376366 35306134 33623635 9eb237cf50a43b65
-  0x0000dd30 64363336 62306634 37373062 3034652e d636b0f4770b04e.
-  0x0000dd40 32372e6c 6c766d2e 31333836 31383532 27.llvm.13861852
-  0x0000dd50 37313133 39303237 34373600 5f5a4e34 71139027476._ZN4
-  0x0000dd60 70796f33 3367696c 31357265 67697374 pyo33gil15regist
-  0x0000dd70 65725f64 65637265 66313768 36333366 er_decref17h633f
-  0x0000dd80 39343863 34396436 38636437 45005f5a 948c49d68cd7E._Z
-  0x0000dd90 4e37315f 244c5424 72757374 635f6465 N71_$LT$rustc_de
-  0x0000dda0 6d616e67 6c652e2e 6c656761 63792e2e mangle..legacy..
-  0x0000ddb0 44656d61 6e676c65 24753230 24617324 Demangle$u20$as$
-  0x0000ddc0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x0000ddd0 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
-  0x0000dde0 68326139 63323532 31663938 65656166 h2a9c2521f98eeaf
-  0x0000ddf0 6345005f 5a4e3434 5f244c54 24245246 cE._ZN44_$LT$$RF
-  0x0000de00 24542475 32302461 73247532 3024636f $T$u20$as$u20$co
-  0x0000de10 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x0000de20 24475424 33666d74 31376838 65323033 $GT$3fmt17h8e203
-  0x0000de30 65613937 64653031 62646545 005f5a4e ea97de01bdeE._ZN
-  0x0000de40 34636f72 65397061 6e69636b 696e6731 4core9panicking1
-  0x0000de50 3370616e 69635f64 6973706c 61793137 3panic_display17
-  0x0000de60 68306535 32663264 34646137 66633231 h0e52f2d4da7fc21
-  0x0000de70 31452e6c 6c766d2e 31383335 36373530 1E.llvm.18356750
-  0x0000de80 34383536 31343531 33313239 005f5f72 485614513129.__r
-  0x0000de90 7573745f 70726f62 65737461 636b005f ust_probestack._
-  0x0000dea0 5a4e3736 5f244c54 2470796f 332e2e65 ZN76_$LT$pyo3..e
-  0x0000deb0 78636570 74696f6e 732e2e50 794e6f74 xceptions..PyNot
-  0x0000dec0 496d706c 656d656e 74656445 72726f72 ImplementedError
-  0x0000ded0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000dee0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x0000def0 33666d74 31376836 62616239 62626337 3fmt17h6bab9bbc7
-  0x0000df00 37663032 65623045 005f5a4e 3470796f 7f02eb0E._ZN4pyo
-  0x0000df10 33313174 7970655f 6f626a65 63743130 311type_object10
-  0x0000df20 50795479 7065496e 666f3131 74797065 PyTypeInfo11type
-  0x0000df30 5f6f626a 65637431 37686364 36636466 _object17hcd6cdf
-  0x0000df40 65393061 61616530 35644500 5f5a4e36 e90aaae05dE._ZN6
-  0x0000df50 395f244c 54247079 6f332e2e 65786365 9_$LT$pyo3..exce
-  0x0000df60 7074696f 6e732e2e 50794279 74657357 ptions..PyBytesW
-  0x0000df70 61726e69 6e672475 32302461 73247532 arning$u20$as$u2
-  0x0000df80 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x0000df90 75672447 54243366 6d743137 68323131 ug$GT$3fmt17h211
-  0x0000dfa0 31366461 31323338 37643531 62450061 16da12387d51bE.a
-  0x0000dfb0 6e6f6e2e 39653131 34656435 30313064 non.9e114ed5010d
-  0x0000dfc0 36323533 62643236 31313239 34373363 6253bd261129473c
-  0x0000dfd0 64313838 2e312e6c 6c766d2e 38333634 d188.1.llvm.8364
-  0x0000dfe0 37333531 37323730 33343736 33353400 735172703476354.
-  0x0000dff0 5f5f474e 555f4548 5f465241 4d455f48 __GNU_EH_FRAME_H
-  0x0000e000 4452005f 5a4e366f 626a6563 7433656c DR._ZN6object3el
-  0x0000e010 66313245 4c465f4e 4f54455f 474e5531 f12ELF_NOTE_GNU1
-  0x0000e020 37686661 34303936 62336634 62373162 7hfa4096b3f4b71b
-  0x0000e030 36644500 5f5a4e34 636f7265 33666d74 6dE._ZN4core3fmt
-  0x0000e040 336e756d 33696d70 35345f24 4c542469 3num3imp54_$LT$i
-  0x0000e050 6d706c24 75323024 636f7265 2e2e666d mpl$u20$core..fm
-  0x0000e060 742e2e44 6973706c 61792475 32302466 t..Display$u20$f
-  0x0000e070 6f722475 32302475 73697a65 24475424 or$u20$usize$GT$
-  0x0000e080 33666d74 31376833 37396637 39393634 3fmt17h379f79964
-  0x0000e090 65646365 64323945 005f5a4e 34636f72 edced29E._ZN4cor
-  0x0000e0a0 65337074 72343264 726f705f 696e5f70 e3ptr42drop_in_p
-  0x0000e0b0 6c616365 244c5424 616c6c6f 632e2e73 lace$LT$alloc..s
-  0x0000e0c0 7472696e 672e2e53 7472696e 67244754 tring..String$GT
-  0x0000e0d0 24313768 61646139 37616330 65653866 $17hada97ac0ee8f
-  0x0000e0e0 64333563 452e6c6c 766d2e35 36393739 d35cE.llvm.56979
-  0x0000e0f0 32393736 39313333 30353734 3736005f 29769133057476._
-  0x0000e100 5a4e3470 796f3331 31636f6e 76657273 ZN4pyo311convers
-  0x0000e110 696f6e73 33737464 336e756d 36345f24 ions3std3num64_$
-  0x0000e120 4c542469 6d706c24 75323024 70796f33 LT$impl$u20$pyo3
-  0x0000e130 2e2e636f 6e766572 73696f6e 2e2e4672 ..conversion..Fr
-  0x0000e140 6f6d5079 4f626a65 63742475 32302466 omPyObject$u20$f
-  0x0000e150 6f722475 32302475 33322447 54243765 or$u20$u32$GT$7e
-  0x0000e160 78747261 63743137 68653339 30323233 xtract17he390223
-  0x0000e170 32326238 62653330 38450061 6e6f6e2e 22b8be308E.anon.
-  0x0000e180 37623934 36616531 64336136 36363739 7b946ae1d3a66679
-  0x0000e190 37653264 62316633 36653463 64366537 7e2db1f36e4cd6e7
-  0x0000e1a0 2e382e6c 6c766d2e 31383335 36373530 .8.llvm.18356750
-  0x0000e1b0 34383536 31343531 33313239 005f6669 485614513129._fi
-  0x0000e1c0 6e69005f 5a4e3634 5f244c54 24737464 ni._ZN64_$LT$std
-  0x0000e1d0 2e2e7379 732e2e75 6e69782e 2e737464 ..sys..unix..std
-  0x0000e1e0 696f2e2e 53746465 72722475 32302461 io..Stderr$u20$a
-  0x0000e1f0 73247532 30247374 642e2e69 6f2e2e57 s$u20$std..io..W
-  0x0000e200 72697465 24475424 35666c75 73683137 rite$GT$5flush17
-  0x0000e210 68316134 34616530 34626436 66343463 h1a44ae04bd6f44c
-  0x0000e220 3045005f 5a4e3136 7061726b 696e675f 0E._ZN16parking_
-  0x0000e230 6c6f745f 636f7265 31317061 726b696e lot_core11parkin
-  0x0000e240 675f6c6f 74313054 68726561 64446174 g_lot10ThreadDat
-  0x0000e250 61336e65 77313768 65333130 63613230 a3new17he310ca20
-  0x0000e260 39633638 66323361 45005f5a 4e37315f 9c68f23aE._ZN71_
-  0x0000e270 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x0000e280 696f6e73 2e2e5079 52756e74 696d6557 ions..PyRuntimeW
-  0x0000e290 61726e69 6e672475 32302461 73247532 arning$u20$as$u2
-  0x0000e2a0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x0000e2b0 75672447 54243366 6d743137 68306366 ug$GT$3fmt17h0cf
-  0x0000e2c0 32616531 30346364 63303764 64450044 2ae104cdc07ddE.D
-  0x0000e2d0 572e7265 662e7275 73745f65 685f7065 W.ref.rust_eh_pe
-  0x0000e2e0 72736f6e 616c6974 79005f5a 4e34636f rsonality._ZN4co
-  0x0000e2f0 7265336f 70733866 756e6374 696f6e36 re3ops8function6
-  0x0000e300 466e4f6e 63653430 63616c6c 5f6f6e63 FnOnce40call_onc
-  0x0000e310 65247537 62242475 37622476 7461626c e$u7b$$u7b$vtabl
-  0x0000e320 652e7368 696d2475 37642424 75376424 e.shim$u7d$$u7d$
-  0x0000e330 31376832 32306163 33383135 66666332 17h220ac3815ffc2
-  0x0000e340 63376445 2e6c6c76 6d2e3331 36303930 c7dE.llvm.316090
-  0x0000e350 37323831 38383037 38313132 33005f5a 7281880781123._Z
-  0x0000e360 4e34636f 72653366 6d743862 75696c64 N4core3fmt8build
-  0x0000e370 65727339 44656275 674c6973 7435656e ers9DebugList5en
-  0x0000e380 74727931 37686239 66666636 62306331 try17hb9fff6b0c1
-  0x0000e390 31343035 31624500 5f5a4e35 616c6c6f 14051bE._ZN5allo
-  0x0000e3a0 63337665 63313656 6563244c 54245424 c3vec16Vec$LT$T$
-  0x0000e3b0 43244124 47542431 36696e74 6f5f626f C$A$GT$16into_bo
-  0x0000e3c0 7865645f 736c6963 65313768 37316534 xed_slice17h71e4
-  0x0000e3d0 34336266 34653837 36633932 45005f5f 43bf4e876c92E.__
-  0x0000e3e0 72646c5f 616c6c6f 63005f5a 4e34636f rdl_alloc._ZN4co
-  0x0000e3f0 7265336f 70733866 756e6374 696f6e36 re3ops8function6
-  0x0000e400 466e4f6e 63653430 63616c6c 5f6f6e63 FnOnce40call_onc
-  0x0000e410 65247537 62242475 37622476 7461626c e$u7b$$u7b$vtabl
-  0x0000e420 652e7368 696d2475 37642424 75376424 e.shim$u7d$$u7d$
-  0x0000e430 31376865 66613165 33653339 36306430 17hefa1e3e3960d0
-  0x0000e440 34373845 2e6c6c76 6d2e3331 36303930 478E.llvm.316090
-  0x0000e450 37323831 38383037 38313132 33006673 7281880781123.fs
-  0x0000e460 74617436 34005f5a 4e337374 64367468 tat64._ZN3std6th
-  0x0000e470 72656164 356c6f63 616c3466 61737431 read5local4fast1
-  0x0000e480 324b6579 244c5424 54244754 24313474 2Key$LT$T$GT$14t
-  0x0000e490 72795f69 6e697469 616c697a 65313768 ry_initialize17h
-  0x0000e4a0 34303537 30363065 33363831 35386434 4057060e368158d4
-  0x0000e4b0 452e6c6c 766d2e31 31343939 39373739 E.llvm.114999779
-  0x0000e4c0 39393837 30343439 31363100 5f5a4e38 99870449161._ZN8
-  0x0000e4d0 315f244c 54247079 6f332e2e 65786365 1_$LT$pyo3..exce
-  0x0000e4e0 7074696f 6e732e2e 5079436f 6e6e6563 ptions..PyConnec
-  0x0000e4f0 74696f6e 41626f72 74656445 72726f72 tionAbortedError
-  0x0000e500 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000e510 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x0000e520 54243366 6d743137 68636466 36383965 T$3fmt17hcdf689e
-  0x0000e530 38346438 33303533 3145005f 5a4e3638 84d830531E._ZN68
-  0x0000e540 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
-  0x0000e550 74696f6e 732e2e50 79537973 74656d45 tions..PySystemE
-  0x0000e560 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x0000e570 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x0000e580 24475424 33666d74 31376836 35343838 $GT$3fmt17h65488
-  0x0000e590 32316362 34396633 34636145 005f5a4e 21cb49f34caE._ZN
-  0x0000e5a0 34636f72 6533666d 7439466f 726d6174 4core3fmt9Format
-  0x0000e5b0 74657231 35646562 75675f75 70706572 ter15debug_upper
-  0x0000e5c0 5f686578 31376834 61653561 64346636 _hex17h4ae5ad4f6
-  0x0000e5d0 66326161 31643045 005f5a4e 38305f24 f2aa1d0E._ZN80_$
-  0x0000e5e0 4c542473 74642e2e 696f2e2e 57726974 LT$std..io..Writ
-  0x0000e5f0 652e2e77 72697465 5f666d74 2e2e4164 e..write_fmt..Ad
-  0x0000e600 61707465 72244c54 24542447 54242475 apter$LT$T$GT$$u
-  0x0000e610 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x0000e620 666d742e 2e577269 74652447 54243977 fmt..Write$GT$9w
-  0x0000e630 72697465 5f737472 31376861 39626534 rite_str17ha9be4
-  0x0000e640 36373639 63336238 35366645 005f5a4e 6769c3b856fE._ZN
-  0x0000e650 37335f24 4c542470 796f332e 2e657863 73_$LT$pyo3..exc
-  0x0000e660 65707469 6f6e732e 2e507952 756e7469 eptions..PyRunti
-  0x0000e670 6d655761 726e696e 67247532 30246173 meWarning$u20$as
-  0x0000e680 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x0000e690 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x0000e6a0 37683961 36653338 62303735 65333539 7h9a6e38b075e359
-  0x0000e6b0 33384500 616e6f6e 2e396531 31346564 38E.anon.9e114ed
-  0x0000e6c0 35303130 64363235 33626432 36313132 5010d6253bd26112
-  0x0000e6d0 39343733 63643138 382e322e 6c6c766d 9473cd188.2.llvm
-  0x0000e6e0 2e383336 34373335 31373237 30333437 .836473517270347
-  0x0000e6f0 36333534 00616e6f 6e2e6539 31333664 6354.anon.e9136d
-  0x0000e700 34636332 66326266 37333364 35393262 4cc2f2bf733d592b
-  0x0000e710 35646638 38393532 30372e32 2e6c6c76 5df8895207.2.llv
-  0x0000e720 6d2e3137 33363837 35343234 30343638 m.17368754240468
-  0x0000e730 30333335 3630005f 5a4e3470 796f3335 033560._ZN4pyo35
-  0x0000e740 74797065 73367374 72696e67 38507953 types6string8PyS
-  0x0000e750 7472696e 67336e65 77313768 32393939 tring3new17h2999
-  0x0000e760 35396564 64343033 32316132 45005f5a 59edd40321a2E._Z
-  0x0000e770 4e36395f 244c5424 636f7265 2e2e616c N69_$LT$core..al
-  0x0000e780 6c6f632e 2e6c6179 6f75742e 2e4c6179 loc..layout..Lay
-  0x0000e790 6f757445 72726f72 24753230 24617324 outError$u20$as$
-  0x0000e7a0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x0000e7b0 65627567 24475424 33666d74 31376830 ebug$GT$3fmt17h0
-  0x0000e7c0 35666339 30343536 61333735 35316645 5fc90456a37551fE
-  0x0000e7d0 005f5a4e 37325f24 4c542424 52462473 ._ZN72_$LT$$RF$s
-  0x0000e7e0 74722475 32302461 73247532 3024616c tr$u20$as$u20$al
-  0x0000e7f0 6c6f632e 2e666669 2e2e635f 7374722e loc..ffi..c_str.
-  0x0000e800 2e435374 72696e67 2e2e6e65 772e2e53 .CString..new..S
-  0x0000e810 7065634e 6577496d 706c2447 54243133 pecNewImpl$GT$13
-  0x0000e820 73706563 5f6e6577 5f696d70 6c313768 spec_new_impl17h
-  0x0000e830 34663633 63626635 35646136 63396266 4f63cbf55da6c9bf
-  0x0000e840 45005f5a 4e34636f 72653573 6c696365 E._ZN4core5slice
-  0x0000e850 32395f24 4c542469 6d706c24 75323024 29_$LT$impl$u20$
-  0x0000e860 24753562 24542475 35642424 47542431 $u5b$T$u5d$$GT$1
-  0x0000e870 35636f70 795f6672 6f6d5f73 6c696365 5copy_from_slice
-  0x0000e880 31376c65 6e5f6d69 736d6174 63685f66 17len_mismatch_f
-  0x0000e890 61696c31 37683537 34313834 30343130 ail17h5741840410
-  0x0000e8a0 32376166 65654500 5f5a4e36 345f244c 27afeeE._ZN64_$L
-  0x0000e8b0 54247374 642e2e73 79732e2e 756e6978 T$std..sys..unix
-  0x0000e8c0 2e2e7374 64696f2e 2e537464 65727224 ..stdio..Stderr$
-  0x0000e8d0 75323024 61732475 32302473 74642e2e u20$as$u20$std..
-  0x0000e8e0 696f2e2e 57726974 65244754 24357772 io..Write$GT$5wr
-  0x0000e8f0 69746531 37686263 35343161 63613961 ite17hbc541aca9a
-  0x0000e900 38333935 32354500 5f5a4e34 70796f33 839525E._ZN4pyo3
-  0x0000e910 3473796e 63323047 494c4f6e 63654365 4sync20GILOnceCe
-  0x0000e920 6c6c244c 54245424 47542434 696e6974 ll$LT$T$GT$4init
-  0x0000e930 31376866 37353966 36666232 61396561 17hf759f6fb2a9ea
-  0x0000e940 38643545 005f5a4e 3470796f 33336769 8d5E._ZN4pyo33gi
-  0x0000e950 6c313472 65676973 7465725f 6f776e65 l14register_owne
-  0x0000e960 64313768 65303736 38316361 61663033 d17he07681caaf03
-  0x0000e970 31613838 45005f5a 4e37325f 244c5424 1a88E._ZN72_$LT$
-  0x0000e980 70796f33 2e2e7479 7065732e 2e627974 pyo3..types..byt
-  0x0000e990 65617272 61792e2e 50794279 74654172 earray..PyByteAr
-  0x0000e9a0 72617924 75323024 61732475 32302463 ray$u20$as$u20$c
-  0x0000e9b0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x0000e9c0 47542433 666d7431 37683965 64363934 GT$3fmt17h9ed694
-  0x0000e9d0 39393231 64376637 34304500 5f5a4e31 9921d7f740E._ZN1
-  0x0000e9e0 36706172 6b696e67 5f6c6f74 5f636f72 6parking_lot_cor
-  0x0000e9f0 6539776f 72645f6c 6f636b38 576f7264 e9word_lock8Word
-  0x0000ea00 4c6f636b 396c6f63 6b5f736c 6f773137 Lock9lock_slow17
-  0x0000ea10 68613837 38356230 30646432 66633664 ha8785b00dd2fc6d
-  0x0000ea20 3445005f 5a4e3631 5f244c54 24737464 4E._ZN61_$LT$std
-  0x0000ea30 2e2e696f 2e2e7374 64696f2e 2e537464 ..io..stdio..Std
-  0x0000ea40 6572724c 6f636b24 75323024 61732475 errLock$u20$as$u
-  0x0000ea50 32302473 74642e2e 696f2e2e 57726974 20$std..io..Writ
-  0x0000ea60 65244754 24397772 6974655f 616c6c31 e$GT$9write_all1
-  0x0000ea70 37683335 34613764 34343966 31303166 7h354a7d449f101f
-  0x0000ea80 31304500 5f5a4e35 616c6c6f 6333666d 10E._ZN5alloc3fm
-  0x0000ea90 7436666f 726d6174 3132666f 726d6174 t6format12format
-  0x0000eaa0 5f696e6e 65723137 68623861 37636339 _inner17hb8a7cc9
-  0x0000eab0 65616436 34646639 3245005f 5a4e3634 ead64df92E._ZN64
-  0x0000eac0 5f244c54 24616c6c 6f632e2e 6666692e _$LT$alloc..ffi.
-  0x0000ead0 2e635f73 74722e2e 4e756c45 72726f72 .c_str..NulError
-  0x0000eae0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000eaf0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x0000eb00 33666d74 31376833 32303638 31303161 3fmt17h32068101a
-  0x0000eb10 61653534 37343945 005f5a4e 34636f72 ae54749E._ZN4cor
-  0x0000eb20 6533666d 74386275 696c6465 72733131 e3fmt8builders11
-  0x0000eb30 44656275 67537472 75637436 66696e69 DebugStruct6fini
-  0x0000eb40 73683137 68323638 34626234 65623733 sh17h2684bb4eb73
-  0x0000eb50 33623862 65450072 7573745f 70616e69 3b8beE.rust_pani
-  0x0000eb60 63005f5a 4e313472 75737463 5f64656d c._ZN14rustc_dem
-  0x0000eb70 616e676c 65384465 6d616e67 6c653661 angle8Demangle6a
-  0x0000eb80 735f7374 72313768 37616339 65353632 s_str17h7ac9e562
-  0x0000eb90 38646665 32376234 45005f5a 4e39315f 8dfe27b4E._ZN91_
-  0x0000eba0 244c5424 7374642e 2e70616e 69636b69 $LT$std..panicki
-  0x0000ebb0 6e672e2e 62656769 6e5f7061 6e69632e ng..begin_panic.
-  0x0000ebc0 2e50616e 69635061 796c6f61 64244c54 .PanicPayload$LT
-  0x0000ebd0 24412447 54242475 32302461 73247532 $A$GT$$u20$as$u2
-  0x0000ebe0 3024636f 72652e2e 70616e69 632e2e42 0$core..panic..B
-  0x0000ebf0 6f784d65 55702447 54243367 65743137 oxMeUp$GT$3get17
-  0x0000ec00 68373731 35346230 61343762 30326630 h77154b0a47b02f0
-  0x0000ec10 3545005f 5a4e3463 6f726533 666d7439 5E._ZN4core3fmt9
-  0x0000ec20 466f726d 61747465 7239616c 7465726e Formatter9altern
-  0x0000ec30 61746531 37683161 33383035 64313133 ate17h1a3805d113
-  0x0000ec40 62393030 37664500 5f5a4e33 365f244c b9007fE._ZN36_$L
-  0x0000ec50 54245424 75323024 61732475 32302463 T$T$u20$as$u20$c
-  0x0000ec60 6f72652e 2e616e79 2e2e416e 79244754 ore..any..Any$GT
-  0x0000ec70 24377479 70655f69 64313768 33623232 $7type_id17h3b22
-  0x0000ec80 35366561 66356232 64383634 45005f5a 56eaf5b2d864E._Z
-  0x0000ec90 4e34636f 72653370 74723730 64726f70 N4core3ptr70drop
-  0x0000eca0 5f696e5f 706c6163 65244c54 2470796f _in_place$LT$pyo
-  0x0000ecb0 332e2e69 6e737461 6e63652e 2e507924 3..instance..Py$
-  0x0000ecc0 4c542470 796f332e 2e747970 65732e2e LT$pyo3..types..
-  0x0000ecd0 616e792e 2e507941 6e792447 54242447 any..PyAny$GT$$G
-  0x0000ece0 54243137 68386365 62613632 64626230 T$17h8ceba62dbb0
-  0x0000ecf0 38346538 61452e6c 6c766d2e 31313934 84e8aE.llvm.1194
-  0x0000ed00 30363231 33363735 36303636 32383035 0621367560662805
-  0x0000ed10 005f5a4e 33737464 33737973 34756e69 ._ZN3std3sys4uni
-  0x0000ed20 78326673 31326361 6e6f6e69 63616c69 x2fs12canonicali
-  0x0000ed30 7a653137 68626237 61393737 65613335 ze17hbb7a977ea35
-  0x0000ed40 39363830 3645005f 5a4e3637 5f244c54 96806E._ZN67_$LT
-  0x0000ed50 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x0000ed60 732e2e50 79454f46 4572726f 72247532 s..PyEOFError$u2
-  0x0000ed70 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x0000ed80 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x0000ed90 666d7431 37683636 33303163 64623531 fmt17h66301cdb51
-  0x0000eda0 64313434 63644500 616e6f6e 2e333437 d144cdE.anon.347
-  0x0000edb0 64323634 65333465 62336130 63373462 d264e34eb3a0c74b
-  0x0000edc0 65356138 39663839 35616337 652e3138 e5a89f895ac7e.18
-  0x0000edd0 2e6c6c76 6d2e3137 36393537 36323334 .llvm.1769576234
-  0x0000ede0 31373831 34353330 3132005f 5a4e3470 1781453012._ZN4p
-  0x0000edf0 796f3335 74797065 73313074 7970656f yo35types10typeo
-  0x0000ee00 626a6563 74365079 54797065 346e616d bject6PyType4nam
-  0x0000ee10 65313768 65656233 35616339 39333364 e17heeb35ac9933d
-  0x0000ee20 34383064 45005f5a 4e37385f 244c5424 480dE._ZN78_$LT$
-  0x0000ee30 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x0000ee40 2e2e6173 796e6369 6f2e2e43 616e6365 ..asyncio..Cance
-  0x0000ee50 6c6c6564 4572726f 72247532 30246173 lledError$u20$as
-  0x0000ee60 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x0000ee70 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
-  0x0000ee80 39396130 34353038 65656462 37656232 99a04508eedb7eb2
-  0x0000ee90 4500616e 6f6e2e39 65313134 65643530 E.anon.9e114ed50
-  0x0000eea0 31306436 32353362 64323631 31323934 10d6253bd2611294
-  0x0000eeb0 37336364 3138382e 332e6c6c 766d2e38 73cd188.3.llvm.8
-  0x0000eec0 33363437 33353137 32373033 34373633 3647351727034763
-  0x0000eed0 3534005f 5a4e3463 6f726539 70616e69 54._ZN4core9pani
-  0x0000eee0 636b696e 67313970 616e6963 5f63616e cking19panic_can
-  0x0000eef0 6e6f745f 756e7769 6e643137 68643132 not_unwind17hd12
-  0x0000ef00 33643963 37313437 33646364 6145005f 3d9c71473dcdaE._
-  0x0000ef10 5a4e3537 5f244c54 24636f72 652e2e66 ZN57_$LT$core..f
-  0x0000ef20 6d742e2e 466f726d 61747465 72247532 mt..Formatter$u2
-  0x0000ef30 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x0000ef40 6d742e2e 57726974 65244754 24397772 mt..Write$GT$9wr
-  0x0000ef50 6974655f 73747231 37683331 37633462 ite_str17h317c4b
-  0x0000ef60 65626232 39376634 30314500 5f5a4e34 ebb297f401E._ZN4
-  0x0000ef70 70796f33 33657272 35507945 7272386e pyo33err5PyErr8n
-  0x0000ef80 65775f74 79706531 37686164 35633331 ew_type17had5c31
-  0x0000ef90 61356364 31306533 38304500 5f474c4f a5cd10e380E._GLO
-  0x0000efa0 42414c5f 4f464653 45545f54 41424c45 BAL_OFFSET_TABLE
-  0x0000efb0 5f00616e 6f6e2e65 39656232 33376366 _.anon.e9eb237cf
-  0x0000efc0 35306134 33623635 64363336 62306634 50a43b65d636b0f4
-  0x0000efd0 37373062 3034652e 33322e6c 6c766d2e 770b04e.32.llvm.
-  0x0000efe0 31333836 31383532 37313133 39303237 1386185271139027
-  0x0000eff0 34373600 5f5a4e34 70796f33 31317479 476._ZN4pyo311ty
-  0x0000f000 70655f6f 626a6563 74313050 79547970 pe_object10PyTyp
-  0x0000f010 65496e66 6f313174 7970655f 6f626a65 eInfo11type_obje
-  0x0000f020 63743137 68313466 35633735 65373436 ct17h14f5c75e746
-  0x0000f030 38623339 3145005f 5a4e3638 5f244c54 8b391E._ZN68_$LT
-  0x0000f040 2470796f 332e2e74 79706573 2e2e7479 $pyo3..types..ty
-  0x0000f050 70656f62 6a656374 2e2e5079 54797065 peobject..PyType
-  0x0000f060 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000f070 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x0000f080 33666d74 31376833 31356438 38613537 3fmt17h315d88a57
-  0x0000f090 34363133 31333945 005f5a4e 33737464 4613139E._ZN3std
-  0x0000f0a0 33737973 34756e69 78313461 626f7274 3sys4unix14abort
-  0x0000f0b0 5f696e74 65726e61 6c313768 65623237 _internal17heb27
-  0x0000f0c0 65616365 65363666 62383466 45005f5a eacee66fb84fE._Z
-  0x0000f0d0 4e34636f 7265336e 756d3632 5f244c54 N4core3num62_$LT
-  0x0000f0e0 24696d70 6c247532 3024636f 72652e2e $impl$u20$core..
-  0x0000f0f0 7374722e 2e747261 6974732e 2e46726f str..traits..Fro
-  0x0000f100 6d537472 24753230 24666f72 24753230 mStr$u20$for$u20
-  0x0000f110 24757369 7a652447 54243866 726f6d5f $usize$GT$8from_
-  0x0000f120 73747231 37683633 30646439 30333965 str17h630dd9039e
-  0x0000f130 35343633 64384500 5f5a4e34 345f244c 5463d8E._ZN44_$L
-  0x0000f140 54242452 46245424 75323024 61732475 T$$RF$T$u20$as$u
-  0x0000f150 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
-  0x0000f160 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
-  0x0000f170 34656330 39643732 63366463 31393339 4ec09d72c6dc1939
-  0x0000f180 45005f5a 4e37325f 244c5424 636f7265 E._ZN72_$LT$core
-  0x0000f190 2e2e6e75 6d2e2e65 72726f72 2e2e5472 ..num..error..Tr
-  0x0000f1a0 7946726f 6d496e74 4572726f 72247532 yFromIntError$u2
-  0x0000f1b0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x0000f1c0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x0000f1d0 666d7431 37683138 36333934 37366334 fmt17h18639476c4
-  0x0000f1e0 31336165 39664500 5f5a4e36 305f244c 13ae9fE._ZN60_$L
-  0x0000f1f0 5424616c 6c6f632e 2e737472 696e672e T$alloc..string.
-  0x0000f200 2e537472 696e6724 75323024 61732475 .String$u20$as$u
-  0x0000f210 32302463 6f72652e 2e636c6f 6e652e2e 20$core..clone..
-  0x0000f220 436c6f6e 65244754 2435636c 6f6e6531 Clone$GT$5clone1
-  0x0000f230 37686430 30306434 62643335 35373932 7hd000d4bd355792
-  0x0000f240 35644500 5f5a4e34 70796f33 35747970 5dE._ZN4pyo35typ
-  0x0000f250 65733361 6e793550 79416e79 37736574 es3any5PyAny7set
-  0x0000f260 61747472 31376836 62383338 62363761 attr17h6b838b67a
-  0x0000f270 33663836 33363145 005f5a4e 33737464 3f86361E._ZN3std
-  0x0000f280 3770726f 63657373 3561626f 72743137 7process5abort17
-  0x0000f290 68366135 37333166 38316438 32666436 h6a5731f81d82fd6
-  0x0000f2a0 3345005f 5a4e3561 6c6c6f63 3473796e 3E._ZN5alloc4syn
-  0x0000f2b0 63333261 7263696e 6e65725f 6c61796f c32arcinner_layo
-  0x0000f2c0 75745f66 6f725f76 616c7565 5f6c6179 ut_for_value_lay
-  0x0000f2d0 6f757431 37683239 65626461 66383335 out17h29ebdaf835
-  0x0000f2e0 39353736 35344500 5f5a4e33 73746434 957654E._ZN3std4
-  0x0000f2f0 74696d65 37496e73 74616e74 336e6f77 time7Instant3now
-  0x0000f300 31376837 62313336 39636339 66633435 17h7b1369cc9fc45
-  0x0000f310 33643945 00616e6f 6e2e3334 37643236 3d9E.anon.347d26
-  0x0000f320 34653334 65623361 30633734 62653561 4e34eb3a0c74be5a
-  0x0000f330 38396638 39356163 37652e31 2e6c6c76 89f895ac7e.1.llv
-  0x0000f340 6d2e3137 36393537 36323334 31373831 m.17695762341781
-  0x0000f350 34353330 3132005f 5a4e3373 74643373 453012._ZN3std3s
-  0x0000f360 79733475 6e697831 37646563 6f64655f ys4unix17decode_
-  0x0000f370 6572726f 725f6b69 6e643137 68326164 error_kind17h2ad
-  0x0000f380 30326437 30373865 34396331 3045005f 02d7078e49c10E._
-  0x0000f390 5a4e3463 6f726533 70747234 3764726f ZN4core3ptr47dro
-  0x0000f3a0 705f696e 5f706c61 6365244c 5424636f p_in_place$LT$co
-  0x0000f3b0 72652e2e 63656c6c 2e2e426f 72726f77 re..cell..Borrow
-  0x0000f3c0 4d757445 72726f72 24475424 31376862 MutError$GT$17hb
-  0x0000f3d0 64653830 65616663 62376563 30326245 de80eafcb7ec02bE
-  0x0000f3e0 2e6c6c76 6d2e3137 36393537 36323334 .llvm.1769576234
-  0x0000f3f0 31373831 34353330 3132005f 5a4e3639 1781453012._ZN69
-  0x0000f400 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
-  0x0000f410 74696f6e 732e2e50 7956616c 75654572 tions..PyValueEr
-  0x0000f420 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x0000f430 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
-  0x0000f440 79244754 2433666d 74313768 38313564 y$GT$3fmt17h815d
-  0x0000f450 39643430 39353930 30336564 4500616e 9d40959003edE.an
-  0x0000f460 6f6e2e62 39613034 38366330 30613431 on.b9a0486c00a41
-  0x0000f470 37326237 62316163 35326233 31356161 72b7b1ac52b315aa
-  0x0000f480 3461332e 34312e6c 6c766d2e 31333233 4a3.41.llvm.1323
-  0x0000f490 38383933 34333232 30303639 32323236 8893432200692226
-  0x0000f4a0 005f5a4e 35335f24 4c542454 24753230 ._ZN53_$LT$T$u20
-  0x0000f4b0 24617324 75323024 70796f33 2e2e636f $as$u20$pyo3..co
-  0x0000f4c0 6e766572 73696f6e 2e2e4672 6f6d5079 nversion..FromPy
-  0x0000f4d0 506f696e 74657224 47542432 3166726f Pointer$GT$21fro
-  0x0000f4e0 6d5f6f77 6e65645f 7074725f 6f725f6f m_owned_ptr_or_o
-  0x0000f4f0 70743137 68393437 66623033 65643632 pt17h947fb03ed62
-  0x0000f500 62313463 37452e6c 6c766d2e 31333233 b14c7E.llvm.1323
-  0x0000f510 38383933 34333232 30303639 32323236 8893432200692226
-  0x0000f520 005f5a4e 37315f24 4c542470 796f332e ._ZN71_$LT$pyo3.
-  0x0000f530 2e657863 65707469 6f6e732e 2e507952 .exceptions..PyR
-  0x0000f540 756e7469 6d654572 726f7224 75323024 untimeError$u20$
-  0x0000f550 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x0000f560 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
-  0x0000f570 74313768 33623235 66663333 31613961 t17h3b25ff331a9a
-  0x0000f580 64323733 45005f5a 4e34636f 72653370 d273E._ZN4core3p
-  0x0000f590 74723736 64726f70 5f696e5f 706c6163 tr76drop_in_plac
-  0x0000f5a0 65244c54 2470796f 332e2e69 6e737461 e$LT$pyo3..insta
-  0x0000f5b0 6e63652e 2e507924 4c542470 796f332e nce..Py$LT$pyo3.
-  0x0000f5c0 2e747970 65732e2e 73747269 6e672e2e .types..string..
-  0x0000f5d0 50795374 72696e67 24475424 24475424 PyString$GT$$GT$
-  0x0000f5e0 31376863 33333937 36383762 33306431 17hc3397687b30d1
-  0x0000f5f0 39333345 2e6c6c76 6d2e3131 32313338 933E.llvm.112138
-  0x0000f600 38393736 33363035 36333334 3933005f 89763605633493._
-  0x0000f610 5a4e3638 5f244c54 2470796f 332e2e65 ZN68_$LT$pyo3..e
-  0x0000f620 78636570 74696f6e 732e2e50 79557365 xceptions..PyUse
-  0x0000f630 72576172 6e696e67 24753230 24617324 rWarning$u20$as$
-  0x0000f640 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x0000f650 65627567 24475424 33666d74 31376830 ebug$GT$3fmt17h0
-  0x0000f660 32616461 61656139 63623265 36343645 2adaaea9cb2e646E
-  0x0000f670 005f5a4e 34636f72 6533666d 74336e75 ._ZN4core3fmt3nu
-  0x0000f680 6d35335f 244c5424 696d706c 24753230 m53_$LT$impl$u20
-  0x0000f690 24636f72 652e2e66 6d742e2e 55707065 $core..fmt..Uppe
-  0x0000f6a0 72486578 24753230 24666f72 24753230 rHex$u20$for$u20
-  0x0000f6b0 24753634 24475424 33666d74 31376830 $u64$GT$3fmt17h0
-  0x0000f6c0 39626438 62636366 36343138 30333045 9bd8bccf6418030E
-  0x0000f6d0 005f5a4e 3470796f 33357479 70657334 ._ZN4pyo35types4
-  0x0000f6e0 6c697374 3650794c 69737436 61707065 list6PyList6appe
-  0x0000f6f0 6e643137 68336166 32363934 33343762 nd17h3af2694347b
-  0x0000f700 65333965 6645005f 5a4e3830 5f244c54 e39efE._ZN80_$LT
-  0x0000f710 24737464 2e2e7061 74682e2e 436f6d70 $std..path..Comp
-  0x0000f720 6f6e656e 74732475 32302461 73247532 onents$u20$as$u2
-  0x0000f730 3024636f 72652e2e 69746572 2e2e7472 0$core..iter..tr
-  0x0000f740 61697473 2e2e6974 65726174 6f722e2e aits..iterator..
-  0x0000f750 49746572 61746f72 24475424 346e6578 Iterator$GT$4nex
-  0x0000f760 74313768 64316632 35666134 30353535 t17hd1f25fa40555
-  0x0000f770 32366135 4500616e 6f6e2e36 39623664 26a5E.anon.69b6d
-  0x0000f780 39366338 63363564 37393439 33333135 96c8c65d79493315
-  0x0000f790 39643566 62393134 3339622e 31332e6c 9d5fb91439b.13.l
-  0x0000f7a0 6c766d2e 35363830 36333734 36323237 lvm.568063746227
-  0x0000f7b0 35353338 37363200 5f5a4e34 70796f33 5538762._ZN4pyo3
-  0x0000f7c0 35696d70 6c5f3136 65787472 6163745f 5impl_16extract_
-  0x0000f7d0 61726775 6d656e74 31394675 6e637469 argument19Functi
-  0x0000f7e0 6f6e4465 73637269 7074696f 6e33346d onDescription34m
-  0x0000f7f0 69737369 6e675f72 65717569 7265645f issing_required_
-  0x0000f800 6b657977 6f72645f 61726775 6d656e74 keyword_argument
-  0x0000f810 73313768 39616163 38323661 37646637 s17h9aac826a7df7
-  0x0000f820 39346331 45005f5a 4e34636f 72653970 94c1E._ZN4core9p
-  0x0000f830 616e6963 6b696e67 31347061 6e69635f anicking14panic_
-  0x0000f840 6e6f756e 77696e64 31376833 65623361 nounwind17h3eb3a
-  0x0000f850 39366265 65396565 32343245 005f5f72 96bee9ee242E.__r
-  0x0000f860 7573745f 64726f70 5f70616e 6963005f ust_drop_panic._
-  0x0000f870 5a4e3738 5f244c54 2470796f 332e2e65 ZN78_$LT$pyo3..e
-  0x0000f880 78636570 74696f6e 732e2e50 794e6f74 xceptions..PyNot
-  0x0000f890 496d706c 656d656e 74656445 72726f72 ImplementedError
-  0x0000f8a0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000f8b0 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x0000f8c0 54243366 6d743137 68363935 32653638 T$3fmt17h6952e68
-  0x0000f8d0 65663837 39666164 6545005f 5a4e3470 ef879fadeE._ZN4p
-  0x0000f8e0 796f3335 696d706c 5f313665 78747261 yo35impl_16extra
-  0x0000f8f0 63745f61 7267756d 656e7431 3946756e ct_argument19Fun
-  0x0000f900 6374696f 6e446573 63726970 74696f6e ctionDescription
-  0x0000f910 32386d75 6c746970 6c655f76 616c7565 28multiple_value
-  0x0000f920 735f666f 725f6172 67756d65 6e743137 s_for_argument17
-  0x0000f930 68316464 30383061 37636435 64633930 h1dd080a7cd5dc90
-  0x0000f940 3145005f 5a4e3470 796f3335 74797065 1E._ZN4pyo35type
-  0x0000f950 73366d6f 64756c65 3850794d 6f64756c s6module8PyModul
-  0x0000f960 65313261 64645f66 756e6374 696f6e31 e12add_function1
-  0x0000f970 37686361 38636639 35666261 33616361 7hca8cf95fba3aca
-  0x0000f980 61654500 5f5a4e39 355f244c 54247374 aeE._ZN95_$LT$st
-  0x0000f990 642e2e70 6174682e 2e436f6d 706f6e65 d..path..Compone
-  0x0000f9a0 6e747324 75323024 61732475 32302463 nts$u20$as$u20$c
-  0x0000f9b0 6f72652e 2e697465 722e2e74 72616974 ore..iter..trait
-  0x0000f9c0 732e2e64 6f75626c 655f656e 6465642e s..double_ended.
-  0x0000f9d0 2e446f75 626c6545 6e646564 49746572 .DoubleEndedIter
-  0x0000f9e0 61746f72 24475424 396e6578 745f6261 ator$GT$9next_ba
-  0x0000f9f0 636b3137 68303865 34653936 31393864 ck17h08e4e96198d
-  0x0000fa00 32393632 3345005f 5a4e3734 5f244c54 29623E._ZN74_$LT
-  0x0000fa10 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x0000fa20 732e2e50 7946696c 65457869 73747345 s..PyFileExistsE
-  0x0000fa30 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x0000fa40 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x0000fa50 61792447 54243366 6d743137 68323035 ay$GT$3fmt17h205
-  0x0000fa60 38663364 38663065 35366637 6545005f 8f3d8f0e56f7eE._
-  0x0000fa70 5a4e3634 5f244c54 24737464 2e2e7061 ZN64_$LT$std..pa
-  0x0000fa80 74682e2e 53747269 70507265 66697845 th..StripPrefixE
-  0x0000fa90 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x0000faa0 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x0000fab0 24475424 33666d74 31376832 65363431 $GT$3fmt17h2e641
-  0x0000fac0 33653938 33313137 31386145 005f5a4e 3e98311718aE._ZN
-  0x0000fad0 3132305f 244c5424 70796f33 2e2e6465 120_$LT$pyo3..de
-  0x0000fae0 72697665 5f757469 6c732e2e 50794675 rive_utils..PyFu
-  0x0000faf0 6e637469 6f6e4172 67756d65 6e747324 nctionArguments$
-  0x0000fb00 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x0000fb10 2e636f6e 76657274 2e2e4672 6f6d244c .convert..From$L
-  0x0000fb20 54242452 46247079 6f332e2e 74797065 T$$RF$pyo3..type
-  0x0000fb30 732e2e6d 6f64756c 652e2e50 794d6f64 s..module..PyMod
-  0x0000fb40 756c6524 47542424 47542434 66726f6d ule$GT$$GT$4from
-  0x0000fb50 31376830 64313535 36636561 32646362 17h0d1556cea2dcb
-  0x0000fb60 36393645 005f5a4e 37305f24 4c542470 696E._ZN70_$LT$p
-  0x0000fb70 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x0000fb80 2e507953 746f7049 74657261 74696f6e .PyStopIteration
-  0x0000fb90 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000fba0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x0000fbb0 33666d74 31376835 35353137 38373661 3fmt17h55517876a
-  0x0000fbc0 34383164 65613845 005f5a4e 34636f72 481dea8E._ZN4cor
-  0x0000fbd0 65337074 72313131 64726f70 5f696e5f e3ptr111drop_in_
-  0x0000fbe0 706c6163 65244c54 2470796f 332e2e65 place$LT$pyo3..e
-  0x0000fbf0 72722e2e 6572725f 73746174 652e2e62 rr..err_state..b
-  0x0000fc00 6f786564 5f617267 73244c54 24616c6c oxed_args$LT$all
-  0x0000fc10 6f632e2e 73747269 6e672e2e 53747269 oc..string..Stri
-  0x0000fc20 6e672447 54242e2e 24753762 24247537 ng$GT$..$u7b$$u7
-  0x0000fc30 6224636c 6f737572 65247537 64242475 b$closure$u7d$$u
-  0x0000fc40 37642424 47542431 37683365 39616439 7d$$GT$17h3e9ad9
-  0x0000fc50 64383162 61326138 3737452e 6c6c766d d81ba2a877E.llvm
-  0x0000fc60 2e333136 30393037 32383138 38303738 .316090728188078
-  0x0000fc70 31313233 005f5a4e 3567696d 6c693472 1123._ZN5gimli4r
-  0x0000fc80 65616436 61626272 65763133 41626272 ead6abbrev13Abbr
-  0x0000fc90 65766961 74696f6e 7336696e 73657274 eviations6insert
-  0x0000fca0 31376830 61373239 33663565 35356233 17h0a7293f5e55b3
-  0x0000fcb0 35353845 005f5a4e 34636f72 65357061 558E._ZN4core5pa
-  0x0000fcc0 6e696331 3070616e 69635f69 6e666f39 nic10panic_info9
-  0x0000fcd0 50616e69 63496e66 6f376d65 73736167 PanicInfo7messag
-  0x0000fce0 65313768 36636635 65383763 64346164 e17h6cf5e87cd4ad
-  0x0000fcf0 34353636 45005f5a 4e34636f 72653366 4566E._ZN4core3f
-  0x0000fd00 6d743946 6f726d61 74746572 33706164 mt9Formatter3pad
-  0x0000fd10 31376865 35303162 33643937 66656564 17he501b3d97feed
-  0x0000fd20 64306645 005f5a4e 39385f24 4c542461 d0fE._ZN98_$LT$a
-  0x0000fd30 6c6c6f63 2e2e7665 632e2e56 6563244c lloc..vec..Vec$L
-  0x0000fd40 54245424 47542424 75323024 61732475 T$T$GT$$u20$as$u
-  0x0000fd50 32302461 6c6c6f63 2e2e7665 632e2e73 20$alloc..vec..s
-  0x0000fd60 7065635f 66726f6d 5f697465 722e2e53 pec_from_iter..S
-  0x0000fd70 70656346 726f6d49 74657224 4c542454 pecFromIter$LT$T
-  0x0000fd80 24432449 24475424 24475424 3966726f $C$I$GT$$GT$9fro
-  0x0000fd90 6d5f6974 65723137 68623636 34613762 m_iter17hb664a7b
-  0x0000fda0 37656265 62346433 3345005f 5a4e3561 7ebeb4d33E._ZN5a
-  0x0000fdb0 6c6c6f63 35616c6c 6f633862 6f785f66 lloc5alloc8box_f
-  0x0000fdc0 72656531 37683938 32656236 66623536 ree17h982eb6fb56
-  0x0000fdd0 65613866 3936452e 6c6c766d 2e383336 ea8f96E.llvm.836
-  0x0000fde0 34373335 31373237 30333437 36333534 4735172703476354
-  0x0000fdf0 005f5a4e 38305f24 4c542470 796f332e ._ZN80_$LT$pyo3.
-  0x0000fe00 2e657863 65707469 6f6e732e 2e507955 .exceptions..PyU
-  0x0000fe10 6e69636f 64655472 616e736c 61746545 nicodeTranslateE
-  0x0000fe20 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x0000fe30 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x0000fe40 61792447 54243366 6d743137 68313037 ay$GT$3fmt17h107
-  0x0000fe50 35373633 38316339 61316363 62450061 576381c9a1ccbE.a
-  0x0000fe60 6e6f6e2e 35313035 62646437 39663233 non.5105bdd79f23
-  0x0000fe70 62313137 31663338 37343266 65616163 b1171f38742feaac
-  0x0000fe80 35643137 2e34312e 6c6c766d 2e333136 5d17.41.llvm.316
-  0x0000fe90 30393037 32383138 38303738 31313233 0907281880781123
-  0x0000fea0 005f5a4e 3470796f 33336572 72396572 ._ZN4pyo33err9er
-  0x0000feb0 725f7374 61746531 30507945 72725374 r_state10PyErrSt
-  0x0000fec0 61746531 34696e74 6f5f6666 695f7475 ate14into_ffi_tu
-  0x0000fed0 706c6531 37683531 64356432 65346565 ple17h51d5d2e4ee
-  0x0000fee0 37353362 35364500 5f5a4e36 375f244c 753b56E._ZN67_$L
-  0x0000fef0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x0000ff00 6e732e2e 50795379 7374656d 45786974 ns..PySystemExit
-  0x0000ff10 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x0000ff20 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x0000ff30 33666d74 31376837 35316137 32666533 3fmt17h751a72fe3
-  0x0000ff40 66613932 63386145 005f5a4e 37345f24 fa92c8aE._ZN74_$
-  0x0000ff50 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x0000ff60 6f6e732e 2e507941 72697468 6d657469 ons..PyArithmeti
-  0x0000ff70 63457272 6f722475 32302461 73247532 cError$u20$as$u2
-  0x0000ff80 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
-  0x0000ff90 706c6179 24475424 33666d74 31376862 play$GT$3fmt17hb
-  0x0000ffa0 33383037 36626162 33356330 32346445 38076bab35c024dE
-  0x0000ffb0 005f5a4e 35335f24 4c542463 6f72652e ._ZN53_$LT$core.
-  0x0000ffc0 2e666d74 2e2e4572 726f7224 75323024 .fmt..Error$u20$
-  0x0000ffd0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x0000ffe0 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
-  0x0000fff0 37686266 36306533 66313662 38653235 7hbf60e3f16b8e25
-  0x00010000 65344500 5f5a4e36 345f244c 5424636f e4E._ZN64_$LT$co
-  0x00010010 72652e2e 7374722e 2e657272 6f722e2e re..str..error..
-  0x00010020 55746638 4572726f 72247532 30246173 Utf8Error$u20$as
-  0x00010030 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x00010040 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
-  0x00010050 37346165 62663162 61333331 66653230 74aebf1ba331fe20
-  0x00010060 45005f5a 4e347079 6f333569 6d706c5f E._ZN4pyo35impl_
-  0x00010070 3970796d 6574686f 64733136 65787472 9pymethods16extr
-  0x00010080 6163745f 635f7374 72696e67 31376864 act_c_string17hd
-  0x00010090 35643566 65333237 31666631 32373845 5d5fe3271ff1278E
-  0x000100a0 2e6c6c76 6d2e3536 39373932 39373639 .llvm.5697929769
-  0x000100b0 31333330 35373437 36005f5a 4e36395f 133057476._ZN69_
-  0x000100c0 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x000100d0 696f6e73 2e2e5079 52756e74 696d6545 ions..PyRuntimeE
-  0x000100e0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x000100f0 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00010100 24475424 33666d74 31376866 32316439 $GT$3fmt17hf21d9
-  0x00010110 38653832 31626435 33383445 005f5a4e 8e821bd5384E._ZN
-  0x00010120 34636f72 6533666d 74336e75 6d35325f 4core3fmt3num52_
-  0x00010130 244c5424 696d706c 24753230 24636f72 $LT$impl$u20$cor
-  0x00010140 652e2e66 6d742e2e 4c6f7765 72486578 e..fmt..LowerHex
-  0x00010150 24753230 24666f72 24753230 24693824 $u20$for$u20$i8$
-  0x00010160 47542433 666d7431 37683666 30613532 GT$3fmt17h6f0a52
-  0x00010170 32643333 32316462 34384500 5f5a4e36 2d3321db48E._ZN6
-  0x00010180 365f244c 54247079 6f332e2e 74797065 6_$LT$pyo3..type
-  0x00010190 732e2e73 7472696e 672e2e50 79537472 s..string..PyStr
-  0x000101a0 696e6724 75323024 61732475 32302463 ing$u20$as$u20$c
-  0x000101b0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x000101c0 47542433 666d7431 37686561 32346166 GT$3fmt17hea24af
-  0x000101d0 37376639 65336133 33314500 5f5a4e34 77f9e3a331E._ZN4
-  0x000101e0 70796f33 3367696c 34504f4f 4c313768 pyo33gil4POOL17h
-  0x000101f0 37393264 65306435 61626662 66656237 792de0d5abfbfeb7
-  0x00010200 4500616e 6f6e2e62 39613034 38366330 E.anon.b9a0486c0
-  0x00010210 30613431 37326237 62316163 35326233 0a4172b7b1ac52b3
-  0x00010220 31356161 3461332e 35322e6c 6c766d2e 15aa4a3.52.llvm.
-  0x00010230 31333233 38383933 34333232 30303639 1323889343220069
-  0x00010240 32323236 005f5f72 7573745f 6465616c 2226.__rust_deal
-  0x00010250 6c6f6300 616e6f6e 2e353130 35626464 loc.anon.5105bdd
-  0x00010260 37396632 33623131 37316633 38373432 79f23b1171f38742
-  0x00010270 66656161 63356431 372e3339 2e6c6c76 feaac5d17.39.llv
-  0x00010280 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x00010290 38313132 33005f5a 4e38315f 244c5424 81123._ZN81_$LT$
-  0x000102a0 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x000102b0 2e2e6173 796e6369 6f2e2e49 6e76616c ..asyncio..Inval
-  0x000102c0 69645374 61746545 72726f72 24753230 idStateError$u20
-  0x000102d0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x000102e0 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
-  0x000102f0 31376834 35633866 34666163 62623235 17h45c8f4facbb25
-  0x00010300 65383245 00616e6f 6e2e3531 30356264 e82E.anon.5105bd
-  0x00010310 64373966 32336231 31373166 33383734 d79f23b1171f3874
-  0x00010320 32666561 61633564 31372e33 382e6c6c 2feaac5d17.38.ll
-  0x00010330 766d2e33 31363039 30373238 31383830 vm.3160907281880
-  0x00010340 37383131 3233005f 5a4e3636 5f244c54 781123._ZN66_$LT
-  0x00010350 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00010360 732e2e50 79457863 65707469 6f6e2475 s..PyException$u
-  0x00010370 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00010380 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
-  0x00010390 6d743137 68396239 38336338 30313730 mt17h9b983c80170
-  0x000103a0 39326639 30450061 6e6f6e2e 62396130 92f90E.anon.b9a0
-  0x000103b0 34383663 30306134 31373262 37623161 486c00a4172b7b1a
-  0x000103c0 63353262 33313561 61346133 2e33342e c52b315aa4a3.34.
-  0x000103d0 6c6c766d 2e313332 33383839 33343332 llvm.13238893432
-  0x000103e0 32303036 39323232 36005f5a 4e347079 200692226._ZN4py
-  0x000103f0 6f333574 79706573 346c6973 74365079 o35types4list6Py
-  0x00010400 4c697374 336c656e 31376836 66396463 List3len17h6f9dc
-  0x00010410 36636535 34383866 34313245 005f5a4e 6ce5488f412E._ZN
-  0x00010420 34636f72 65337074 72313235 64726f70 4core3ptr125drop
-  0x00010430 5f696e5f 706c6163 65244c54 2470796f _in_place$LT$pyo
-  0x00010440 332e2e65 72722e2e 6572725f 73746174 3..err..err_stat
-  0x00010450 652e2e62 6f786564 5f617267 73244c54 e..boxed_args$LT
-  0x00010460 24636f72 652e2e6e 756d2e2e 64656332 $core..num..dec2
-  0x00010470 666c742e 2e506172 7365466c 6f617445 flt..ParseFloatE
-  0x00010480 72726f72 24475424 2e2e2475 37622424 rror$GT$..$u7b$$
-  0x00010490 75376224 636c6f73 75726524 75376424 u7b$closure$u7d$
-  0x000104a0 24753764 24244754 24313768 38653232 $u7d$$GT$17h8e22
-  0x000104b0 39643865 37393330 38623033 452e6c6c 9d8e79308b03E.ll
-  0x000104c0 766d2e33 31363039 30373238 31383830 vm.3160907281880
-  0x000104d0 37383131 3233005f 5a4e3463 6f726533 781123._ZN4core3
-  0x000104e0 666d7439 466f726d 61747465 72313164 fmt9Formatter11d
-  0x000104f0 65627567 5f747570 6c653137 68343739 ebug_tuple17h479
-  0x00010500 62343665 33353532 61653863 3245005f b46e3552ae8c2E._
-  0x00010510 5a4e3638 5f244c54 24737464 2e2e7468 ZN68_$LT$std..th
-  0x00010520 72656164 2e2e6c6f 63616c2e 2e416363 read..local..Acc
-  0x00010530 65737345 72726f72 24753230 24617324 essError$u20$as$
-  0x00010540 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00010550 65627567 24475424 33666d74 31376833 ebug$GT$3fmt17h3
-  0x00010560 66353965 63383536 34343434 31656445 f59ec85644441edE
-  0x00010570 00616e6f 6e2e6239 61303438 36633030 .anon.b9a0486c00
-  0x00010580 61343137 32623762 31616335 32623331 a4172b7b1ac52b31
-  0x00010590 35616134 61332e33 372e6c6c 766d2e31 5aa4a3.37.llvm.1
-  0x000105a0 33323338 38393334 33323230 30363932 3238893432200692
-  0x000105b0 32323600 5f5a4e34 636f7265 33707472 226._ZN4core3ptr
-  0x000105c0 31333264 726f705f 696e5f70 6c616365 132drop_in_place
-  0x000105d0 244c5424 636f7265 2e2e6365 6c6c2e2e $LT$core..cell..
-  0x000105e0 5265664d 7574244c 5424616c 6c6f632e RefMut$LT$alloc.
-  0x000105f0 2e766563 2e2e5665 63244c54 24636f72 .vec..Vec$LT$cor
-  0x00010600 652e2e70 74722e2e 6e6f6e5f 6e756c6c e..ptr..non_null
-  0x00010610 2e2e4e6f 6e4e756c 6c244c54 2470796f ..NonNull$LT$pyo
-  0x00010620 335f6666 692e2e6f 626a6563 742e2e50 3_ffi..object..P
-  0x00010630 794f626a 65637424 47542424 47542424 yObject$GT$$GT$$
-  0x00010640 47542424 47542431 37683733 66306565 GT$$GT$17h73f0ee
-  0x00010650 63356263 61353961 6233452e 6c6c766d c5bca59ab3E.llvm
-  0x00010660 2e313332 33383839 33343332 32303036 .132388934322006
-  0x00010670 39323232 36005f5a 4e37305f 244c5424 92226._ZN70_$LT$
-  0x00010680 636f7265 2e2e7061 6e69632e 2e6c6f63 core..panic..loc
-  0x00010690 6174696f 6e2e2e4c 6f636174 696f6e24 ation..Location$
-  0x000106a0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x000106b0 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
-  0x000106c0 2433666d 74313768 66636131 38333635 $3fmt17hfca18365
-  0x000106d0 61646234 34346263 45005f5a 4e337374 adb444bcE._ZN3st
-  0x000106e0 64397061 6e69636b 696e6731 31626567 d9panicking11beg
-  0x000106f0 696e5f70 616e6963 31376863 64613365 in_panic17hcda3e
-  0x00010700 32386334 35383366 35323045 005f5a4e 28c4583f520E._ZN
-  0x00010710 37345f24 4c542470 796f332e 2e657863 74_$LT$pyo3..exc
-  0x00010720 65707469 6f6e732e 2e507943 6f6e6e65 eptions..PyConne
-  0x00010730 6374696f 6e457272 6f722475 32302461 ctionError$u20$a
-  0x00010740 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00010750 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00010760 31376835 30623138 36383164 66363965 17h50b18681df69e
-  0x00010770 30326345 00616e6f 6e2e6539 65623233 02cE.anon.e9eb23
-  0x00010780 37636635 30613433 62363564 36333662 7cf50a43b65d636b
-  0x00010790 30663437 37306230 34652e31 322e6c6c 0f4770b04e.12.ll
-  0x000107a0 766d2e31 33383631 38353237 31313339 vm.1386185271139
-  0x000107b0 30323734 3736005f 5a4e3837 5f244c54 027476._ZN87_$LT
-  0x000107c0 24636f72 652e2e73 74722e2e 6c6f7373 $core..str..loss
-  0x000107d0 792e2e55 74663843 68756e6b 73247532 y..Utf8Chunks$u2
-  0x000107e0 30246173 24753230 24636f72 652e2e69 0$as$u20$core..i
-  0x000107f0 7465722e 2e747261 6974732e 2e697465 ter..traits..ite
-  0x00010800 7261746f 722e2e49 74657261 746f7224 rator..Iterator$
-  0x00010810 47542434 6e657874 31376838 38393531 GT$4next17h88951
-  0x00010820 63636435 66663064 38386245 005f5a4e ccd5ff0d88bE._ZN
-  0x00010830 37375f24 4c542470 796f332e 2e657863 77_$LT$pyo3..exc
-  0x00010840 65707469 6f6e732e 2e507946 6c6f6174 eptions..PyFloat
-  0x00010850 696e6750 6f696e74 4572726f 72247532 ingPointError$u2
-  0x00010860 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x00010870 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x00010880 666d7431 37683332 63383238 64643932 fmt17h32c828dd92
-  0x00010890 31323061 62334500 5f5a4e36 345f244c 120ab3E._ZN64_$L
-  0x000108a0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x000108b0 6e732e2e 50794f53 4572726f 72247532 ns..PyOSError$u2
-  0x000108c0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x000108d0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
-  0x000108e0 74313768 64376535 34663137 62343031 t17hd7e54f17b401
-  0x000108f0 31353937 45005f5f 72757374 5f616c6c 1597E.__rust_all
-  0x00010900 6f635f7a 65726f65 64005f5a 4e34636f oc_zeroed._ZN4co
-  0x00010910 72653370 74723735 64726f70 5f696e5f re3ptr75drop_in_
-  0x00010920 706c6163 65244c54 24636f72 652e2e72 place$LT$core..r
-  0x00010930 6573756c 742e2e52 6573756c 74244c54 esult..Result$LT
-  0x00010940 24245246 24737472 24432470 796f332e $$RF$str$C$pyo3.
-  0x00010950 2e657272 2e2e5079 45727224 47542424 .err..PyErr$GT$$
-  0x00010960 47542431 37683833 39623037 64323863 GT$17h839b07d28c
-  0x00010970 35306464 3135452e 6c6c766d 2e313332 50dd15E.llvm.132
-  0x00010980 33383839 33343332 32303036 39323232 3889343220069222
-  0x00010990 36005f5a 4e37335f 244c5424 70796f33 6._ZN73_$LT$pyo3
-  0x000109a0 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
-  0x000109b0 41737365 7274696f 6e457272 6f722475 AssertionError$u
-  0x000109c0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x000109d0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x000109e0 33666d74 31376865 30356166 36643164 3fmt17he05af6d1d
-  0x000109f0 36643636 32303545 005f5a4e 34636f72 6d66205E._ZN4cor
-  0x00010a00 6533666d 7439466f 726d6174 74657231 e3fmt9Formatter1
-  0x00010a10 32646562 75675f73 74727563 74313768 2debug_struct17h
-  0x00010a20 66386464 36363839 35346665 65343332 f8dd668954fee432
-  0x00010a30 4500616e 6f6e2e65 39313336 64346363 E.anon.e9136d4cc
-  0x00010a40 32663262 66373333 64353932 62356466 2f2bf733d592b5df
-  0x00010a50 38383935 3230372e 352e6c6c 766d2e31 8895207.5.llvm.1
-  0x00010a60 37333638 37353432 34303436 38303333 7368754240468033
-  0x00010a70 35363000 616e6f6e 2e363832 66303533 560.anon.682f053
-  0x00010a80 62613364 36643134 61663562 32376366 ba3d6d14af5b27cf
-  0x00010a90 63626264 31363336 332e312e 6c6c766d cbbd16363.1.llvm
-  0x00010aa0 2e353639 37393239 37363931 33333035 .569792976913305
-  0x00010ab0 37343736 005f5a4e 35305f24 4c542424 7476._ZN50_$LT$$
-  0x00010ac0 5246246d 75742475 32302457 24753230 RF$mut$u20$W$u20
-  0x00010ad0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x00010ae0 742e2e57 72697465 24475424 31307772 t..Write$GT$10wr
-  0x00010af0 6974655f 63686172 31376839 37323363 ite_char17h9723c
-  0x00010b00 64353736 35633435 32386445 2e6c6c76 d5765c4528dE.llv
-  0x00010b10 6d2e3330 34313339 33393538 35363939 m.30413939585699
-  0x00010b20 37343334 39005f5a 4e36395f 244c5424 74349._ZN69_$LT$
-  0x00010b30 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x00010b40 2e2e5079 496e6465 78457272 6f722475 ..PyIndexError$u
-  0x00010b50 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00010b60 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x00010b70 33666d74 31376836 63663961 62353439 3fmt17h6cf9ab549
-  0x00010b80 38656131 35303945 005f5a4e 37355f24 8ea1509E._ZN75_$
-  0x00010b90 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x00010ba0 6f6e732e 2e507945 6e766972 6f6e6d65 ons..PyEnvironme
-  0x00010bb0 6e744572 726f7224 75323024 61732475 ntError$u20$as$u
-  0x00010bc0 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
-  0x00010bd0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
-  0x00010be0 63643462 36396231 65653635 66333566 cd4b69b1ee65f35f
-  0x00010bf0 4500616e 6f6e2e62 39613034 38366330 E.anon.b9a0486c0
-  0x00010c00 30613431 37326237 62316163 35326233 0a4172b7b1ac52b3
-  0x00010c10 31356161 3461332e 33322e6c 6c766d2e 15aa4a3.32.llvm.
-  0x00010c20 31333233 38383933 34333232 30303639 1323889343220069
-  0x00010c30 32323236 00616e6f 6e2e3762 39343661 2226.anon.7b946a
-  0x00010c40 65316433 61363636 37393765 32646231 e1d3a666797e2db1
-  0x00010c50 66333665 34636436 65372e33 332e6c6c f36e4cd6e7.33.ll
-  0x00010c60 766d2e31 38333536 37353034 38353631 vm.1835675048561
-  0x00010c70 34353133 31323900 5f5a4e31 31706172 4513129._ZN11par
-  0x00010c80 6b696e67 5f6c6f74 39726177 5f6d7574 king_lot9raw_mut
-  0x00010c90 65783852 61774d75 74657839 6c6f636b ex8RawMutex9lock
-  0x00010ca0 5f736c6f 77313768 30383338 65626338 _slow17h0838ebc8
-  0x00010cb0 32326561 30326666 45005f5a 4e36395f 22ea02ffE._ZN69_
-  0x00010cc0 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00010cd0 696f6e73 2e2e5079 53797374 656d4578 ions..PySystemEx
-  0x00010ce0 69742475 32302461 73247532 3024636f it$u20$as$u20$co
-  0x00010cf0 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x00010d00 24475424 33666d74 31376864 66306362 $GT$3fmt17hdf0cb
-  0x00010d10 31633036 62313464 39303545 005f5a4e 1c06b14d905E._ZN
-  0x00010d20 34636f72 65336f70 73386675 6e637469 4core3ops8functi
-  0x00010d30 6f6e3646 6e4f6e63 65343063 616c6c5f on6FnOnce40call_
-  0x00010d40 6f6e6365 24753762 24247537 62247674 once$u7b$$u7b$vt
-  0x00010d50 61626c65 2e736869 6d247537 64242475 able.shim$u7d$$u
-  0x00010d60 37642431 37686364 65306230 30333565 7d$17hcde0b0035e
-  0x00010d70 36633862 6565452e 6c6c766d 2e313332 6c8beeE.llvm.132
-  0x00010d80 33383839 33343332 32303036 39323232 3889343220069222
-  0x00010d90 36005f5a 4e34636f 72653970 616e6963 6._ZN4core9panic
-  0x00010da0 6b696e67 31336173 73657274 5f666169 king13assert_fai
-  0x00010db0 6c656431 37686639 61373437 34666634 led17hf9a7474ff4
-  0x00010dc0 31663338 33654500 5f5a4e37 315f244c 1f383eE._ZN71_$L
-  0x00010dd0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x00010de0 6e732e2e 5079556e 69636f64 65576172 ns..PyUnicodeWar
-  0x00010df0 6e696e67 24753230 24617324 75323024 ning$u20$as$u20$
-  0x00010e00 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00010e10 24475424 33666d74 31376838 31393065 $GT$3fmt17h8190e
-  0x00010e20 36363061 37386231 61303245 005f5a4e 660a78b1a02E._ZN
-  0x00010e30 39616464 72326c69 6e653970 6174685f 9addr2line9path_
-  0x00010e40 70757368 31376832 62646362 38353864 push17h2bdcb858d
-  0x00010e50 30663164 65643945 005f5a4e 34636f72 0f1ded9E._ZN4cor
-  0x00010e60 6533666d 7439466f 726d6174 74657231 e3fmt9Formatter1
-  0x00010e70 30646562 75675f6c 69737431 37683966 0debug_list17h9f
-  0x00010e80 32663238 61393733 32666633 37384500 2f28a9732ff378E.
-  0x00010e90 5f5a4e34 636f7265 33666d74 39466f72 _ZN4core3fmt9For
-  0x00010ea0 6d617474 65723235 64656275 675f7475 matter25debug_tu
-  0x00010eb0 706c655f 6669656c 64325f66 696e6973 ple_field2_finis
-  0x00010ec0 68313768 35396338 61353364 62646563 h17h59c8a53dbdec
-  0x00010ed0 32633237 4500616e 6f6e2e36 38326630 2c27E.anon.682f0
-  0x00010ee0 35336261 33643664 31346166 35623237 53ba3d6d14af5b27
-  0x00010ef0 63666362 62643136 3336332e 34302e6c cfcbbd16363.40.l
-  0x00010f00 6c766d2e 35363937 39323937 36393133 lvm.569792976913
-  0x00010f10 33303537 34373600 5f5a4e34 636f7265 3057476._ZN4core
-  0x00010f20 33707472 33376472 6f705f69 6e5f706c 3ptr37drop_in_pl
-  0x00010f30 61636524 4c542463 6f72652e 2e666d74 ace$LT$core..fmt
-  0x00010f40 2e2e4572 726f7224 47542431 37686532 ..Error$GT$17he2
-  0x00010f50 30636333 61363863 36316262 3139452e 0cc3a68c61bb19E.
-  0x00010f60 6c6c766d 2e353639 37393239 37363931 llvm.56979297691
-  0x00010f70 33333035 37343736 005f5a4e 34636f72 33057476._ZN4cor
-  0x00010f80 65337074 72313038 64726f70 5f696e5f e3ptr108drop_in_
-  0x00010f90 706c6163 65244c54 2470796f 332e2e65 place$LT$pyo3..e
-  0x00010fa0 72722e2e 6572725f 73746174 652e2e62 rr..err_state..b
-  0x00010fb0 6f786564 5f617267 73244c54 24244c50 oxed_args$LT$$LP
-  0x00010fc0 24245246 24737472 24432424 52502424 $$RF$str$C$$RP$$
-  0x00010fd0 4754242e 2e247537 62242475 37622463 GT$..$u7b$$u7b$c
-  0x00010fe0 6c6f7375 72652475 37642424 75376424 losure$u7d$$u7d$
-  0x00010ff0 24475424 31376861 61353932 66613566 $GT$17haa592fa5f
-  0x00011000 36363937 38306445 2e6c6c76 6d2e3331 669780dE.llvm.31
-  0x00011010 36303930 37323831 38383037 38313132 6090728188078112
-  0x00011020 33005f5a 4e37325f 244c5424 70796f33 3._ZN72_$LT$pyo3
-  0x00011030 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
-  0x00011040 53796e74 61785761 726e696e 67247532 SyntaxWarning$u2
-  0x00011050 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x00011060 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x00011070 666d7431 37683338 31616465 36313131 fmt17h381ade6111
-  0x00011080 61366139 39364500 5f5a4e37 315f244c a6a996E._ZN71_$L
-  0x00011090 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x000110a0 6e732e2e 50794174 74726962 75746545 ns..PyAttributeE
-  0x000110b0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x000110c0 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x000110d0 24475424 33666d74 31376836 35636366 $GT$3fmt17h65ccf
-  0x000110e0 61346364 37633966 61626345 005f5a4e a4cd7c9fabcE._ZN
-  0x000110f0 36345f24 4c542473 74642e2e 7379732e 64_$LT$std..sys.
-  0x00011100 2e756e69 782e2e73 7464696f 2e2e5374 .unix..stdio..St
-  0x00011110 64657272 24753230 24617324 75323024 derr$u20$as$u20$
-  0x00011120 7374642e 2e696f2e 2e577269 74652447 std..io..Write$G
-  0x00011130 54243134 77726974 655f7665 63746f72 T$14write_vector
-  0x00011140 65643137 68323739 31353734 63303035 ed17h2791574c005
-  0x00011150 36363166 6645005f 5a4e3638 5f244c54 661ffE._ZN68_$LT
-  0x00011160 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00011170 732e2e50 794c6f6f 6b757045 72726f72 s..PyLookupError
-  0x00011180 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00011190 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x000111a0 33666d74 31376838 31633337 62663362 3fmt17h81c37bf3b
-  0x000111b0 36643731 30353145 005f5a4e 33737464 6d71051E._ZN3std
-  0x000111c0 34706174 68345061 74683769 735f6669 4path4Path7is_fi
-  0x000111d0 6c653137 68613066 30323762 36663237 le17ha0f027b6f27
-  0x000111e0 37363638 6545005f 5a4e3631 5f244c54 7668eE._ZN61_$LT
-  0x000111f0 24245246 24737464 2e2e696f 2e2e7374 $$RF$std..io..st
-  0x00011200 64696f2e 2e537464 65727224 75323024 dio..Stderr$u20$
-  0x00011210 61732475 32302473 74642e2e 696f2e2e as$u20$std..io..
-  0x00011220 57726974 65244754 24397772 6974655f Write$GT$9write_
-  0x00011230 666d7431 37683533 66313762 36346131 fmt17h53f17b64a1
-  0x00011240 32666139 64624500 5f5a4e33 73746439 2fa9dbE._ZN3std9
-  0x00011250 70616e69 636b696e 67323072 7573745f panicking20rust_
-  0x00011260 70616e69 635f7769 74685f68 6f6f6b31 panic_with_hook1
-  0x00011270 37683530 63303964 30303064 63353631 7h50c09d000dc561
-  0x00011280 64324500 5f5a4e34 636f7265 33666d74 d2E._ZN4core3fmt
-  0x00011290 336e756d 33696d70 35325f24 4c542469 3num3imp52_$LT$i
-  0x000112a0 6d706c24 75323024 636f7265 2e2e666d mpl$u20$core..fm
-  0x000112b0 742e2e44 6973706c 61792475 32302466 t..Display$u20$f
-  0x000112c0 6f722475 32302475 36342447 54243366 or$u20$u64$GT$3f
-  0x000112d0 6d743137 68616237 33386265 37336337 mt17hab738be73c7
-  0x000112e0 62376338 3645005f 5a4e3463 6f726533 b7c86E._ZN4core3
-  0x000112f0 666d7431 30417267 756d656e 74563131 fmt10ArgumentV11
-  0x00011300 3066726f 6d5f7573 697a6531 37686165 0from_usize17hae
-  0x00011310 61653833 65363833 30313631 61314500 ae83e6830161a1E.
-  0x00011320 5f5a4e34 636f7265 33707472 32303564 _ZN4core3ptr205d
-  0x00011330 726f705f 696e5f70 6c616365 244c5424 rop_in_place$LT$
-  0x00011340 244c5424 616c6c6f 632e2e62 6f786564 $LT$alloc..boxed
-  0x00011350 2e2e426f 78244c54 2464796e 24753230 ..Box$LT$dyn$u20
-  0x00011360 24636f72 652e2e65 72726f72 2e2e4572 $core..error..Er
-  0x00011370 726f7224 75326224 636f7265 2e2e6d61 ror$u2b$core..ma
-  0x00011380 726b6572 2e2e5365 6e642475 32622463 rker..Send$u2b$c
-  0x00011390 6f72652e 2e6d6172 6b65722e 2e53796e ore..marker..Syn
-  0x000113a0 63244754 24247532 30246173 24753230 c$GT$$u20$as$u20
-  0x000113b0 24636f72 652e2e63 6f6e7665 72742e2e $core..convert..
-  0x000113c0 46726f6d 244c5424 616c6c6f 632e2e73 From$LT$alloc..s
-  0x000113d0 7472696e 672e2e53 7472696e 67244754 tring..String$GT
-  0x000113e0 24244754 242e2e66 726f6d2e 2e537472 $$GT$..from..Str
-  0x000113f0 696e6745 72726f72 24475424 31376834 ingError$GT$17h4
-  0x00011400 34663361 38313438 33353164 31333845 4f3a8148351d138E
-  0x00011410 2e6c6c76 6d2e3330 34313339 33393538 .llvm.3041393958
-  0x00011420 35363939 37343334 39005f5a 4e37355f 569974349._ZN75_
-  0x00011430 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00011440 696f6e73 2e2e5079 556e6963 6f646545 ions..PyUnicodeE
-  0x00011450 6e636f64 65457272 6f722475 32302461 ncodeError$u20$a
-  0x00011460 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00011470 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x00011480 68613133 30646639 38356235 62346364 ha130df985b5b4cd
-  0x00011490 6645005f 5a4e3732 5f244c54 2470796f fE._ZN72_$LT$pyo
-  0x000114a0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x000114b0 79526573 6f757263 65576172 6e696e67 yResourceWarning
-  0x000114c0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x000114d0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x000114e0 33666d74 31376866 34326633 32313932 3fmt17hf42f32192
-  0x000114f0 62366264 34623945 005f5a4e 35616c6c b6bd4b9E._ZN5all
-  0x00011500 6f633772 61775f76 65633139 52617756 oc7raw_vec19RawV
-  0x00011510 6563244c 54245424 43244124 47542431 ec$LT$T$C$A$GT$1
-  0x00011520 36726573 65727665 5f666f72 5f707573 6reserve_for_pus
-  0x00011530 68313768 39363834 33613830 65373135 h17h96843a80e715
-  0x00011540 30636539 45005f5a 4e35616c 6c6f6337 0ce9E._ZN5alloc7
-  0x00011550 7261775f 76656331 39526177 56656324 raw_vec19RawVec$
-  0x00011560 4c542454 24432441 24475424 31367265 LT$T$C$A$GT$16re
-  0x00011570 73657276 655f666f 725f7075 73683137 serve_for_push17
-  0x00011580 68386339 62316631 34656237 39386130 h8c9b1f14eb798a0
-  0x00011590 6145005f 5a4e3735 5f244c54 2470796f aE._ZN75_$LT$pyo
-  0x000115a0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x000115b0 79556e69 636f6465 4465636f 64654572 yUnicodeDecodeEr
-  0x000115c0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x000115d0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x000115e0 47542433 666d7431 37686434 32623864 GT$3fmt17hd42b8d
-  0x000115f0 32326538 64393137 30364500 5f5a4e34 22e8d91706E._ZN4
-  0x00011600 636f7265 33666d74 39466f72 6d617474 core3fmt9Formatt
-  0x00011610 65723977 72697465 5f666d74 31376861 er9write_fmt17ha
-  0x00011620 34613838 34646232 35346136 31663945 4a884db254a61f9E
-  0x00011630 00616e6f 6e2e6539 65623233 37636635 .anon.e9eb237cf5
-  0x00011640 30613433 62363564 36333662 30663437 0a43b65d636b0f47
-  0x00011650 37306230 34652e33 332e6c6c 766d2e31 70b04e.33.llvm.1
-  0x00011660 33383631 38353237 31313339 30323734 3861852711390274
-  0x00011670 3736005f 5a4e3463 6f726533 6e756d36 76._ZN4core3num6
-  0x00011680 305f244c 5424696d 706c2475 32302463 0_$LT$impl$u20$c
-  0x00011690 6f72652e 2e737472 2e2e7472 61697473 ore..str..traits
-  0x000116a0 2e2e4672 6f6d5374 72247532 3024666f ..FromStr$u20$fo
-  0x000116b0 72247532 30247536 34244754 24386672 r$u20$u64$GT$8fr
-  0x000116c0 6f6d5f73 74723137 68376161 61373164 om_str17h7aaa71d
-  0x000116d0 36313765 65373038 3945005f 5a4e3463 617ee7089E._ZN4c
-  0x000116e0 6f726533 70747231 32366472 6f705f69 ore3ptr126drop_i
-  0x000116f0 6e5f706c 61636524 4c542470 796f332e n_place$LT$pyo3.
-  0x00011700 2e657272 2e2e6572 725f7374 6174652e .err..err_state.
-  0x00011710 2e626f78 65645f61 72677324 4c542463 .boxed_args$LT$c
-  0x00011720 6f72652e 2e636861 722e2e64 65636f64 ore..char..decod
-  0x00011730 652e2e44 65636f64 65557466 31364572 e..DecodeUtf16Er
-  0x00011740 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
-  0x00011750 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x00011760 75376424 24475424 31376834 62316437 u7d$$GT$17h4b1d7
-  0x00011770 31373539 30636233 66326645 2e6c6c76 17590cb3f2fE.llv
-  0x00011780 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x00011790 38313132 33005f5a 4e34636f 72653366 81123._ZN4core3f
-  0x000117a0 6d74336e 756d3532 5f244c54 24696d70 mt3num52_$LT$imp
-  0x000117b0 6c247532 3024636f 72652e2e 666d742e l$u20$core..fmt.
-  0x000117c0 2e557070 65724865 78247532 3024666f .UpperHex$u20$fo
-  0x000117d0 72247532 30247538 24475424 33666d74 r$u20$u8$GT$3fmt
-  0x000117e0 31376838 62626161 66653333 38346332 17h8bbaafe3384c2
-  0x000117f0 61613745 005f5a4e 34636f72 65337074 aa7E._ZN4core3pt
-  0x00011800 72333764 726f705f 696e5f70 6c616365 r37drop_in_place
-  0x00011810 244c5424 636f7265 2e2e666d 742e2e45 $LT$core..fmt..E
-  0x00011820 72726f72 24475424 31376865 32306363 rror$GT$17he20cc
-  0x00011830 33613638 63363162 62313945 2e6c6c76 3a68c61bb19E.llv
-  0x00011840 6d2e3330 34313339 33393538 35363939 m.30413939585699
-  0x00011850 37343334 3900616e 6f6e2e62 39613034 74349.anon.b9a04
-  0x00011860 38366330 30613431 37326237 62316163 86c00a4172b7b1ac
-  0x00011870 35326233 31356161 3461332e 31342e6c 52b315aa4a3.14.l
-  0x00011880 6c766d2e 31333233 38383933 34333232 lvm.132388934322
-  0x00011890 30303639 32323236 005f5a4e 3470796f 00692226._ZN4pyo
-  0x000118a0 3335696d 706c5f38 70796d6f 64756c65 35impl_8pymodule
-  0x000118b0 394d6f64 756c6544 65663131 6d616b65 9ModuleDef11make
-  0x000118c0 5f6d6f64 756c6531 37683739 66323466 _module17h79f24f
-  0x000118d0 64373561 36653263 37634500 5f5a4e36 d75a6e2c7cE._ZN6
-  0x000118e0 345f244c 54247079 6f332e2e 65786365 4_$LT$pyo3..exce
-  0x000118f0 7074696f 6e732e2e 5079494f 4572726f ptions..PyIOErro
-  0x00011900 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x00011910 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x00011920 2433666d 74313768 61393939 62653136 $3fmt17ha999be16
-  0x00011930 39653039 39353735 45005f5a 4e34636f 9e099575E._ZN4co
-  0x00011940 72653366 6d743946 6f726d61 74746572 re3fmt9Formatter
-  0x00011950 39777269 74655f73 74723137 68383136 9write_str17h816
-  0x00011960 38366138 33336636 38666335 3345005f 86a833f68fc53E._
-  0x00011970 5a4e3737 5f244c54 2470796f 332e2e65 ZN77_$LT$pyo3..e
-  0x00011980 78636570 74696f6e 732e2e50 7950726f xceptions..PyPro
-  0x00011990 63657373 4c6f6f6b 75704572 726f7224 cessLookupError$
-  0x000119a0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x000119b0 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
-  0x000119c0 2433666d 74313768 39663662 38316666 $3fmt17h9f6b81ff
-  0x000119d0 33383864 34346637 4500616e 6f6e2e36 388d44f7E.anon.6
-  0x000119e0 38326630 35336261 33643664 31346166 82f053ba3d6d14af
-  0x000119f0 35623237 63666362 62643136 3336332e 5b27cfcbbd16363.
-  0x00011a00 302e6c6c 766d2e35 36393739 32393736 0.llvm.569792976
-  0x00011a10 39313333 30353734 3736005f 5a4e3470 9133057476._ZN4p
-  0x00011a20 796f3335 74797065 73357475 706c6531 yo35types5tuple1
-  0x00011a30 32355f24 4c542469 6d706c24 75323024 25_$LT$impl$u20$
-  0x00011a40 70796f33 2e2e636f 6e766572 73696f6e pyo3..conversion
-  0x00011a50 2e2e496e 746f5079 244c5424 70796f33 ..IntoPy$LT$pyo3
-  0x00011a60 2e2e696e 7374616e 63652e2e 5079244c ..instance..Py$L
-  0x00011a70 54247079 6f332e2e 74797065 732e2e61 T$pyo3..types..a
-  0x00011a80 6e792e2e 5079416e 79244754 24244754 ny..PyAny$GT$$GT
-  0x00011a90 24247532 3024666f 72247532 3024244c $$u20$for$u20$$L
-  0x00011aa0 50245430 24432424 52502424 47542437 P$T0$C$$RP$$GT$7
-  0x00011ab0 696e746f 5f707931 37686436 65643665 into_py17hd6ed6e
-  0x00011ac0 63303331 36663838 31344500 5f5a4e35 c0316f8814E._ZN5
-  0x00011ad0 616c6c6f 63377261 775f7665 63313952 alloc7raw_vec19R
-  0x00011ae0 61775665 63244c54 24542443 24412447 awVec$LT$T$C$A$G
-  0x00011af0 54243136 72657365 7276655f 666f725f T$16reserve_for_
-  0x00011b00 70757368 31376835 66636230 64323066 push17h5fcb0d20f
-  0x00011b10 62333166 34373845 005f5a4e 33737464 b31f478E._ZN3std
-  0x00011b20 3970616e 69636b69 6e673131 70616e69 9panicking11pani
-  0x00011b30 635f636f 756e7431 38474c4f 42414c5f c_count18GLOBAL_
-  0x00011b40 50414e49 435f434f 554e5431 37683439 PANIC_COUNT17h49
-  0x00011b50 31643832 30656438 33313865 63354500 1d820ed8318ec5E.
-  0x00011b60 5f5a4e36 365f244c 54247079 6f332e2e _ZN66_$LT$pyo3..
-  0x00011b70 65786365 7074696f 6e732e2e 50794e61 exceptions..PyNa
-  0x00011b80 6d654572 726f7224 75323024 61732475 meError$u20$as$u
-  0x00011b90 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x00011ba0 62756724 47542433 666d7431 37686664 bug$GT$3fmt17hfd
-  0x00011bb0 61316566 31313737 34373962 36314500 a1ef1177479b61E.
-  0x00011bc0 5f5a4e34 636f7265 33666d74 336e756d _ZN4core3fmt3num
-  0x00011bd0 35355f24 4c542469 6d706c24 75323024 55_$LT$impl$u20$
-  0x00011be0 636f7265 2e2e666d 742e2e4c 6f776572 core..fmt..Lower
-  0x00011bf0 48657824 75323024 666f7224 75323024 Hex$u20$for$u20$
-  0x00011c00 7573697a 65244754 2433666d 74313768 usize$GT$3fmt17h
-  0x00011c10 62373334 32646431 37353064 63383837 b7342dd1750dc887
-  0x00011c20 45005f5a 4e347079 6f333574 79706573 E._ZN4pyo35types
-  0x00011c30 35747570 6c653750 79547570 6c65336c 5tuple7PyTuple3l
-  0x00011c40 656e3137 68636537 37616434 63346438 en17hce77ad4c4d8
-  0x00011c50 65633437 63450061 6e6f6e2e 36383266 ec47cE.anon.682f
-  0x00011c60 30353362 61336436 64313461 66356232 053ba3d6d14af5b2
-  0x00011c70 37636663 62626431 36333633 2e332e6c 7cfcbbd16363.3.l
-  0x00011c80 6c766d2e 35363937 39323937 36393133 lvm.569792976913
-  0x00011c90 33303537 34373600 5f5a4e34 636f7265 3057476._ZN4core
-  0x00011ca0 33707472 35306472 6f705f69 6e5f706c 3ptr50drop_in_pl
-  0x00011cb0 61636524 4c542461 6c6c6f63 2e2e626f ace$LT$alloc..bo
-  0x00011cc0 72726f77 2e2e436f 77244c54 24737472 rrow..Cow$LT$str
-  0x00011cd0 24475424 24475424 31376862 32316338 $GT$$GT$17hb21c8
-  0x00011ce0 31353465 35386630 66633645 2e6c6c76 154e58f0fc6E.llv
-  0x00011cf0 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x00011d00 38313132 33005f5a 4e337374 6432696f 81123._ZN3std2io
-  0x00011d10 35657272 6f723833 5f244c54 24696d70 5error83_$LT$imp
-  0x00011d20 6c247532 3024636f 72652e2e 666d742e l$u20$core..fmt.
-  0x00011d30 2e446562 75672475 32302466 6f722475 .Debug$u20$for$u
-  0x00011d40 32302473 74642e2e 696f2e2e 6572726f 20$std..io..erro
-  0x00011d50 722e2e72 6570725f 62697470 61636b65 r..repr_bitpacke
-  0x00011d60 642e2e52 65707224 47542433 666d7431 d..Repr$GT$3fmt1
-  0x00011d70 37686465 62323866 30306234 36383538 7hdeb28f00b46858
-  0x00011d80 66394500 5f5f7275 73745f66 6f726569 f9E.__rust_forei
-  0x00011d90 676e5f65 78636570 74696f6e 005f5a4e gn_exception._ZN
-  0x00011da0 31367061 726b696e 675f6c6f 745f636f 16parking_lot_co
-  0x00011db0 72653131 7061726b 696e675f 6c6f7431 re11parking_lot1
-  0x00011dc0 36637265 6174655f 68617368 7461626c 6create_hashtabl
-  0x00011dd0 65313768 32633161 61373966 33353030 e17h2c1aa79f3500
-  0x00011de0 38343261 45005f5a 4e37365f 244c5424 842aE._ZN76_$LT$
-  0x00011df0 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x00011e00 2e2e5079 4368696c 6450726f 63657373 ..PyChildProcess
-  0x00011e10 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x00011e20 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
-  0x00011e30 6c617924 47542433 666d7431 37683337 lay$GT$3fmt17h37
-  0x00011e40 64363931 38646163 62323765 66354500 d6918dacb27ef5E.
-  0x00011e50 5f5a4e33 73746431 30737973 5f636f6d _ZN3std10sys_com
-  0x00011e60 6d6f6e39 6261636b 74726163 6532365f mon9backtrace26_
-  0x00011e70 5f727573 745f656e 645f7368 6f72745f _rust_end_short_
-  0x00011e80 6261636b 74726163 65313768 39393133 backtrace17h9913
-  0x00011e90 66386430 38623932 35613365 45005f5a f8d08b925a3eE._Z
-  0x00011ea0 4e36375f 244c5424 70796f33 2e2e6578 N67_$LT$pyo3..ex
-  0x00011eb0 63657074 696f6e73 2e2e5079 4b657945 ceptions..PyKeyE
-  0x00011ec0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x00011ed0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x00011ee0 61792447 54243366 6d743137 68323030 ay$GT$3fmt17h200
-  0x00011ef0 31393931 62626661 39323233 3345005f 1991bbfa92233E._
-  0x00011f00 5a4e3736 5f244c54 2470796f 332e2e65 ZN76_$LT$pyo3..e
-  0x00011f10 78636570 74696f6e 732e2e50 794b6579 xceptions..PyKey
-  0x00011f20 626f6172 64496e74 65727275 70742475 boardInterrupt$u
-  0x00011f30 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00011f40 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x00011f50 33666d74 31376866 31636333 35376536 3fmt17hf1cc357e6
-  0x00011f60 37623635 62386345 00616e6f 6e2e6138 7b65b8cE.anon.a8
-  0x00011f70 30393032 64366262 30383737 33626636 0902d6bb08773bf6
-  0x00011f80 37343364 30323363 37646637 33652e31 743d023c7df73e.1
-  0x00011f90 332e6c6c 766d2e31 31393430 36323133 3.llvm.119406213
-  0x00011fa0 36373536 30363632 38303500 5f5a4e35 67560662805._ZN5
-  0x00011fb0 305f244c 54242452 46246d75 74247532 0_$LT$$RF$mut$u2
-  0x00011fc0 30245724 75323024 61732475 32302463 0$W$u20$as$u20$c
-  0x00011fd0 6f72652e 2e666d74 2e2e5772 69746524 ore..fmt..Write$
-  0x00011fe0 47542439 77726974 655f666d 74313768 GT$9write_fmt17h
-  0x00011ff0 35343664 37613034 33666238 35653033 546d7a043fb85e03
-  0x00012000 452e6c6c 766d2e33 30343133 39333935 E.llvm.304139395
-  0x00012010 38353639 39373433 3439005f 5a4e3737 8569974349._ZN77
-  0x00012020 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
-  0x00012030 74696f6e 732e2e50 79436f6e 6e656374 tions..PyConnect
-  0x00012040 696f6e52 65736574 4572726f 72247532 ionResetError$u2
-  0x00012050 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x00012060 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
-  0x00012070 74313768 38343164 62646331 33623032 t17h841dbdc13b02
-  0x00012080 38303733 45005f5a 4e37335f 244c5424 8073E._ZN73_$LT$
-  0x00012090 636f7265 2e2e7061 6e69632e 2e70616e core..panic..pan
-  0x000120a0 69635f69 6e666f2e 2e50616e 6963496e ic_info..PanicIn
-  0x000120b0 666f2475 32302461 73247532 3024636f fo$u20$as$u20$co
-  0x000120c0 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x000120d0 24475424 33666d74 31376838 65313132 $GT$3fmt17h8e112
-  0x000120e0 38623833 39313439 35343545 005f5a4e 8b839149545E._ZN
-  0x000120f0 34325f24 4c542473 74722475 32302461 42_$LT$str$u20$a
-  0x00012100 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00012110 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00012120 31376863 62303461 63633532 34346433 17hcb04acc5244d3
-  0x00012130 35653345 005f5a4e 3470796f 33357479 5e3E._ZN4pyo35ty
-  0x00012140 70657331 30747970 656f626a 65637436 pes10typeobject6
-  0x00012150 50795479 7065346e 616d6538 494e5445 PyType4name8INTE
-  0x00012160 524e4544 31376864 65333233 30623965 RNED17hde3230b9e
-  0x00012170 35666533 33376345 2e6c6c76 6d2e3134 5fe337cE.llvm.14
-  0x00012180 36333134 33313432 33313037 36383738 6314314231076878
-  0x00012190 32330061 6e6f6e2e 37623934 36616531 23.anon.7b946ae1
-  0x000121a0 64336136 36363739 37653264 62316633 d3a666797e2db1f3
-  0x000121b0 36653463 64366537 2e32302e 6c6c766d 6e4cd6e7.20.llvm
-  0x000121c0 2e313833 35363735 30343835 36313435 .183567504856145
-  0x000121d0 31333132 39005f5a 4e356769 6d6c6934 13129._ZN5gimli4
-  0x000121e0 72656164 36616262 72657631 33416262 read6abbrev13Abb
-  0x000121f0 72657669 6174696f 6e733565 6d707479 reviations5empty
-  0x00012200 31376838 33353132 34323264 33633430 17h83512422d3c40
-  0x00012210 34333445 005f5a4e 37335f24 4c542470 434E._ZN73_$LT$p
-  0x00012220 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x00012230 2e507952 65666572 656e6365 4572726f .PyReferenceErro
-  0x00012240 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x00012250 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
-  0x00012260 47542433 666d7431 37683662 33626437 GT$3fmt17h6b3bd7
-  0x00012270 64356636 63613738 31304500 5f5a4e34 d5f6ca7810E._ZN4
-  0x00012280 636f7265 33737472 38636f6e 76657274 core3str8convert
-  0x00012290 73396672 6f6d5f75 74663831 37683936 s9from_utf817h96
-  0x000122a0 66653034 66346336 64336631 65614500 fe04f4c6d3f1eaE.
-  0x000122b0 5f5a4e35 305f244c 54242452 46246d75 _ZN50_$LT$$RF$mu
-  0x000122c0 74247532 30245724 75323024 61732475 t$u20$W$u20$as$u
-  0x000122d0 32302463 6f72652e 2e666d74 2e2e5772 20$core..fmt..Wr
-  0x000122e0 69746524 47542439 77726974 655f7374 ite$GT$9write_st
-  0x000122f0 72313768 63313764 37653936 32356237 r17hc17d7e9625b7
-  0x00012300 64666661 452e6c6c 766d2e33 30343133 dffaE.llvm.30413
-  0x00012310 39333935 38353639 39373433 3439005f 93958569974349._
-  0x00012320 5a4e3463 6f726533 666d7433 6e756d35 ZN4core3fmt3num5
-  0x00012330 325f244c 5424696d 706c2475 32302463 2_$LT$impl$u20$c
-  0x00012340 6f72652e 2e666d74 2e2e5570 70657248 ore..fmt..UpperH
-  0x00012350 65782475 32302466 6f722475 32302469 ex$u20$for$u20$i
-  0x00012360 38244754 2433666d 74313768 39353130 8$GT$3fmt17h9510
-  0x00012370 34393264 61356137 66356636 45005f5a 492da5a7f5f6E._Z
-  0x00012380 4e37355f 244c5424 70796f33 2e2e6578 N75_$LT$pyo3..ex
-  0x00012390 63657074 696f6e73 2e2e5079 4e6f7441 ceptions..PyNotA
-  0x000123a0 44697265 63746f72 79457272 6f722475 DirectoryError$u
-  0x000123b0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x000123c0 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
-  0x000123d0 6d743137 68313133 32306234 30623230 mt17h11320b40b20
-  0x000123e0 32323731 6145005f 5a4e3735 5f244c54 2271aE._ZN75_$LT
-  0x000123f0 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00012400 732e2e50 7950726f 63657373 4c6f6f6b s..PyProcessLook
-  0x00012410 75704572 726f7224 75323024 61732475 upError$u20$as$u
-  0x00012420 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x00012430 62756724 47542433 666d7431 37683839 bug$GT$3fmt17h89
-  0x00012440 30366134 36656637 62313433 63314500 06a46ef7b143c1E.
-  0x00012450 5f5a4e34 636f7265 33707472 34376472 _ZN4core3ptr47dr
-  0x00012460 6f705f69 6e5f706c 61636524 4c542463 op_in_place$LT$c
-  0x00012470 6f72652e 2e63656c 6c2e2e42 6f72726f ore..cell..Borro
-  0x00012480 774d7574 4572726f 72244754 24313768 wMutError$GT$17h
-  0x00012490 62646538 30656166 63623765 63303262 bde80eafcb7ec02b
-  0x000124a0 452e6c6c 766d2e31 38333536 37353034 E.llvm.183567504
-  0x000124b0 38353631 34353133 31323900 5f5a4e36 85614513129._ZN6
-  0x000124c0 365f244c 54247079 6f332e2e 65786365 6_$LT$pyo3..exce
-  0x000124d0 7074696f 6e732e2e 50795479 70654572 ptions..PyTypeEr
-  0x000124e0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x000124f0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x00012500 47542433 666d7431 37683032 35616565 GT$3fmt17h025aee
-  0x00012510 31346264 38313566 34314500 616e6f6e 14bd815f41E.anon
-  0x00012520 2e376239 34366165 31643361 36363637 .7b946ae1d3a6667
-  0x00012530 39376532 64623166 33366534 63643665 97e2db1f36e4cd6e
-  0x00012540 372e3332 2e6c6c76 6d2e3138 33353637 7.32.llvm.183567
-  0x00012550 35303438 35363134 35313331 3239005f 50485614513129._
-  0x00012560 5a4e3561 6c6c6f63 35616c6c 6f633862 ZN5alloc5alloc8b
-  0x00012570 6f785f66 72656531 37683664 36306465 ox_free17h6d60de
-  0x00012580 32653865 37303762 6464452e 6c6c766d 2e8e707bddE.llvm
-  0x00012590 2e313332 33383839 33343332 32303036 .132388934322006
-  0x000125a0 39323232 36005f5a 4e38345f 244c5424 92226._ZN84_$LT$
-  0x000125b0 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x000125c0 2e2e5079 50656e64 696e6744 65707265 ..PyPendingDepre
-  0x000125d0 63617469 6f6e5761 726e696e 67247532 cationWarning$u2
-  0x000125e0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x000125f0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x00012600 666d7431 37683433 66366465 30646662 fmt17h43f6de0dfb
-  0x00012610 66613864 35394500 5f5a4e37 355f244c fa8d59E._ZN75_$L
-  0x00012620 54246769 6d6c692e 2e726561 642e2e61 T$gimli..read..a
-  0x00012630 62627265 762e2e41 74747269 62757465 bbrev..Attribute
-  0x00012640 73247532 30246173 24753230 24636f72 s$u20$as$u20$cor
-  0x00012650 652e2e6f 70732e2e 64657265 662e2e44 e..ops..deref..D
-  0x00012660 65726566 24475424 35646572 65663137 eref$GT$5deref17
-  0x00012670 68306539 37373830 37363364 35303136 h0e97780763d5016
-  0x00012680 6245005f 5a4e3831 5f244c54 24245246 bE._ZN81_$LT$$RF
-  0x00012690 24247535 62247538 24753564 24247532 $$u5b$u8$u5d$$u2
-  0x000126a0 30246173 24753230 24616c6c 6f632e2e 0$as$u20$alloc..
-  0x000126b0 6666692e 2e635f73 74722e2e 43537472 ffi..c_str..CStr
-  0x000126c0 696e672e 2e6e6577 2e2e5370 65634e65 ing..new..SpecNe
-  0x000126d0 77496d70 6c244754 24313373 7065635f wImpl$GT$13spec_
-  0x000126e0 6e65775f 696d706c 31376863 63623131 new_impl17hccb11
-  0x000126f0 37646165 31376561 34306545 005f5a4e 7dae17ea40eE._ZN
-  0x00012700 31316d69 6e697a5f 6f786964 6537696e 11miniz_oxide7in
-  0x00012710 666c6174 6534636f 72653137 4465636f flate4core17Deco
-  0x00012720 6d707265 73736f72 4f786964 65336e65 mpressorOxide3ne
-  0x00012730 77313768 64363261 36326536 33653439 w17hd62a62e63e49
-  0x00012740 32303465 45005f5a 4e347079 6f333574 204eE._ZN4pyo35t
-  0x00012750 79706573 35747570 6c653133 375f244c ypes5tuple137_$L
-  0x00012760 5424696d 706c2475 32302470 796f332e T$impl$u20$pyo3.
-  0x00012770 2e636f6e 76657273 696f6e2e 2e496e74 .conversion..Int
-  0x00012780 6f507924 4c542470 796f332e 2e696e73 oPy$LT$pyo3..ins
-  0x00012790 74616e63 652e2e50 79244c54 2470796f tance..Py$LT$pyo
-  0x000127a0 332e2e74 79706573 2e2e616e 792e2e50 3..types..any..P
-  0x000127b0 79416e79 24475424 24475424 24753230 yAny$GT$$GT$$u20
-  0x000127c0 24666f72 24753230 24244c50 24543024 $for$u20$$LP$T0$
-  0x000127d0 43245431 24432454 32244324 54332452 C$T1$C$T2$C$T3$R
-  0x000127e0 50242447 54243769 6e746f5f 70793137 P$$GT$7into_py17
-  0x000127f0 68666265 62323837 64393533 63633839 hfbeb287d953cc89
-  0x00012800 6245005f 5a4e3636 5f244c54 2470796f bE._ZN66_$LT$pyo
-  0x00012810 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00012820 79494f45 72726f72 24753230 24617324 yIOError$u20$as$
-  0x00012830 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00012840 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
-  0x00012850 68343638 34623836 33633734 30356332 h4684b863c7405c2
-  0x00012860 3445005f 5a4e3636 5f244c54 2470796f 4E._ZN66_$LT$pyo
-  0x00012870 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00012880 79576172 6e696e67 24753230 24617324 yWarning$u20$as$
-  0x00012890 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x000128a0 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
-  0x000128b0 68633561 61623830 32333639 61356265 hc5aab802369a5be
-  0x000128c0 3845005f 5a4e3470 796f3335 74797065 8E._ZN4pyo35type
-  0x000128d0 7333616e 79355079 416e7937 67657461 s3any5PyAny7geta
-  0x000128e0 74747231 37686364 38353164 62343365 ttr17hcd851db43e
-  0x000128f0 35363835 31334500 5f5a4e34 636f7265 568513E._ZN4core
-  0x00012900 33707472 39376472 6f705f69 6e5f706c 3ptr97drop_in_pl
-  0x00012910 61636524 4c542470 796f332e 2e657272 ace$LT$pyo3..err
-  0x00012920 2e2e6572 725f7374 6174652e 2e626f78 ..err_state..box
-  0x00012930 65645f61 72677324 4c542424 52462473 ed_args$LT$$RF$s
-  0x00012940 74722447 54242e2e 24753762 24247537 tr$GT$..$u7b$$u7
-  0x00012950 6224636c 6f737572 65247537 64242475 b$closure$u7d$$u
-  0x00012960 37642424 47542431 37683266 38633161 7d$$GT$17h2f8c1a
-  0x00012970 65313363 61616262 3130452e 6c6c766d e13caabb10E.llvm
-  0x00012980 2e333136 30393037 32383138 38303738 .316090728188078
-  0x00012990 31313233 005f5a4e 34636f72 65337074 1123._ZN4core3pt
-  0x000129a0 72313232 64726f70 5f696e5f 706c6163 r122drop_in_plac
-  0x000129b0 65244c54 24616c6c 6f632e2e 7665632e e$LT$alloc..vec.
-  0x000129c0 2e696e74 6f5f6974 65722e2e 496e746f .into_iter..Into
-  0x000129d0 49746572 244c5424 636f7265 2e2e7074 Iter$LT$core..pt
-  0x000129e0 722e2e6e 6f6e5f6e 756c6c2e 2e4e6f6e r..non_null..Non
-  0x000129f0 4e756c6c 244c5424 70796f33 5f666669 Null$LT$pyo3_ffi
-  0x00012a00 2e2e6f62 6a656374 2e2e5079 4f626a65 ..object..PyObje
-  0x00012a10 63742447 54242447 54242447 54243137 ct$GT$$GT$$GT$17
-  0x00012a20 68333534 65363562 32633334 36323231 h354e65b2c346221
-  0x00012a30 31452e6c 6c766d2e 31333233 38383933 1E.llvm.13238893
-  0x00012a40 34333232 30303639 32323236 00727573 432200692226.rus
-  0x00012a50 745f6265 67696e5f 756e7769 6e640061 t_begin_unwind.a
-  0x00012a60 6e6f6e2e 35313035 62646437 39663233 non.5105bdd79f23
-  0x00012a70 62313137 31663338 37343266 65616163 b1171f38742feaac
-  0x00012a80 35643137 2e32352e 6c6c766d 2e333136 5d17.25.llvm.316
-  0x00012a90 30393037 32383138 38303738 31313233 0907281880781123
-  0x00012aa0 005f5a4e 34636f72 65337074 72333764 ._ZN4core3ptr37d
-  0x00012ab0 726f705f 696e5f70 6c616365 244c5424 rop_in_place$LT$
-  0x00012ac0 70796f33 2e2e6572 722e2e50 79457272 pyo3..err..PyErr
-  0x00012ad0 24475424 31376862 64373435 37623032 $GT$17hbd7457b02
-  0x00012ae0 30353733 64316245 2e6c6c76 6d2e3133 0573d1bE.llvm.13
-  0x00012af0 32333838 39333433 32323030 36393232 2388934322006922
-  0x00012b00 3236005f 5a4e3733 5f244c54 2470796f 26._ZN73_$LT$pyo
-  0x00012b10 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00012b20 79496e74 65727275 70746564 4572726f yInterruptedErro
-  0x00012b30 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x00012b40 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x00012b50 2433666d 74313768 62373261 30323261 $3fmt17hb72a022a
-  0x00012b60 37613662 64326139 45005f5a 4e37345f 7a6bd2a9E._ZN74_
-  0x00012b70 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00012b80 696f6e73 2e2e5079 42726f6b 656e5069 ions..PyBrokenPi
-  0x00012b90 70654572 726f7224 75323024 61732475 peError$u20$as$u
-  0x00012ba0 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
-  0x00012bb0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
-  0x00012bc0 35326533 34643635 62623439 37343361 52e34d65bb49743a
-  0x00012bd0 45005f5a 4e347079 6f333131 74797065 E._ZN4pyo311type
-  0x00012be0 5f6f626a 65637431 30507954 79706549 _object10PyTypeI
-  0x00012bf0 6e666f31 31747970 655f6f62 6a656374 nfo11type_object
-  0x00012c00 31376835 31626561 39373962 32316137 17h51bea979b21a7
-  0x00012c10 39353745 005f5a4e 36385f24 4c542473 957E._ZN68_$LT$s
-  0x00012c20 74642e2e 7379732e 2e756e69 782e2e6f td..sys..unix..o
-  0x00012c30 735f7374 722e2e53 6c696365 24753230 s_str..Slice$u20
-  0x00012c40 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x00012c50 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
-  0x00012c60 6d743137 68376536 66646639 33326137 mt17h7e6fdf932a7
-  0x00012c70 63306436 3545005f 5a4e3463 6f726533 c0d65E._ZN4core3
-  0x00012c80 70747231 33326472 6f705f69 6e5f706c ptr132drop_in_pl
-  0x00012c90 61636524 4c542463 6f72652e 2e63656c ace$LT$core..cel
-  0x00012ca0 6c2e2e52 65664d75 74244c54 24616c6c l..RefMut$LT$all
-  0x00012cb0 6f632e2e 7665632e 2e566563 244c5424 oc..vec..Vec$LT$
-  0x00012cc0 636f7265 2e2e7074 722e2e6e 6f6e5f6e core..ptr..non_n
-  0x00012cd0 756c6c2e 2e4e6f6e 4e756c6c 244c5424 ull..NonNull$LT$
-  0x00012ce0 70796f33 5f666669 2e2e6f62 6a656374 pyo3_ffi..object
-  0x00012cf0 2e2e5079 4f626a65 63742447 54242447 ..PyObject$GT$$G
-  0x00012d00 54242447 54242447 54243137 68373366 T$$GT$$GT$17h73f
-  0x00012d10 30656563 35626361 35396162 33452e6c 0eec5bca59ab3E.l
-  0x00012d20 6c766d2e 31383335 36373530 34383536 lvm.183567504856
-  0x00012d30 31343531 33313239 005f5a4e 35616c6c 14513129._ZN5all
-  0x00012d40 6f633772 61775f76 65633137 63617061 oc7raw_vec17capa
-  0x00012d50 63697479 5f6f7665 72666c6f 77313768 city_overflow17h
-  0x00012d60 35363434 37356434 33616330 65333763 564475d43ac0e37c
-  0x00012d70 45005f5a 4e36365f 244c5424 70796f33 E._ZN66_$LT$pyo3
-  0x00012d80 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
-  0x00012d90 4f534572 726f7224 75323024 61732475 OSError$u20$as$u
-  0x00012da0 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
-  0x00012db0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
-  0x00012dc0 65646161 37313563 63353363 33306133 edaa715cc53c30a3
-  0x00012dd0 45005f5a 4e337374 64337379 7334756e E._ZN3std3sys4un
-  0x00012de0 6978356c 6f636b73 31326675 7465785f ix5locks12futex_
-  0x00012df0 72776c6f 636b3652 774c6f63 6b313472 rwlock6RwLock14r
-  0x00012e00 6561645f 636f6e74 656e6465 64313768 ead_contended17h
-  0x00012e10 38643264 34663235 66613765 32636666 8d2d4f25fa7e2cff
-  0x00012e20 45005f5a 4e34636f 72653366 6d74336e E._ZN4core3fmt3n
-  0x00012e30 756d3369 6d703531 5f244c54 24696d70 um3imp51_$LT$imp
-  0x00012e40 6c247532 3024636f 72652e2e 666d742e l$u20$core..fmt.
-  0x00012e50 2e446973 706c6179 24753230 24666f72 .Display$u20$for
-  0x00012e60 24753230 24753824 47542433 666d7431 $u20$u8$GT$3fmt1
-  0x00012e70 37686534 39313863 37383231 36623839 7he4918c78216b89
-  0x00012e80 39354500 5f5a4e38 325f244c 5424636f 95E._ZN82_$LT$co
-  0x00012e90 72652e2e 63686172 2e2e4573 63617065 re..char..Escape
-  0x00012ea0 44656275 67247532 30246173 24753230 Debug$u20$as$u20
-  0x00012eb0 24636f72 652e2e69 7465722e 2e747261 $core..iter..tra
-  0x00012ec0 6974732e 2e697465 7261746f 722e2e49 its..iterator..I
-  0x00012ed0 74657261 746f7224 47542434 6e657874 terator$GT$4next
-  0x00012ee0 31376830 63653463 35626335 36643433 17h0ce4c5bc56d43
-  0x00012ef0 34396645 005f5a4e 34335f24 4c542463 49fE._ZN43_$LT$c
-  0x00012f00 68617224 75323024 61732475 32302463 har$u20$as$u20$c
-  0x00012f10 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
-  0x00012f20 79244754 2433666d 74313768 33316334 y$GT$3fmt17h31c4
-  0x00012f30 63323462 62643038 61613234 45005f5a c24bbd08aa24E._Z
-  0x00012f40 4e34636f 72653373 74723770 61747465 N4core3str7patte
-  0x00012f50 726e3131 53747253 65617263 68657233 rn11StrSearcher3
-  0x00012f60 6e657731 37683633 33363731 30333133 new17h6336710313
-  0x00012f70 61336266 35624500 616e6f6e 2e653965 a3bf5bE.anon.e9e
-  0x00012f80 62323337 63663530 61343362 36356436 b237cf50a43b65d6
-  0x00012f90 33366230 66343737 30623034 652e3334 36b0f4770b04e.34
-  0x00012fa0 2e6c6c76 6d2e3133 38363138 35323731 .llvm.1386185271
-  0x00012fb0 31333930 32373437 36005f5a 4e37315f 139027476._ZN71_
-  0x00012fc0 244c5424 72757374 635f6465 6d616e67 $LT$rustc_demang
-  0x00012fd0 6c652e2e 53697a65 4c696d69 74457868 le..SizeLimitExh
-  0x00012fe0 61757374 65642475 32302461 73247532 austed$u20$as$u2
-  0x00012ff0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x00013000 75672447 54243366 6d743137 68313461 ug$GT$3fmt17h14a
-  0x00013010 39353135 33383838 38636337 3445005f 951538888cc74E._
-  0x00013020 5a4e3736 5f244c54 2470796f 332e2e65 ZN76_$LT$pyo3..e
-  0x00013030 78636570 74696f6e 732e2e50 794d6f64 xceptions..PyMod
-  0x00013040 756c654e 6f74466f 756e6445 72726f72 uleNotFoundError
-  0x00013050 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00013060 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
-  0x00013070 33666d74 31376862 39306661 32653435 3fmt17hb90fa2e45
-  0x00013080 38643534 63643545 005f5a4e 3470796f 8d54cd5E._ZN4pyo
-  0x00013090 3335696d 706c5f39 70796d65 74686f64 35impl_9pymethod
-  0x000130a0 73313150 794d6574 686f6444 65663133 s11PyMethodDef13
-  0x000130b0 61735f6d 6574686f 645f6465 66313768 as_method_def17h
-  0x000130c0 36323464 62643262 63336135 61623361 624dbd2bc3a5ab3a
-  0x000130d0 45005f5f 544d435f 454e445f 5f005f5a E.__TMC_END__._Z
-  0x000130e0 4e37305f 244c5424 70796f33 2e2e6578 N70_$LT$pyo3..ex
-  0x000130f0 63657074 696f6e73 2e2e5079 53796e74 ceptions..PySynt
-  0x00013100 61785761 726e696e 67247532 30246173 axWarning$u20$as
-  0x00013110 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x00013120 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
-  0x00013130 62616565 61373866 62373663 62336661 baeea78fb76cb3fa
-  0x00013140 45005f5a 4e35385f 244c5424 616c6c6f E._ZN58_$LT$allo
-  0x00013150 632e2e73 7472696e 672e2e53 7472696e c..string..Strin
-  0x00013160 67247532 30246173 24753230 24636f72 g$u20$as$u20$cor
-  0x00013170 652e2e66 6d742e2e 57726974 65244754 e..fmt..Write$GT
-  0x00013180 24397772 6974655f 73747231 37686361 $9write_str17hca
-  0x00013190 62643366 63396637 34396165 3330452e bd3fc9f749ae30E.
-  0x000131a0 6c6c766d 2e353639 37393239 37363931 llvm.56979297691
-  0x000131b0 33333035 37343736 005f5a4e 36325f24 33057476._ZN62_$
-  0x000131c0 4c542470 796f332e 2e747970 65732e2e LT$pyo3..types..
-  0x000131d0 616e792e 2e507941 6e792475 32302461 any..PyAny$u20$a
-  0x000131e0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x000131f0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00013200 31376830 31626664 37666166 35616464 17h01bfd7faf5add
-  0x00013210 32656145 00616e6f 6e2e6239 61303438 2eaE.anon.b9a048
-  0x00013220 36633030 61343137 32623762 31616335 6c00a4172b7b1ac5
-  0x00013230 32623331 35616134 61332e33 382e6c6c 2b315aa4a3.38.ll
-  0x00013240 766d2e31 33323338 38393334 33323230 vm.1323889343220
-  0x00013250 30363932 32323600 5f5a4e34 70796f33 0692226._ZN4pyo3
-  0x00013260 3131636f 6e766572 73696f6e 73337374 11conversions3st
-  0x00013270 64367374 72696e67 38325f24 4c542469 d6string82_$LT$i
-  0x00013280 6d706c24 75323024 70796f33 2e2e636f mpl$u20$pyo3..co
-  0x00013290 6e766572 73696f6e 2e2e4672 6f6d5079 nversion..FromPy
-  0x000132a0 4f626a65 63742475 32302466 6f722475 Object$u20$for$u
-  0x000132b0 32302461 6c6c6f63 2e2e7374 72696e67 20$alloc..string
-  0x000132c0 2e2e5374 72696e67 24475424 37657874 ..String$GT$7ext
-  0x000132d0 72616374 31376830 38613037 33393561 ract17h08a07395a
-  0x000132e0 35336564 30393845 005f5a4e 31367061 53ed098E._ZN16pa
-  0x000132f0 726b696e 675f6c6f 745f636f 72653131 rking_lot_core11
-  0x00013300 7061726b 696e675f 6c6f7439 48415348 parking_lot9HASH
-  0x00013310 5441424c 45313768 39666364 36623530 TABLE17h9fcd6b50
-  0x00013320 36353864 37373930 45005f5a 4e37325f 658d7790E._ZN72_
-  0x00013330 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00013340 696f6e73 2e2e5079 41726974 686d6574 ions..PyArithmet
-  0x00013350 69634572 726f7224 75323024 61732475 icError$u20$as$u
-  0x00013360 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x00013370 62756724 47542433 666d7431 37683864 bug$GT$3fmt17h8d
-  0x00013380 35383330 33323933 32643332 35384500 583032932d3258E.
-  0x00013390 5f5a4e34 315f244c 54246368 61722475 _ZN41_$LT$char$u
-  0x000133a0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x000133b0 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
-  0x000133c0 6d743137 68616363 61316530 38353438 mt17hacca1e08548
-  0x000133d0 35333266 3145005f 5a4e3373 74643970 532f1E._ZN3std9p
-  0x000133e0 616e6963 6b696e67 31316265 67696e5f anicking11begin_
-  0x000133f0 70616e69 63313768 37613363 65663763 panic17h7a3cef7c
-  0x00013400 39346533 37356238 45005f5a 4e34636f 94e375b8E._ZN4co
-  0x00013410 72653366 6d743862 75696c64 65727331 re3fmt8builders1
-  0x00013420 31446562 75675374 72756374 35666965 1DebugStruct5fie
-  0x00013430 6c643137 68333461 63316262 63383861 ld17h34ac1bbc88a
-  0x00013440 37396163 3345005f 5a4e3931 5f244c54 79ac3E._ZN91_$LT
-  0x00013450 24737464 2e2e7061 6e69636b 696e672e $std..panicking.
-  0x00013460 2e727573 745f7061 6e69635f 77697468 .rust_panic_with
-  0x00013470 6f75745f 686f6f6b 2e2e5265 77726170 out_hook..Rewrap
-  0x00013480 426f7824 75323024 61732475 32302463 Box$u20$as$u20$c
-  0x00013490 6f72652e 2e70616e 69632e2e 426f784d ore..panic..BoxM
-  0x000134a0 65557024 47542433 67657431 37686439 eUp$GT$3get17hd9
-  0x000134b0 35383738 63343462 65363932 39384500 5878c44be69298E.
-  0x000134c0 5f5a4e33 73746431 30737973 5f636f6d _ZN3std10sys_com
-  0x000134d0 6d6f6e39 6261636b 74726163 6532365f mon9backtrace26_
-  0x000134e0 5f727573 745f656e 645f7368 6f72745f _rust_end_short_
-  0x000134f0 6261636b 74726163 65313768 35313532 backtrace17h5152
-  0x00013500 65353338 33393536 66363532 45005f5a e5383956f652E._Z
-  0x00013510 4e34636f 72653366 6d74336e 756d3532 N4core3fmt3num52
-  0x00013520 5f244c54 24696d70 6c247532 3024636f _$LT$impl$u20$co
-  0x00013530 72652e2e 666d742e 2e4c6f77 65724865 re..fmt..LowerHe
-  0x00013540 78247532 3024666f 72247532 30247538 x$u20$for$u20$u8
-  0x00013550 24475424 33666d74 31376836 31646533 $GT$3fmt17h61de3
-  0x00013560 64643830 38363461 32646245 005f5a4e dd80864a2dbE._ZN
-  0x00013570 31347275 7374635f 64656d61 6e676c65 14rustc_demangle
-  0x00013580 3864656d 616e676c 65313768 31383332 8demangle17h1832
-  0x00013590 39643866 66333639 35653333 45005f5a 9d8ff3695e33E._Z
-  0x000135a0 4e35616c 6c6f6337 7261775f 76656331 N5alloc7raw_vec1
-  0x000135b0 39526177 56656324 4c542454 24432441 9RawVec$LT$T$C$A
-  0x000135c0 24475424 31367265 73657276 655f666f $GT$16reserve_fo
-  0x000135d0 725f7075 73683137 68336538 63623966 r_push17h3e8cb9f
-  0x000135e0 34313333 66373736 3645005f 5a4e3463 4133f7766E._ZN4c
-  0x000135f0 6f726533 70747236 3964726f 705f696e ore3ptr69drop_in
-  0x00013600 5f706c61 6365244c 5424616c 6c6f632e _place$LT$alloc.
-  0x00013610 2e626f72 726f772e 2e436f77 244c5424 .borrow..Cow$LT$
-  0x00013620 636f7265 2e2e6666 692e2e63 5f737472 core..ffi..c_str
-  0x00013630 2e2e4353 74722447 54242447 54243137 ..CStr$GT$$GT$17
-  0x00013640 68333437 33336165 33396530 36666433 h34733ae39e06fd3
-  0x00013650 32452e6c 6c766d2e 35363937 39323937 2E.llvm.56979297
-  0x00013660 36393133 33303537 34373600 5f5a4e34 69133057476._ZN4
-  0x00013670 636f7265 33666d74 336e756d 35335f24 core3fmt3num53_$
-  0x00013680 4c542469 6d706c24 75323024 636f7265 LT$impl$u20$core
-  0x00013690 2e2e666d 742e2e4c 6f776572 48657824 ..fmt..LowerHex$
-  0x000136a0 75323024 666f7224 75323024 69333224 u20$for$u20$i32$
-  0x000136b0 47542433 666d7431 37683733 34383138 GT$3fmt17h734818
-  0x000136c0 63386663 36326563 36624500 5f5a4e37 c8fc62ec6bE._ZN7
-  0x000136d0 305f244c 54247079 6f332e2e 65786365 0_$LT$pyo3..exce
-  0x000136e0 7074696f 6e732e2e 50794275 66666572 ptions..PyBuffer
-  0x000136f0 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x00013700 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
-  0x00013710 6c617924 47542433 666d7431 37686638 lay$GT$3fmt17hf8
-  0x00013720 63306534 31666434 37343930 33314500 c0e41fd4749031E.
-  0x00013730 5f5a4e34 636f7265 33666d74 38627569 _ZN4core3fmt8bui
-  0x00013740 6c646572 73394465 6275674c 69737436 lders9DebugList6
-  0x00013750 66696e69 73683137 68386466 34646433 finish17h8df4dd3
-  0x00013760 32643637 37346331 3645005f 5a4e3463 2d6774c16E._ZN4c
-  0x00013770 6f726533 6f707338 66756e63 74696f6e ore3ops8function
-  0x00013780 36466e4f 6e636534 3063616c 6c5f6f6e 6FnOnce40call_on
-  0x00013790 63652475 37622424 75376224 76746162 ce$u7b$$u7b$vtab
-  0x000137a0 6c652e73 68696d24 75376424 24753764 le.shim$u7d$$u7d
-  0x000137b0 24313768 31343965 37363032 35386232 $17h149e760258b2
-  0x000137c0 63303334 452e6c6c 766d2e33 31363039 c034E.llvm.31609
-  0x000137d0 30373238 31383830 37383131 3233005f 07281880781123._
-  0x000137e0 5a4e3638 5f244c54 2470796f 332e2e65 ZN68_$LT$pyo3..e
-  0x000137f0 78636570 74696f6e 732e2e50 79496d70 xceptions..PyImp
-  0x00013800 6f727445 72726f72 24753230 24617324 ortError$u20$as$
-  0x00013810 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00013820 65627567 24475424 33666d74 31376862 ebug$GT$3fmt17hb
-  0x00013830 36366635 39316336 64313234 61623045 66f591c6d124ab0E
-  0x00013840 005f5a4e 39335f24 4c542473 74642e2e ._ZN93_$LT$std..
-  0x00013850 70616e69 636b696e 672e2e62 6567696e panicking..begin
-  0x00013860 5f70616e 69635f68 616e646c 65722e2e _panic_handler..
-  0x00013870 53747250 616e6963 5061796c 6f616424 StrPanicPayload$
-  0x00013880 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x00013890 2e70616e 69632e2e 426f784d 65557024 .panic..BoxMeUp$
-  0x000138a0 47542433 67657431 37686335 39626463 GT$3get17hc59bdc
-  0x000138b0 66353836 66656637 36634500 5f5a4e34 f586fef76cE._ZN4
-  0x000138c0 636f7265 33666d74 336e756d 33696d70 core3fmt3num3imp
-  0x000138d0 35325f24 4c542469 6d706c24 75323024 52_$LT$impl$u20$
-  0x000138e0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x000138f0 61792475 32302466 6f722475 32302475 ay$u20$for$u20$u
-  0x00013900 33322447 54243366 6d743137 68653432 32$GT$3fmt17he42
-  0x00013910 32623831 39393931 30643434 3845005f 2b8199910d448E._
-  0x00013920 5a4e3567 696d6c69 36636f6d 6d6f6e39 ZN5gimli6common9
-  0x00013930 53656374 696f6e49 64346e61 6d653137 SectionId4name17
-  0x00013940 68623139 65636163 66343635 37353866 hb19ecacf465758f
-  0x00013950 3145005f 5a4e3373 74643561 6c6c6f63 1E._ZN3std5alloc
-  0x00013960 38727573 745f6f6f 6d313768 62623263 8rust_oom17hbb2c
-  0x00013970 66343837 35363734 32336639 45005f5f f487567423f9E.__
-  0x00013980 72675f6f 6f6d005f 5a4e3873 6d616c6c rg_oom._ZN8small
-  0x00013990 76656331 37536d61 6c6c5665 63244c54 vec17SmallVec$LT
-  0x000139a0 24412447 54243131 7472795f 72657365 $A$GT$11try_rese
-  0x000139b0 72766531 37683531 37393330 37386366 rve17h51793078cf
-  0x000139c0 62356536 64384500 5f5a4e36 305f244c b5e6d8E._ZN60_$L
-  0x000139d0 54247374 642e2e74 696d652e 2e496e73 T$std..time..Ins
-  0x000139e0 74616e74 24753230 24617324 75323024 tant$u20$as$u20$
-  0x000139f0 636f7265 2e2e6f70 732e2e61 72697468 core..ops..arith
-  0x00013a00 2e2e5375 62244754 24337375 62313768 ..Sub$GT$3sub17h
-  0x00013a10 61646430 63646364 38303332 61326461 add0cdcd8032a2da
-  0x00013a20 4500616e 6f6e2e30 64626133 64326361 E.anon.0dba3d2ca
-  0x00013a30 61636634 35386663 34343331 31373537 acf458fc44311757
-  0x00013a40 33363162 6333612e 302e6c6c 766d2e31 361bc3a.0.llvm.1
-  0x00013a50 31323133 38383937 36333630 35363333 1213889763605633
-  0x00013a60 34393300 5f5a4e34 70796f33 35747970 493._ZN4pyo35typ
-  0x00013a70 65733574 75706c65 37507954 75706c65 es5tuple7PyTuple
-  0x00013a80 31386765 745f6974 656d5f75 6e636865 18get_item_unche
-  0x00013a90 636b6564 31376863 36376634 38633665 cked17hc67f48c6e
-  0x00013aa0 39303232 65626545 005f5a4e 37325f24 9022ebeE._ZN72_$
-  0x00013ab0 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x00013ac0 6f6e732e 2e507942 6c6f636b 696e6749 ons..PyBlockingI
-  0x00013ad0 4f457272 6f722475 32302461 73247532 OError$u20$as$u2
-  0x00013ae0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x00013af0 75672447 54243366 6d743137 68653464 ug$GT$3fmt17he4d
-  0x00013b00 64383432 61653461 66636532 3345005f d842ae4afce23E._
-  0x00013b10 5a4e3730 5f244c54 2470796f 332e2e65 ZN70_$LT$pyo3..e
-  0x00013b20 78636570 74696f6e 732e2e50 79426173 xceptions..PyBas
-  0x00013b30 65457863 65707469 6f6e2475 32302461 eException$u20$a
-  0x00013b40 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00013b50 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x00013b60 68666431 65373063 39623338 37643632 hfd1e70c9b387d62
-  0x00013b70 3945005f 5a4e3470 796f3333 67696c38 9E._ZN4pyo33gil8
-  0x00013b80 47494c47 75617264 31376163 71756972 GILGuard17acquir
-  0x00013b90 655f756e 63686563 6b656431 37683038 e_unchecked17h08
-  0x00013ba0 65346165 32373835 61313131 6232452e e4ae2785a111b2E.
-  0x00013bb0 6c6c766d 2e313332 33383839 33343332 llvm.13238893432
-  0x00013bc0 32303036 39323232 36005f5a 4e34636f 200692226._ZN4co
-  0x00013bd0 7265336f 70733866 756e6374 696f6e36 re3ops8function6
-  0x00013be0 466e4f6e 63653430 63616c6c 5f6f6e63 FnOnce40call_onc
-  0x00013bf0 65247537 62242475 37622476 7461626c e$u7b$$u7b$vtabl
-  0x00013c00 652e7368 696d2475 37642424 75376424 e.shim$u7d$$u7d$
-  0x00013c10 31376837 64356566 62316137 62636631 17h7d5efb1a7bcf1
-  0x00013c20 33396245 2e6c6c76 6d2e3331 36303930 39bE.llvm.316090
-  0x00013c30 37323831 38383037 38313132 33005f5a 7281880781123._Z
-  0x00013c40 4e34636f 72653370 74723132 3364726f N4core3ptr123dro
-  0x00013c50 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
-  0x00013c60 6f332e2e 6572722e 2e657272 5f737461 o3..err..err_sta
-  0x00013c70 74652e2e 626f7865 645f6172 6773244c te..boxed_args$L
-  0x00013c80 5424636f 72652e2e 6e756d2e 2e657272 T$core..num..err
-  0x00013c90 6f722e2e 54727946 726f6d49 6e744572 or..TryFromIntEr
-  0x00013ca0 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
-  0x00013cb0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x00013cc0 75376424 24475424 31376837 32666432 u7d$$GT$17h72fd2
-  0x00013cd0 37636661 63653538 64316345 2e6c6c76 7cface58d1cE.llv
-  0x00013ce0 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x00013cf0 38313132 33005f5a 4e39315f 244c5424 81123._ZN91_$LT$
-  0x00013d00 7374642e 2e70616e 69636b69 6e672e2e std..panicking..
-  0x00013d10 62656769 6e5f7061 6e69632e 2e50616e begin_panic..Pan
-  0x00013d20 69635061 796c6f61 64244c54 24412447 icPayload$LT$A$G
-  0x00013d30 54242475 32302461 73247532 3024636f T$$u20$as$u20$co
-  0x00013d40 72652e2e 70616e69 632e2e42 6f784d65 re..panic..BoxMe
-  0x00013d50 55702447 54243367 65743137 68643837 Up$GT$3get17hd87
-  0x00013d60 63303932 64393739 32656565 3045005f c092d9792eee0E._
-  0x00013d70 5a4e3463 6f726533 666d7438 6275696c ZN4core3fmt8buil
-  0x00013d80 64657273 38446562 75675365 7435656e ders8DebugSet5en
-  0x00013d90 74727931 37683739 36313134 34656431 try17h7961144ed1
-  0x00013da0 62613166 31364500 5f5f7275 73745f61 ba1f16E.__rust_a
-  0x00013db0 6c6c6f63 5f657272 6f725f68 616e646c lloc_error_handl
-  0x00013dc0 65725f73 686f756c 645f7061 6e696300 er_should_panic.
-  0x00013dd0 5f5a4e33 73746435 70616e69 63313372 _ZN3std5panic13r
-  0x00013de0 6573756d 655f756e 77696e64 31376862 esume_unwind17hb
-  0x00013df0 30643261 31386337 37613233 64653645 0d2a18c77a23de6E
-  0x00013e00 005f5a4e 3470796f 3338696e 7374616e ._ZN4pyo38instan
-  0x00013e10 63653132 50794e61 74697665 54797065 ce12PyNativeType
-  0x00013e20 3138756e 63686563 6b65645f 646f776e 18unchecked_down
-  0x00013e30 63617374 31376865 33383534 39663231 cast17he38549f21
-  0x00013e40 36363333 34613445 005f5a4e 33737464 66334a4E._ZN3std
-  0x00013e50 33737973 34756e69 78313774 68726561 3sys4unix17threa
-  0x00013e60 645f6c6f 63616c5f 64746f72 31337265 d_local_dtor13re
-  0x00013e70 67697374 65725f64 746f7231 37683133 gister_dtor17h13
-  0x00013e80 65363933 38316663 31306334 66644500 e69381fc10c4fdE.
-  0x00013e90 5f5a4e31 30375f24 4c542473 74642e2e _ZN107_$LT$std..
-  0x00013ea0 73796e63 2e2e6d70 73632e2e 52656376 sync..mpsc..Recv
-  0x00013eb0 54696d65 6f757445 72726f72 24753230 TimeoutError$u20
-  0x00013ec0 24617324 75323024 636f7265 2e2e636f $as$u20$core..co
-  0x00013ed0 6e766572 742e2e46 726f6d24 4c542473 nvert..From$LT$s
-  0x00013ee0 74642e2e 73796e63 2e2e6d70 73632e2e td..sync..mpsc..
-  0x00013ef0 52656376 4572726f 72244754 24244754 RecvError$GT$$GT
-  0x00013f00 24346672 6f6d3137 68383039 66656165 $4from17h809feae
-  0x00013f10 38336332 35616138 6145005f 5a4e3463 83c25aa8aE._ZN4c
-  0x00013f20 6f726539 70616e69 636b696e 67313870 ore9panicking18p
-  0x00013f30 616e6963 5f6e6f75 6e77696e 645f666d anic_nounwind_fm
-  0x00013f40 74313768 35323038 33336431 34343766 t17h520833d1447f
-  0x00013f50 34386539 45005f5a 4e337374 64337379 48e9E._ZN3std3sy
-  0x00013f60 7334756e 69783573 7464696f 31327061 s4unix5stdio12pa
-  0x00013f70 6e69635f 6f757470 75743137 68313961 nic_output17h19a
-  0x00013f80 32353430 33386131 66646531 38450061 254038a1fde18E.a
-  0x00013f90 6e6f6e2e 37623934 36616531 64336136 non.7b946ae1d3a6
-  0x00013fa0 36363739 37653264 62316633 36653463 66797e2db1f36e4c
-  0x00013fb0 64366537 2e31352e 6c6c766d 2e313833 d6e7.15.llvm.183
-  0x00013fc0 35363735 30343835 36313435 31333132 5675048561451312
-  0x00013fd0 3900616e 6f6e2e36 38326630 35336261 9.anon.682f053ba
-  0x00013fe0 33643664 31346166 35623237 63666362 3d6d14af5b27cfcb
-  0x00013ff0 62643136 3336332e 322e6c6c 766d2e35 bd16363.2.llvm.5
-  0x00014000 36393739 32393736 39313333 30353734 6979297691330574
-  0x00014010 3736005f 5a4e3373 74643674 68726561 76._ZN3std6threa
-  0x00014020 64397969 656c645f 6e6f7731 37683139 d9yield_now17h19
-  0x00014030 38383033 61636338 30643432 32394500 8803acc80d4229E.
-  0x00014040 5f5a4e34 636f7265 33666d74 39466f72 _ZN4core3fmt9For
-  0x00014050 6d617474 65723236 64656275 675f7374 matter26debug_st
-  0x00014060 72756374 5f666965 6c64325f 66696e69 ruct_field2_fini
-  0x00014070 73683137 68363930 36313831 33663262 sh17h69061813f2b
-  0x00014080 38643234 3345005f 5a4e3470 796f3335 8d243E._ZN4pyo35
-  0x00014090 74797065 73386675 6e637469 6f6e3131 types8function11
-  0x000140a0 50794346 756e6374 696f6e31 32696e74 PyCFunction12int
-  0x000140b0 65726e61 6c5f6e65 77313768 35333561 ernal_new17h535a
-  0x000140c0 35333666 63303137 65316338 45005f5a 536fc017e1c8E._Z
-  0x000140d0 4e36385f 244c5424 70796f33 2e2e7479 N68_$LT$pyo3..ty
-  0x000140e0 7065732e 2e6d6170 70696e67 2e2e5079 pes..mapping..Py
-  0x000140f0 4d617070 696e6724 75323024 61732475 Mapping$u20$as$u
-  0x00014100 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x00014110 62756724 47542433 666d7431 37686363 bug$GT$3fmt17hcc
-  0x00014120 38316334 64396634 33363331 38644500 81c4d9f436318dE.
-  0x00014130 5f5a4e34 70796f33 35696d70 6c5f3136 _ZN4pyo35impl_16
-  0x00014140 65787472 6163745f 61726775 6d656e74 extract_argument
-  0x00014150 31394675 6e637469 6f6e4465 73637269 19FunctionDescri
-  0x00014160 7074696f 6e323665 78747261 63745f61 ption26extract_a
-  0x00014170 7267756d 656e7473 5f666173 7463616c rguments_fastcal
-  0x00014180 6c313768 63623338 65393335 33666265 l17hcb38e9353fbe
-  0x00014190 30313961 45005f5a 4e337374 64367468 019aE._ZN3std6th
-  0x000141a0 72656164 356c6f63 616c3466 61737431 read5local4fast1
-  0x000141b0 324b6579 244c5424 54244754 24313474 2Key$LT$T$GT$14t
-  0x000141c0 72795f69 6e697469 616c697a 65313768 ry_initialize17h
-  0x000141d0 38633438 36613933 37626237 33336663 8c486a937bb733fc
-  0x000141e0 452e6c6c 766d2e33 31363039 30373238 E.llvm.316090728
-  0x000141f0 31383830 37383131 3233005f 5a4e3463 1880781123._ZN4c
-  0x00014200 6f726539 70616e69 636b696e 67313870 ore9panicking18p
-  0x00014210 616e6963 5f626f75 6e64735f 63686563 anic_bounds_chec
-  0x00014220 6b313768 61663036 66656662 32336562 k17haf06fefb23eb
-  0x00014230 61383264 45005f5a 4e35616c 6c6f6337 a82dE._ZN5alloc7
-  0x00014240 7261775f 76656331 39526177 56656324 raw_vec19RawVec$
-  0x00014250 4c542454 24432441 24475424 37726573 LT$T$C$A$GT$7res
-  0x00014260 65727665 3231646f 5f726573 65727665 erve21do_reserve
-  0x00014270 5f616e64 5f68616e 646c6531 37686132 _and_handle17ha2
-  0x00014280 35643062 38333363 31663462 63344500 5d0b833c1f4bc4E.
-  0x00014290 5f5a4e37 325f244c 54247079 6f332e2e _ZN72_$LT$pyo3..
-  0x000142a0 65786365 7074696f 6e732e2e 50794272 exceptions..PyBr
-  0x000142b0 6f6b656e 50697065 4572726f 72247532 okenPipeError$u2
-  0x000142c0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x000142d0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
-  0x000142e0 74313768 63373062 36636437 36376332 t17hc70b6cd767c2
-  0x000142f0 34363964 45005f5a 4e34636f 72653366 469dE._ZN4core3f
-  0x00014300 6d74336e 756d3535 5f244c54 24696d70 mt3num55_$LT$imp
-  0x00014310 6c247532 3024636f 72652e2e 666d742e l$u20$core..fmt.
-  0x00014320 2e557070 65724865 78247532 3024666f .UpperHex$u20$fo
-  0x00014330 72247532 30247573 697a6524 47542433 r$u20$usize$GT$3
-  0x00014340 666d7431 37683362 38646637 66373734 fmt17h3b8df7f774
-  0x00014350 33613062 63314500 5f5a4e37 335f244c 3a0bc1E._ZN73_$L
-  0x00014360 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x00014370 6e732e2e 6173796e 63696f2e 2e517565 ns..asyncio..Que
-  0x00014380 75654675 6c6c2475 32302461 73247532 ueFull$u20$as$u2
-  0x00014390 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x000143a0 75672447 54243366 6d743137 68616531 ug$GT$3fmt17hae1
-  0x000143b0 36626561 39333261 36636433 6345005f 6bea932a6cd3cE._
-  0x000143c0 5a4e3736 5f244c54 2470796f 332e2e65 ZN76_$LT$pyo3..e
-  0x000143d0 78636570 74696f6e 732e2e50 7946696c xceptions..PyFil
-  0x000143e0 654e6f74 466f756e 64457272 6f722475 eNotFoundError$u
-  0x000143f0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00014400 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x00014410 33666d74 31376835 38333939 62643264 3fmt17h58399bd2d
-  0x00014420 63623232 62376645 005f5a4e 33737464 cb22b7fE._ZN3std
-  0x00014430 33656e76 375f7661 725f6f73 31376863 3env7_var_os17hc
-  0x00014440 61363034 39373234 62643530 37303745 a6049724bd50707E
-  0x00014450 005f5a4e 35616c6c 6f633573 6c696365 ._ZN5alloc5slice
-  0x00014460 36345f24 4c542469 6d706c24 75323024 64_$LT$impl$u20$
-  0x00014470 616c6c6f 632e2e62 6f72726f 772e2e54 alloc..borrow..T
-  0x00014480 6f4f776e 65642475 32302466 6f722475 oOwned$u20$for$u
-  0x00014490 32302424 75356224 54247535 64242447 20$$u5b$T$u5d$$G
-  0x000144a0 54243874 6f5f6f77 6e656431 37686230 T$8to_owned17hb0
-  0x000144b0 63643762 39316465 31323232 33354500 cd7b91de122235E.
-  0x000144c0 5f5f7275 73745f61 6c6c6f63 005f5a4e __rust_alloc._ZN
-  0x000144d0 35335f24 4c542470 796f332e 2e657272 53_$LT$pyo3..err
-  0x000144e0 2e2e5079 45727224 75323024 61732475 ..PyErr$u20$as$u
-  0x000144f0 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x00014500 62756724 47542433 666d7431 37683961 bug$GT$3fmt17h9a
-  0x00014510 31613835 65646633 39616237 61624500 1a85edf39ab7abE.
-  0x00014520 5f5a4e34 636f7265 33707472 37306472 _ZN4core3ptr70dr
-  0x00014530 6f705f69 6e5f706c 61636524 4c542470 op_in_place$LT$p
-  0x00014540 796f332e 2e696e73 74616e63 652e2e50 yo3..instance..P
-  0x00014550 79244c54 2470796f 332e2e74 79706573 y$LT$pyo3..types
-  0x00014560 2e2e616e 792e2e50 79416e79 24475424 ..any..PyAny$GT$
-  0x00014570 24475424 31376838 65333538 64656462 $GT$17h8e358dedb
-  0x00014580 64396531 36666345 2e6c6c76 6d2e3135 d9e16fcE.llvm.15
-  0x00014590 35353539 32313330 30363839 35373638 5559213006895768
-  0x000145a0 3939005f 5a4e3738 5f244c54 2470796f 99._ZN78_$LT$pyo
-  0x000145b0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x000145c0 79556e69 636f6465 5472616e 736c6174 yUnicodeTranslat
-  0x000145d0 65457272 6f722475 32302461 73247532 eError$u20$as$u2
-  0x000145e0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
-  0x000145f0 75672447 54243366 6d743137 68363964 ug$GT$3fmt17h69d
-  0x00014600 61366437 63333737 63306632 3545005f a6d7c377c0f25E._
-  0x00014610 5a4e3732 5f244c54 2470796f 332e2e65 ZN72_$LT$pyo3..e
-  0x00014620 78636570 74696f6e 732e2e50 79426173 xceptions..PyBas
-  0x00014630 65457863 65707469 6f6e2475 32302461 eException$u20$a
-  0x00014640 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00014650 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00014660 31376839 66386131 66303435 30613832 17h9f8a1f0450a82
-  0x00014670 30373745 005f5a4e 34636f72 6533666d 077E._ZN4core3fm
-  0x00014680 74386275 696c6465 72733130 44656275 t8builders10Debu
-  0x00014690 67547570 6c653666 696e6973 68313768 gTuple6finish17h
-  0x000146a0 65613361 39303564 62343638 61663537 ea3a905db468af57
-  0x000146b0 45005f5a 4e34636f 72653366 6d743946 E._ZN4core3fmt9F
-  0x000146c0 6f726d61 74746572 31327061 645f696e ormatter12pad_in
-  0x000146d0 74656772 616c3137 68363733 63613764 tegral17h673ca7d
-  0x000146e0 32396231 34333164 6245005f 5a4e3730 29b1431dbE._ZN70
-  0x000146f0 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
-  0x00014700 74696f6e 732e2e50 79557365 72576172 tions..PyUserWar
-  0x00014710 6e696e67 24753230 24617324 75323024 ning$u20$as$u20$
-  0x00014720 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x00014730 61792447 54243366 6d743137 68373039 ay$GT$3fmt17h709
-  0x00014740 64303466 33323536 37633266 3145005f d04f32567c2f1E._
-  0x00014750 5a4e3930 5f244c54 24737464 2e2e7061 ZN90_$LT$std..pa
-  0x00014760 6e69636b 696e672e 2e626567 696e5f70 nicking..begin_p
-  0x00014770 616e6963 5f68616e 646c6572 2e2e5061 anic_handler..Pa
-  0x00014780 6e696350 61796c6f 61642475 32302461 nicPayload$u20$a
-  0x00014790 73247532 3024636f 72652e2e 70616e69 s$u20$core..pani
-  0x000147a0 632e2e42 6f784d65 55702447 54243874 c..BoxMeUp$GT$8t
-  0x000147b0 616b655f 626f7831 37683333 32363866 ake_box17h33268f
-  0x000147c0 38346634 63366537 66364500 5f5a4e34 84f4c6e7f6E._ZN4
-  0x000147d0 70796f33 3367696c 3947494c 5f434f55 pyo33gil9GIL_COU
-  0x000147e0 4e54375f 5f676574 6974355f 5f4b4559 NT7__getit5__KEY
-  0x000147f0 31376862 64623538 35343265 64643037 17hbdb58542edd07
-  0x00014800 32373445 005f5a4e 37305f24 4c542470 274E._ZN70_$LT$p
-  0x00014810 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x00014820 2e507953 796e7461 78457272 6f722475 .PySyntaxError$u
-  0x00014830 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00014840 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x00014850 33666d74 31376862 65306431 31373134 3fmt17hbe0d11714
-  0x00014860 31353661 37656545 005f5a4e 34636f72 156a7eeE._ZN4cor
-  0x00014870 65337074 72353464 726f705f 696e5f70 e3ptr54drop_in_p
-  0x00014880 6c616365 244c5424 24524624 6d757424 lace$LT$$RF$mut$
-  0x00014890 75323024 616c6c6f 632e2e73 7472696e u20$alloc..strin
-  0x000148a0 672e2e53 7472696e 67244754 24313768 g..String$GT$17h
-  0x000148b0 39623732 35373836 32393737 33363433 9b72578629773643
-  0x000148c0 452e6c6c 766d2e33 30343133 39333935 E.llvm.304139395
-  0x000148d0 38353639 39373433 3439005f 5a4e3470 8569974349._ZN4p
-  0x000148e0 796f3331 31636f6e 76657273 696f6e73 yo311conversions
-  0x000148f0 33737464 36737472 696e6736 385f244c 3std6string68_$L
-  0x00014900 5424696d 706c2475 32302470 796f332e T$impl$u20$pyo3.
-  0x00014910 2e636f6e 76657273 696f6e2e 2e46726f .conversion..Fro
-  0x00014920 6d50794f 626a6563 74247532 3024666f mPyObject$u20$fo
-  0x00014930 72247532 30242452 46247374 72244754 r$u20$$RF$str$GT
-  0x00014940 24376578 74726163 74313768 65346666 $7extract17he4ff
-  0x00014950 30316638 66626166 62636239 45005f5a 01f8fbafbcb9E._Z
-  0x00014960 4e35616c 6c6f6335 616c6c6f 63313868 N5alloc5alloc18h
-  0x00014970 616e646c 655f616c 6c6f635f 6572726f andle_alloc_erro
-  0x00014980 72313768 30376564 62383761 61616232 r17h07edb87aaab2
-  0x00014990 34633334 45005f5a 4e34636f 72653370 4c34E._ZN4core3p
-  0x000149a0 74723730 64726f70 5f696e5f 706c6163 tr70drop_in_plac
-  0x000149b0 65244c54 2470796f 332e2e69 6e737461 e$LT$pyo3..insta
-  0x000149c0 6e63652e 2e507924 4c542470 796f332e nce..Py$LT$pyo3.
-  0x000149d0 2e747970 65732e2e 616e792e 2e507941 .types..any..PyA
-  0x000149e0 6e792447 54242447 54243137 68386365 ny$GT$$GT$17h8ce
-  0x000149f0 62613632 64626230 38346538 61452e6c ba62dbb084e8aE.l
-  0x00014a00 6c766d2e 33303431 33393339 35383536 lvm.304139395856
-  0x00014a10 39393734 33343900 5f5a4e34 636f7265 9974349._ZN4core
-  0x00014a20 33707472 38316472 6f705f69 6e5f706c 3ptr81drop_in_pl
-  0x00014a30 61636524 4c542463 6f72652e 2e6f7074 ace$LT$core..opt
-  0x00014a40 696f6e2e 2e4f7074 696f6e24 4c542470 ion..Option$LT$p
-  0x00014a50 796f332e 2e657272 2e2e6572 725f7374 yo3..err..err_st
-  0x00014a60 6174652e 2e507945 72725374 61746524 ate..PyErrState$
-  0x00014a70 47542424 47542431 37686338 30373966 GT$$GT$17hc8079f
-  0x00014a80 36346633 31623166 3130452e 6c6c766d 64f31b1f10E.llvm
-  0x00014a90 2e313338 36313835 32373131 33393032 .138618527113902
-  0x00014aa0 37343736 00616e6f 6e2e6234 62633165 7476.anon.b4bc1e
-  0x00014ab0 36646439 30383334 32663362 62353465 6dd908342f3bb54e
-  0x00014ac0 36333633 65663764 61382e32 302e6c6c 6363ef7da8.20.ll
-  0x00014ad0 766d2e36 35373230 36383037 31323833 vm.6572068071283
-  0x00014ae0 38353839 3239005f 5a4e3732 5f244c54 858929._ZN72_$LT
-  0x00014af0 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00014b00 732e2e50 79436f6e 6e656374 696f6e45 s..PyConnectionE
-  0x00014b10 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x00014b20 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00014b30 24475424 33666d74 31376864 61613463 $GT$3fmt17hdaa4c
-  0x00014b40 39376433 37623937 61383845 005f5a4e 97d37b97a88E._ZN
-  0x00014b50 3470796f 33313174 7970655f 6f626a65 4pyo311type_obje
-  0x00014b60 63743130 50795479 7065496e 666f3131 ct10PyTypeInfo11
-  0x00014b70 74797065 5f6f626a 65637431 37683337 type_object17h37
-  0x00014b80 38393764 32313739 34346134 33614500 897d217944a43aE.
-  0x00014b90 5f5a4e36 395f244c 54247079 6f332e2e _ZN69_$LT$pyo3..
-  0x00014ba0 65786365 7074696f 6e732e2e 5079556e exceptions..PyUn
-  0x00014bb0 69636f64 65457272 6f722475 32302461 icodeError$u20$a
-  0x00014bc0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00014bd0 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x00014be0 68393762 65653737 61326632 38373362 h97bee77a2f2873b
-  0x00014bf0 3845005f 5a4e3638 5f244c54 2470796f 8E._ZN68_$LT$pyo
-  0x00014c00 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00014c10 79457863 65707469 6f6e2475 32302461 yException$u20$a
-  0x00014c20 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00014c30 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00014c40 31376833 36366262 36373133 61316431 17h366bb6713a1d1
-  0x00014c50 30643045 005f5a4e 34636f72 65336f70 0d0E._ZN4core3op
-  0x00014c60 73386675 6e637469 6f6e3646 6e4f6e63 s8function6FnOnc
-  0x00014c70 65343063 616c6c5f 6f6e6365 24753762 e40call_once$u7b
-  0x00014c80 24247537 62247674 61626c65 2e736869 $$u7b$vtable.shi
-  0x00014c90 6d247537 64242475 37642431 37686363 m$u7d$$u7d$17hcc
-  0x00014ca0 38316436 36616263 31376431 3966452e 81d66abc17d19fE.
-  0x00014cb0 6c6c766d 2e333735 35343034 32313134 llvm.37554042114
-  0x00014cc0 32323239 30343036 005f5a4e 35385f24 22290406._ZN58_$
-  0x00014cd0 4c542473 74642e2e 696f2e2e 6572726f LT$std..io..erro
-  0x00014ce0 722e2e45 72726f72 24753230 24617324 r..Error$u20$as$
-  0x00014cf0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00014d00 65627567 24475424 33666d74 31376836 ebug$GT$3fmt17h6
-  0x00014d10 38646332 37306165 33653963 36386245 8dc270ae3e9c68bE
-  0x00014d20 005f5a4e 35385f24 4c542461 6c6c6f63 ._ZN58_$LT$alloc
-  0x00014d30 2e2e7374 72696e67 2e2e5374 72696e67 ..string..String
-  0x00014d40 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00014d50 2e2e666d 742e2e57 72697465 24475424 ..fmt..Write$GT$
-  0x00014d60 31307772 6974655f 63686172 31376831 10write_char17h1
-  0x00014d70 62366436 30366431 63623164 35623745 b6d606d1cb1d5b7E
-  0x00014d80 2e6c6c76 6d2e3536 39373932 39373639 .llvm.5697929769
-  0x00014d90 31333330 35373437 36005f5a 4e33365f 133057476._ZN36_
-  0x00014da0 244c5424 54247532 30246173 24753230 $LT$T$u20$as$u20
-  0x00014db0 24636f72 652e2e61 6e792e2e 416e7924 $core..any..Any$
-  0x00014dc0 47542437 74797065 5f696431 37683162 GT$7type_id17h1b
-  0x00014dd0 66666266 34323531 31636562 37324500 ffbf42511ceb72E.
-  0x00014de0 5f5a4e37 365f244c 54247079 6f332e2e _ZN76_$LT$pyo3..
-  0x00014df0 65786365 7074696f 6e732e2e 50795a65 exceptions..PyZe
-  0x00014e00 726f4469 76697369 6f6e4572 726f7224 roDivisionError$
-  0x00014e10 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x00014e20 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
-  0x00014e30 2433666d 74313768 39663538 30626636 $3fmt17h9f580bf6
-  0x00014e40 39643565 35643433 45005f5a 4e34636f 9d5e5d43E._ZN4co
-  0x00014e50 72653373 7472356c 6f737379 39557466 re3str5lossy9Utf
-  0x00014e60 38436875 6e6b3769 6e76616c 69643137 8Chunk7invalid17
-  0x00014e70 68386164 66626630 39316632 30396365 h8adfbf091f209ce
-  0x00014e80 3845005f 5a4e3373 74643674 68726561 8E._ZN3std6threa
-  0x00014e90 64356c6f 63616c34 66617374 31324b65 d5local4fast12Ke
-  0x00014ea0 79244c54 24542447 54243134 7472795f y$LT$T$GT$14try_
-  0x00014eb0 696e6974 69616c69 7a653137 68353165 initialize17h51e
-  0x00014ec0 33323039 63623639 36343836 63452e6c 3209cb696486cE.l
-  0x00014ed0 6c766d2e 33313630 39303732 38313838 lvm.316090728188
-  0x00014ee0 30373831 31323300 5f5a4e36 385f244c 0781123._ZN68_$L
-  0x00014ef0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x00014f00 6e732e2e 50795379 6e746178 4572726f ns..PySyntaxErro
-  0x00014f10 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x00014f20 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x00014f30 2433666d 74313768 38316339 38333435 $3fmt17h81c98345
-  0x00014f40 65386536 37643061 45005f5a 4e37375f e8e67d0aE._ZN77_
-  0x00014f50 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00014f60 696f6e73 2e2e5079 556e6963 6f646544 ions..PyUnicodeD
-  0x00014f70 65636f64 65457272 6f722475 32302461 ecodeError$u20$a
-  0x00014f80 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00014f90 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00014fa0 31376832 31636236 63316531 37326232 17h21cb6c1e172b2
-  0x00014fb0 66333945 005f5a4e 34325f24 4c542424 f39E._ZN42_$LT$$
-  0x00014fc0 52462454 24753230 24617324 75323024 RF$T$u20$as$u20$
-  0x00014fd0 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00014fe0 24475424 33666d74 31376838 30363861 $GT$3fmt17h8068a
-  0x00014ff0 30356463 34353135 31373345 005f5a4e 05dc4515173E._ZN
-  0x00015000 34636f72 6533666d 74336e75 6d35335f 4core3fmt3num53_
-  0x00015010 244c5424 696d706c 24753230 24636f72 $LT$impl$u20$cor
-  0x00015020 652e2e66 6d742e2e 55707065 72486578 e..fmt..UpperHex
-  0x00015030 24753230 24666f72 24753230 24753332 $u20$for$u20$u32
-  0x00015040 24475424 33666d74 31376866 34613163 $GT$3fmt17hf4a1c
-  0x00015050 35336665 63346464 61653045 005f5a4e 53fec4ddae0E._ZN
-  0x00015060 34636f72 65337074 72393264 726f705f 4core3ptr92drop_
-  0x00015070 696e5f70 6c616365 244c5424 7374642e in_place$LT$std.
-  0x00015080 2e696f2e 2e577269 74652e2e 77726974 .io..Write..writ
-  0x00015090 655f666d 742e2e41 64617074 6572244c e_fmt..Adapter$L
-  0x000150a0 54247374 642e2e73 79732e2e 756e6978 T$std..sys..unix
-  0x000150b0 2e2e7374 64696f2e 2e537464 65727224 ..stdio..Stderr$
-  0x000150c0 47542424 47542431 37686334 61313330 GT$$GT$17hc4a130
-  0x000150d0 63663065 64366231 3833452e 6c6c766d cf0ed6b183E.llvm
-  0x000150e0 2e383336 34373335 31373237 30333437 .836473517270347
-  0x000150f0 36333534 005f5a4e 33737464 36746872 6354._ZN3std6thr
-  0x00015100 65616435 6c6f6361 6c346661 73743132 ead5local4fast12
-  0x00015110 4b657924 4c542454 24475424 31347472 Key$LT$T$GT$14tr
-  0x00015120 795f696e 69746961 6c697a65 31376832 y_initialize17h2
-  0x00015130 36623533 66643732 65373535 64633545 6b53fd72e755dc5E
-  0x00015140 2e6c6c76 6d2e3331 30393632 35373132 .llvm.3109625712
-  0x00015150 34313635 30353335 33005f5a 4e34636f 416505353._ZN4co
-  0x00015160 72653370 74723434 64726f70 5f696e5f re3ptr44drop_in_
-  0x00015170 706c6163 65244c54 24636f72 652e2e63 place$LT$core..c
-  0x00015180 656c6c2e 2e426f72 726f7745 72726f72 ell..BorrowError
-  0x00015190 24475424 31376832 61336639 64343234 $GT$17h2a3f9d424
-  0x000151a0 30336638 31613545 2e6c6c76 6d2e3133 03f81a5E.llvm.13
-  0x000151b0 32333838 39333433 32323030 36393232 2388934322006922
-  0x000151c0 3236005f 5a4e3463 6f726539 70616e69 26._ZN4core9pani
-  0x000151d0 636b696e 67397061 6e69635f 666d7431 cking9panic_fmt1
-  0x000151e0 37686633 33613134 37356234 64633563 7hf33a1475b4dc5c
-  0x000151f0 33654500 5f5a4e37 355f244c 54247079 3eE._ZN75_$LT$py
-  0x00015200 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x00015210 50794465 70726563 6174696f 6e576172 PyDeprecationWar
-  0x00015220 6e696e67 24753230 24617324 75323024 ning$u20$as$u20$
-  0x00015230 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00015240 24475424 33666d74 31376864 65396566 $GT$3fmt17hde9ef
-  0x00015250 34663864 61353134 66613245 005f5a4e 4f8da514fa2E._ZN
-  0x00015260 34636f72 65357061 6e696331 3070616e 4core5panic10pan
-  0x00015270 69635f69 6e666f39 50616e69 63496e66 ic_info9PanicInf
-  0x00015280 6f386c6f 63617469 6f6e3137 68626635 o8location17hbf5
-  0x00015290 66646162 35336365 34656532 3545005f fdab53ce4ee25E._
-  0x000152a0 5a4e3833 5f244c54 24706172 6b696e67 ZN83_$LT$parking
-  0x000152b0 5f6c6f74 5f636f72 652e2e70 61726b69 _lot_core..parki
-  0x000152c0 6e675f6c 6f742e2e 54687265 61644461 ng_lot..ThreadDa
-  0x000152d0 74612475 32302461 73247532 3024636f ta$u20$as$u20$co
-  0x000152e0 72652e2e 6f70732e 2e64726f 702e2e44 re..ops..drop..D
-  0x000152f0 726f7024 47542434 64726f70 31376832 rop$GT$4drop17h2
-  0x00015300 39323238 37396232 61376432 30613045 922879b2a7d20a0E
-  0x00015310 005f5a4e 37395f24 4c542470 796f332e ._ZN79_$LT$pyo3.
-  0x00015320 2e657863 65707469 6f6e732e 2e507943 .exceptions..PyC
-  0x00015330 6f6e6e65 6374696f 6e41626f 72746564 onnectionAborted
-  0x00015340 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x00015350 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x00015360 67244754 2433666d 74313768 35353963 g$GT$3fmt17h559c
-  0x00015370 39313664 63366631 33646332 4500616e 916dc6f13dc2E.an
-  0x00015380 6f6e2e62 39613034 38366330 30613431 on.b9a0486c00a41
-  0x00015390 37326237 62316163 35326233 31356161 72b7b1ac52b315aa
-  0x000153a0 3461332e 302e6c6c 766d2e31 33323338 4a3.0.llvm.13238
-  0x000153b0 38393334 33323230 30363932 32323600 893432200692226.
-  0x000153c0 5f5a4e33 73746439 70616e69 636b696e _ZN3std9panickin
-  0x000153d0 67313264 65666175 6c745f68 6f6f6b31 g12default_hook1
-  0x000153e0 37686133 35303064 61353761 61346163 7ha3500da57aa4ac
-  0x000153f0 34664500 5f5a4e33 73746434 70617468 4fE._ZN3std4path
-  0x00015400 34506174 68366973 5f646972 31376836 4Path6is_dir17h6
-  0x00015410 66313166 35326265 66313330 62333945 f11f52bef130b39E
-  0x00015420 005f5a4e 33737464 3970616e 69636b69 ._ZN3std9panicki
-  0x00015430 6e673448 4f4f4b31 37683762 62363361 ng4HOOK17h7bb63a
-  0x00015440 36346164 35303130 38374500 5f5a4e34 64ad501087E._ZN4
-  0x00015450 636f7265 33707472 31323164 726f705f core3ptr121drop_
-  0x00015460 696e5f70 6c616365 244c5424 70796f33 in_place$LT$pyo3
-  0x00015470 2e2e6572 722e2e65 72725f73 74617465 ..err..err_state
-  0x00015480 2e2e626f 7865645f 61726773 244c5424 ..boxed_args$LT$
-  0x00015490 636f7265 2e2e6e75 6d2e2e65 72726f72 core..num..error
-  0x000154a0 2e2e5061 72736549 6e744572 726f7224 ..ParseIntError$
-  0x000154b0 4754242e 2e247537 62242475 37622463 GT$..$u7b$$u7b$c
-  0x000154c0 6c6f7375 72652475 37642424 75376424 losure$u7d$$u7d$
-  0x000154d0 24475424 31376862 62336531 65616638 $GT$17hbb3e1eaf8
-  0x000154e0 31623839 31383045 2e6c6c76 6d2e3331 1b89180E.llvm.31
-  0x000154f0 36303930 37323831 38383037 38313132 6090728188078112
-  0x00015500 33005f5a 4e38325f 244c5424 70796f33 3._ZN82_$LT$pyo3
-  0x00015510 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
-  0x00015520 50656e64 696e6744 65707265 63617469 PendingDeprecati
-  0x00015530 6f6e5761 726e696e 67247532 30246173 onWarning$u20$as
-  0x00015540 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x00015550 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
-  0x00015560 63346264 36646335 35366362 65643438 c4bd6dc556cbed48
-  0x00015570 4500616e 6f6e2e62 39613034 38366330 E.anon.b9a0486c0
-  0x00015580 30613431 37326237 62316163 35326233 0a4172b7b1ac52b3
-  0x00015590 31356161 3461332e 34302e6c 6c766d2e 15aa4a3.40.llvm.
-  0x000155a0 31333233 38383933 34333232 30303639 1323889343220069
-  0x000155b0 32323236 005f5a4e 34636f72 65337074 2226._ZN4core3pt
-  0x000155c0 72343864 726f705f 696e5f70 6c616365 r48drop_in_place
-  0x000155d0 244c5424 636f7265 2e2e7374 722e2e65 $LT$core..str..e
-  0x000155e0 72726f72 2e2e5574 66384572 726f7224 rror..Utf8Error$
-  0x000155f0 47542431 37683263 65333464 33643064 GT$17h2ce34d3d0d
-  0x00015600 39326633 3064452e 6c6c766d 2e313736 92f30dE.llvm.176
-  0x00015610 39353736 32333431 37383134 35333031 9576234178145301
-  0x00015620 32005f5a 4e347079 6f333131 74797065 2._ZN4pyo311type
-  0x00015630 5f6f626a 65637431 30507954 79706549 _object10PyTypeI
-  0x00015640 6e666f31 31747970 655f6f62 6a656374 nfo11type_object
-  0x00015650 31376862 30346661 34366266 65613535 17hb04fa46bfea55
-  0x00015660 32313645 005f5a4e 366d656d 63687236 216E._ZN6memchr6
-  0x00015670 6d656d63 68723378 38363473 73653236 memchr3x864sse26
-  0x00015680 6d656d63 68723137 68643138 32616166 memchr17hd182aaf
-  0x00015690 62643635 30333639 3345005f 5a4e3373 bd6503693E._ZN3s
-  0x000156a0 74643570 616e6963 31396765 745f6261 td5panic19get_ba
-  0x000156b0 636b7472 6163655f 7374796c 65313768 cktrace_style17h
-  0x000156c0 61613831 61323437 31346461 65653333 aa81a24714daee33
-  0x000156d0 45005f5a 4e34636f 72653370 74723437 E._ZN4core3ptr47
-  0x000156e0 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
-  0x000156f0 24636f72 652e2e63 656c6c2e 2e426f72 $core..cell..Bor
-  0x00015700 726f774d 75744572 726f7224 47542431 rowMutError$GT$1
-  0x00015710 37686264 65383065 61666362 37656330 7hbde80eafcb7ec0
-  0x00015720 3262452e 6c6c766d 2e313332 33383839 2bE.llvm.1323889
-  0x00015730 33343332 32303036 39323232 36005f5a 3432200692226._Z
-  0x00015740 4e39385f 244c5424 616c6c6f 632e2e76 N98_$LT$alloc..v
-  0x00015750 65632e2e 56656324 4c542454 24475424 ec..Vec$LT$T$GT$
-  0x00015760 24753230 24617324 75323024 616c6c6f $u20$as$u20$allo
-  0x00015770 632e2e76 65632e2e 73706563 5f66726f c..vec..spec_fro
-  0x00015780 6d5f6974 65722e2e 53706563 46726f6d m_iter..SpecFrom
-  0x00015790 49746572 244c5424 54244324 49244754 Iter$LT$T$C$I$GT
-  0x000157a0 24244754 24396672 6f6d5f69 74657231 $$GT$9from_iter1
-  0x000157b0 37683166 38616362 63663332 34646464 7h1f8acbcf324ddd
-  0x000157c0 34334500 616e6f6e 2e643139 66316461 43E.anon.d19f1da
-  0x000157d0 33366265 39626136 32373562 39636666 36be9ba6275b9cff
-  0x000157e0 31636264 64336439 372e302e 6c6c766d 1cbdd3d97.0.llvm
-  0x000157f0 2e313633 39353833 32353833 31373232 .163958325831722
-  0x00015800 30303232 31005f5a 4e347079 6f333367 00221._ZN4pyo33g
-  0x00015810 696c3133 4f574e45 445f4f42 4a454354 il13OWNED_OBJECT
-  0x00015820 53375f5f 67657469 74355f5f 4b455931 S7__getit5__KEY1
-  0x00015830 37686265 65643033 35386262 35653939 7hbeed0358bb5e99
-  0x00015840 38364500 5f5a4e38 385f244c 54247374 86E._ZN88_$LT$st
-  0x00015850 642e2e74 696d652e 2e496e73 74616e74 d..time..Instant
-  0x00015860 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00015870 2e2e6f70 732e2e61 72697468 2e2e4164 ..ops..arith..Ad
-  0x00015880 64244c54 24636f72 652e2e74 696d652e d$LT$core..time.
-  0x00015890 2e447572 6174696f 6e244754 24244754 .Duration$GT$$GT
-  0x000158a0 24336164 64313768 30363536 36633361 $3add17h06566c3a
-  0x000158b0 39343834 31613530 45005f5a 4e37375f 94841a50E._ZN77_
-  0x000158c0 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x000158d0 696f6e73 2e2e5079 44657072 65636174 ions..PyDeprecat
-  0x000158e0 696f6e57 61726e69 6e672475 32302461 ionWarning$u20$a
-  0x000158f0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00015900 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00015910 31376836 33366236 62336633 32313033 17h636b6b3f32103
-  0x00015920 39616445 00616e6f 6e2e3762 39343661 9adE.anon.7b946a
-  0x00015930 65316433 61363636 37393765 32646231 e1d3a666797e2db1
-  0x00015940 66333665 34636436 65372e39 2e6c6c76 f36e4cd6e7.9.llv
-  0x00015950 6d2e3138 33353637 35303438 35363134 m.18356750485614
-  0x00015960 35313331 3239005f 5a4e3730 5f244c54 513129._ZN70_$LT
-  0x00015970 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00015980 732e2e50 794c6f6f 6b757045 72726f72 s..PyLookupError
-  0x00015990 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x000159a0 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x000159b0 54243366 6d743137 68623535 66623537 T$3fmt17hb55fb57
-  0x000159c0 64323564 63366439 3745005f 5a4e3434 d25dc6d97E._ZN44
-  0x000159d0 5f244c54 24245246 24542475 32302461 _$LT$$RF$T$u20$a
-  0x000159e0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x000159f0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00015a00 31376833 38373232 39383435 63333431 17h387229845c341
-  0x00015a10 33666245 005f5a4e 36375f24 4c542470 3fbE._ZN67_$LT$p
-  0x00015a20 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x00015a30 2e507956 616c7565 4572726f 72247532 .PyValueError$u2
-  0x00015a40 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x00015a50 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
-  0x00015a60 74313768 34633931 64393230 30373330 t17h4c91d9200730
-  0x00015a70 34353938 4500616e 6f6e2e62 39613034 4598E.anon.b9a04
-  0x00015a80 38366330 30613431 37326237 62316163 86c00a4172b7b1ac
-  0x00015a90 35326233 31356161 3461332e 33392e6c 52b315aa4a3.39.l
-  0x00015aa0 6c766d2e 31333233 38383933 34333232 lvm.132388934322
-  0x00015ab0 30303639 32323236 005f5a4e 33737464 00692226._ZN3std
-  0x00015ac0 34706174 68345061 74683133 5f737472 4path4Path13_str
-  0x00015ad0 69705f70 72656669 78313768 39613265 ip_prefix17h9a2e
-  0x00015ae0 61383537 39333134 61383361 45005f5a a8579314a83aE._Z
-  0x00015af0 4e34636f 72653370 74723135 3564726f N4core3ptr155dro
-  0x00015b00 705f696e 5f706c61 6365244c 54247061 p_in_place$LT$pa
-  0x00015b10 726b696e 675f6c6f 742e2e6f 6e63652e rking_lot..once.
-  0x00015b20 2e4f6e63 652e2e63 616c6c5f 6f6e6365 .Once..call_once
-  0x00015b30 5f666f72 6365244c 54247079 6f332e2e _force$LT$pyo3..
-  0x00015b40 67696c2e 2e47494c 47756172 642e2e61 gil..GILGuard..a
-  0x00015b50 63717569 72652e2e 24753762 24247537 cquire..$u7b$$u7
-  0x00015b60 6224636c 6f737572 65247537 64242475 b$closure$u7d$$u
-  0x00015b70 37642424 4754242e 2e247537 62242475 7d$$GT$..$u7b$$u
-  0x00015b80 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x00015b90 75376424 24475424 31376830 37376630 u7d$$GT$17h077f0
-  0x00015ba0 30326534 32653237 32633745 2e6c6c76 02e42e272c7E.llv
-  0x00015bb0 6d2e3133 32333838 39333433 32323030 m.13238893432200
-  0x00015bc0 36393232 3236005f 5a4e3938 5f244c54 692226._ZN98_$LT
-  0x00015bd0 24616c6c 6f632e2e 73747269 6e672e2e $alloc..string..
-  0x00015be0 53747269 6e672475 32302461 73247532 String$u20$as$u2
-  0x00015bf0 3024636f 72652e2e 636f6e76 6572742e 0$core..convert.
-  0x00015c00 2e46726f 6d244c54 24616c6c 6f632e2e .From$LT$alloc..
-  0x00015c10 626f7272 6f772e2e 436f7724 4c542473 borrow..Cow$LT$s
-  0x00015c20 74722447 54242447 54242447 54243466 tr$GT$$GT$$GT$4f
-  0x00015c30 726f6d31 37683132 66386531 63313037 rom17h12f8e1c107
-  0x00015c40 65346438 31654500 616e6f6e 2e653965 e4d81eE.anon.e9e
-  0x00015c50 62323337 63663530 61343362 36356436 b237cf50a43b65d6
-  0x00015c60 33366230 66343737 30623034 652e3238 36b0f4770b04e.28
-  0x00015c70 2e6c6c76 6d2e3133 38363138 35323731 .llvm.1386185271
-  0x00015c80 31333930 32373437 36005f5a 4e35616c 139027476._ZN5al
-  0x00015c90 6c6f6336 73747269 6e673653 7472696e loc6string6Strin
-  0x00015ca0 67313566 726f6d5f 75746638 5f6c6f73 g15from_utf8_los
-  0x00015cb0 73793137 68663363 30313339 64626365 sy17hf3c0139dbce
-  0x00015cc0 64616666 3045005f 5a4e3463 6f726533 daff0E._ZN4core3
-  0x00015cd0 70747237 3164726f 705f696e 5f706c61 ptr71drop_in_pla
-  0x00015ce0 6365244c 5424636f 72652e2e 72657375 ce$LT$core..resu
-  0x00015cf0 6c742e2e 52657375 6c74244c 54246936 lt..Result$LT$i6
-  0x00015d00 34244324 70796f33 2e2e6572 722e2e50 4$C$pyo3..err..P
-  0x00015d10 79457272 24475424 24475424 31376833 yErr$GT$$GT$17h3
-  0x00015d20 64333236 62353337 33303161 32333145 d326b537301a231E
-  0x00015d30 2e6c6c76 6d2e3138 33353637 35303438 .llvm.1835675048
-  0x00015d40 35363134 35313331 3239005f 5a4e3463 5614513129._ZN4c
-  0x00015d50 6f726537 756e6963 6f646531 32756e69 ore7unicode12uni
-  0x00015d60 636f6465 5f646174 61326363 366c6f6f code_data2cc6loo
-  0x00015d70 6b757031 37686565 39643061 66373638 kup17hee9d0af768
-  0x00015d80 64613462 39334500 5f5a4e37 355f244c da4b93E._ZN75_$L
-  0x00015d90 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x00015da0 6e732e2e 5079466c 6f617469 6e67506f ns..PyFloatingPo
-  0x00015db0 696e7445 72726f72 24753230 24617324 intError$u20$as$
-  0x00015dc0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00015dd0 65627567 24475424 33666d74 31376861 ebug$GT$3fmt17ha
-  0x00015de0 65643338 36383130 33656161 32666645 ed3868103eaa2ffE
-  0x00015df0 005f5a4e 36315f24 4c542470 796f332e ._ZN61_$LT$pyo3.
-  0x00015e00 2e67696c 2e2e4749 4c477561 72642475 .gil..GILGuard$u
-  0x00015e10 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00015e20 6f70732e 2e64726f 702e2e44 726f7024 ops..drop..Drop$
-  0x00015e30 47542434 64726f70 31376837 37313561 GT$4drop17h7715a
-  0x00015e40 66656663 65323762 38656445 005f5a4e fefce27b8edE._ZN
-  0x00015e50 37345f24 4c542470 796f332e 2e657863 74_$LT$pyo3..exc
-  0x00015e60 65707469 6f6e732e 2e50795a 65726f44 eptions..PyZeroD
-  0x00015e70 69766973 696f6e45 72726f72 24753230 ivisionError$u20
-  0x00015e80 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x00015e90 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
-  0x00015ea0 31376832 38653834 65383661 34623436 17h28e84e86a4b46
-  0x00015eb0 36313945 005f5a4e 3470796f 33313174 619E._ZN4pyo311t
-  0x00015ec0 7970655f 6f626a65 63743130 50795479 ype_object10PyTy
-  0x00015ed0 7065496e 666f3131 74797065 5f6f626a peInfo11type_obj
-  0x00015ee0 65637431 37686335 33373139 61333762 ect17hc53719a37b
-  0x00015ef0 66323532 31304500 5f5a4e34 636f7265 f25210E._ZN4core
-  0x00015f00 33737472 35636f75 6e743233 63686172 3str5count23char
-  0x00015f10 5f636f75 6e745f67 656e6572 616c5f63 _count_general_c
-  0x00015f20 61736531 37686561 33356262 32343862 ase17hea35bb248b
-  0x00015f30 64306436 62374500 616e6f6e 2e393761 d0d6b7E.anon.97a
-  0x00015f40 64393331 63353463 38383563 61393664 d931c54c885ca96d
-  0x00015f50 66643732 65663130 61623033 382e3133 fd72ef10ab038.13
-  0x00015f60 2e6c6c76 6d2e3330 34313339 33393538 .llvm.3041393958
-  0x00015f70 35363939 37343334 39005f5a 4e37365f 569974349._ZN76_
-  0x00015f80 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00015f90 696f6e73 2e2e5079 556e626f 756e644c ions..PyUnboundL
-  0x00015fa0 6f63616c 4572726f 72247532 30246173 ocalError$u20$as
-  0x00015fb0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x00015fc0 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x00015fd0 37683961 37646466 66353436 34643937 7h9a7ddff5464d97
-  0x00015fe0 66644500 5f5a4e37 325f244c 54247079 fdE._ZN72_$LT$py
-  0x00015ff0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x00016000 50795065 726d6973 73696f6e 4572726f PyPermissionErro
-  0x00016010 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
-  0x00016020 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
-  0x00016030 2433666d 74313768 61663465 30343765 $3fmt17haf4e047e
-  0x00016040 31646639 35663830 45005f5a 4e36385f 1df95f80E._ZN68_
-  0x00016050 244c5424 636f7265 2e2e6e75 6d2e2e65 $LT$core..num..e
-  0x00016060 72726f72 2e2e5061 72736549 6e744572 rror..ParseIntEr
-  0x00016070 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x00016080 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x00016090 47542433 666d7431 37686465 61613433 GT$3fmt17hdeaa43
-  0x000160a0 37316333 34346538 66304500 616e6f6e 71c344e8f0E.anon
-  0x000160b0 2e653965 62323337 63663530 61343362 .e9eb237cf50a43b
-  0x000160c0 36356436 33366230 66343737 30623034 65d636b0f4770b04
-  0x000160d0 652e3531 2e6c6c76 6d2e3133 38363138 e.51.llvm.138618
-  0x000160e0 35323731 31333930 32373437 36005f5a 5271139027476._Z
-  0x000160f0 4e34636f 72653370 74723530 64726f70 N4core3ptr50drop
-  0x00016100 5f696e5f 706c6163 65244c54 24616c6c _in_place$LT$all
-  0x00016110 6f632e2e 626f7272 6f772e2e 436f7724 oc..borrow..Cow$
-  0x00016120 4c542473 74722447 54242447 54243137 LT$str$GT$$GT$17
-  0x00016130 68623231 63383135 34653538 66306663 hb21c8154e58f0fc
-  0x00016140 36452e6c 6c766d2e 31333836 31383532 6E.llvm.13861852
-  0x00016150 37313133 39303237 34373600 5f5a4e34 71139027476._ZN4
-  0x00016160 636f7265 3970616e 69636b69 6e673139 core9panicking19
-  0x00016170 61737365 72745f66 61696c65 645f696e assert_failed_in
-  0x00016180 6e657231 37686166 39383136 32323762 ner17haf9816227b
-  0x00016190 32306236 66324500 5f5a4e39 315f244c 20b6f2E._ZN91_$L
-  0x000161a0 54247374 642e2e70 616e6963 6b696e67 T$std..panicking
-  0x000161b0 2e2e6265 67696e5f 70616e69 632e2e50 ..begin_panic..P
-  0x000161c0 616e6963 5061796c 6f616424 4c542441 anicPayload$LT$A
-  0x000161d0 24475424 24753230 24617324 75323024 $GT$$u20$as$u20$
-  0x000161e0 636f7265 2e2e7061 6e69632e 2e426f78 core..panic..Box
-  0x000161f0 4d655570 24475424 3874616b 655f626f MeUp$GT$8take_bo
-  0x00016200 78313768 39366631 65373333 37373563 x17h96f1e733775c
-  0x00016210 36663731 45005f5a 4e337374 64397061 6f71E._ZN3std9pa
-  0x00016220 6e69636b 696e6731 3170616e 69635f63 nicking11panic_c
-  0x00016230 6f756e74 31376973 5f7a6572 6f5f736c ount17is_zero_sl
-  0x00016240 6f775f70 61746831 37683163 31393136 ow_path17h1c1916
-  0x00016250 39366434 35623438 33624500 5f5a4e34 96d45b483bE._ZN4
-  0x00016260 636f7265 33666d74 336e756d 33696d70 core3fmt3num3imp
-  0x00016270 35325f24 4c542469 6d706c24 75323024 52_$LT$impl$u20$
-  0x00016280 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x00016290 61792475 32302466 6f722475 32302469 ay$u20$for$u20$i
-  0x000162a0 33322447 54243366 6d743137 68626437 32$GT$3fmt17hbd7
-  0x000162b0 39346133 33666665 62376162 6345005f 94a33ffeb7abcE._
-  0x000162c0 5a4e3470 796f3333 65727239 6572725f ZN4pyo33err9err_
-  0x000162d0 73746174 65313062 6f786564 5f617267 state10boxed_arg
-  0x000162e0 73313768 64646165 38343136 62303337 s17hddae8416b037
-  0x000162f0 64373035 45005f5a 4e37345f 244c5424 d705E._ZN74_$LT$
-  0x00016300 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x00016310 2e2e5079 4b657962 6f617264 496e7465 ..PyKeyboardInte
-  0x00016320 72727570 74247532 30246173 24753230 rrupt$u20$as$u20
-  0x00016330 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x00016340 67244754 2433666d 74313768 33636436 g$GT$3fmt17h3cd6
-  0x00016350 30633234 35343535 63663666 45005f5a 0c245455cf6fE._Z
-  0x00016360 4e39315f 244c5424 7374642e 2e737973 N91_$LT$std..sys
-  0x00016370 5f636f6d 6d6f6e2e 2e626163 6b747261 _common..backtra
-  0x00016380 63652e2e 5f707269 6e742e2e 44697370 ce.._print..Disp
-  0x00016390 6c617942 61636b74 72616365 24753230 layBacktrace$u20
-  0x000163a0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
-  0x000163b0 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
-  0x000163c0 6d743137 68353737 39643762 66376637 mt17h5779d7bf7f7
-  0x000163d0 30636230 6345005f 5f727573 745f7061 0cb0cE.__rust_pa
-  0x000163e0 6e69635f 636c6561 6e757000 616e6f6e nic_cleanup.anon
-  0x000163f0 2e333437 64323634 65333465 62336130 .347d264e34eb3a0
-  0x00016400 63373462 65356138 39663839 35616337 c74be5a89f895ac7
-  0x00016410 652e3633 2e6c6c76 6d2e3137 36393537 e.63.llvm.176957
-  0x00016420 36323334 31373831 34353330 3132005f 62341781453012._
-  0x00016430 5a4e3634 5f244c54 24737464 2e2e7379 ZN64_$LT$std..sy
-  0x00016440 732e2e75 6e69782e 2e737464 696f2e2e s..unix..stdio..
-  0x00016450 5374646f 75742475 32302461 73247532 Stdout$u20$as$u2
-  0x00016460 30247374 642e2e69 6f2e2e57 72697465 0$std..io..Write
-  0x00016470 24475424 35666c75 73683137 68353432 $GT$5flush17h542
-  0x00016480 37333865 66376237 63313135 3745005f 738ef7b7c1157E._
-  0x00016490 5a4e3470 796f3333 65727235 50794572 ZN4pyo33err5PyEr
-  0x000164a0 72313066 726f6d5f 76616c75 65313768 r10from_value17h
-  0x000164b0 37636564 36653739 39656462 38623836 7ced6e799edb8b86
-  0x000164c0 45005f5a 4e34636f 72653366 6d743946 E._ZN4core3fmt9F
-  0x000164d0 6f726d61 74746572 32356465 6275675f ormatter25debug_
-  0x000164e0 7475706c 655f6669 656c6431 5f66696e tuple_field1_fin
-  0x000164f0 69736831 37683637 61343636 39633330 ish17h67a4669c30
-  0x00016500 32343533 34344500 5f5a4e34 70796f33 245344E._ZN4pyo3
-  0x00016510 3131636f 6e766572 73696f6e 73337374 11conversions3st
-  0x00016520 64367374 72696e67 3133335f 244c5424 d6string133_$LT$
-  0x00016530 696d706c 24753230 2470796f 332e2e63 impl$u20$pyo3..c
-  0x00016540 6f6e7665 7273696f 6e2e2e49 6e746f50 onversion..IntoP
-  0x00016550 79244c54 2470796f 332e2e69 6e737461 y$LT$pyo3..insta
-  0x00016560 6e63652e 2e507924 4c542470 796f332e nce..Py$LT$pyo3.
-  0x00016570 2e747970 65732e2e 616e792e 2e507941 .types..any..PyA
-  0x00016580 6e792447 54242447 54242475 32302466 ny$GT$$GT$$u20$f
-  0x00016590 6f722475 32302461 6c6c6f63 2e2e7374 or$u20$alloc..st
-  0x000165a0 72696e67 2e2e5374 72696e67 24475424 ring..String$GT$
-  0x000165b0 37696e74 6f5f7079 31376834 31616238 7into_py17h41ab8
-  0x000165c0 37396339 36393866 32306545 005f5a4e 79c9698f20eE._ZN
-  0x000165d0 37325f24 4c542470 796f332e 2e657863 72_$LT$pyo3..exc
-  0x000165e0 65707469 6f6e732e 2e507946 696c6545 eptions..PyFileE
-  0x000165f0 78697374 73457272 6f722475 32302461 xistsError$u20$a
-  0x00016600 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00016610 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x00016620 68653261 35303364 61316539 65333965 he2a503da1e9e39e
-  0x00016630 3145005f 5a4e3463 6f726533 70747239 1E._ZN4core3ptr9
-  0x00016640 3764726f 705f696e 5f706c61 6365244c 7drop_in_place$L
-  0x00016650 54247079 6f332e2e 6572722e 2e657272 T$pyo3..err..err
-  0x00016660 5f737461 74652e2e 626f7865 645f6172 _state..boxed_ar
-  0x00016670 6773244c 54242452 46247374 72244754 gs$LT$$RF$str$GT
-  0x00016680 242e2e24 75376224 24753762 24636c6f $..$u7b$$u7b$clo
-  0x00016690 73757265 24753764 24247537 64242447 sure$u7d$$u7d$$G
-  0x000166a0 54243137 68633164 39333235 34393562 T$17hc1d9325495b
-  0x000166b0 34613937 31452e6c 6c766d2e 33373535 4a971E.llvm.3755
-  0x000166c0 34303432 31313432 32323930 34303600 404211422290406.
-  0x000166d0 616e6f6e 2e623961 30343836 63303061 anon.b9a0486c00a
-  0x000166e0 34313732 62376231 61633532 62333135 4172b7b1ac52b315
-  0x000166f0 61613461 332e3531 2e6c6c76 6d2e3133 aa4a3.51.llvm.13
-  0x00016700 32333838 39333433 32323030 36393232 2388934322006922
-  0x00016710 3236005f 5a4e3638 5f244c54 2470796f 26._ZN68_$LT$pyo
-  0x00016720 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00016730 79547970 65457272 6f722475 32302461 yTypeError$u20$a
-  0x00016740 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00016750 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
-  0x00016760 31376862 30616161 65303831 66633632 17hb0aaae081fc62
-  0x00016770 63626445 00616e6f 6e2e3965 31313465 cbdE.anon.9e114e
-  0x00016780 64353031 30643632 35336264 32363131 d5010d6253bd2611
-  0x00016790 32393437 33636431 38382e35 2e6c6c76 29473cd188.5.llv
-  0x000167a0 6d2e3833 36343733 35313732 37303334 m.83647351727034
-  0x000167b0 37363335 34005f5a 4e34636f 72653366 76354._ZN4core3f
-  0x000167c0 66693563 5f737472 34435374 7236746f fi5c_str4CStr6to
-  0x000167d0 5f737472 31376837 35623762 61376664 _str17h75b7ba7fd
-  0x000167e0 63653432 36363045 005f5a4e 34636f72 ce42660E._ZN4cor
-  0x000167f0 65337074 72313232 64726f70 5f696e5f e3ptr122drop_in_
-  0x00016800 706c6163 65244c54 2470796f 332e2e65 place$LT$pyo3..e
-  0x00016810 72722e2e 6572725f 73746174 652e2e62 rr..err_state..b
-  0x00016820 6f786564 5f617267 73244c54 24244c50 oxed_args$LT$$LP
-  0x00016830 24616c6c 6f632e2e 73747269 6e672e2e $alloc..string..
-  0x00016840 53747269 6e672443 24245250 24244754 String$C$$RP$$GT
-  0x00016850 242e2e24 75376224 24753762 24636c6f $..$u7b$$u7b$clo
-  0x00016860 73757265 24753764 24247537 64242447 sure$u7d$$u7d$$G
-  0x00016870 54243137 68353334 38646132 35336335 T$17h5348da253c5
-  0x00016880 64336439 32452e6c 6c766d2e 33313630 d3d92E.llvm.3160
-  0x00016890 39303732 38313838 30373831 31323300 907281880781123.
-  0x000168a0 616e6f6e 2e623961 30343836 63303061 anon.b9a0486c00a
-  0x000168b0 34313732 62376231 61633532 62333135 4172b7b1ac52b315
-  0x000168c0 61613461 332e3133 2e6c6c76 6d2e3133 aa4a3.13.llvm.13
-  0x000168d0 32333838 39333433 32323030 36393232 2388934322006922
-  0x000168e0 3236005f 5a4e3730 5f244c54 2470796f 26._ZN70_$LT$pyo
-  0x000168f0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x00016900 79467574 75726557 61726e69 6e672475 yFutureWarning$u
-  0x00016910 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x00016920 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
-  0x00016930 6d743137 68623935 30336361 35636431 mt17hb9503ca5cd1
-  0x00016940 63626437 3945005f 5a4e3731 5f244c54 cbd79E._ZN71_$LT
-  0x00016950 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00016960 732e2e50 79417373 65727469 6f6e4572 s..PyAssertionEr
-  0x00016970 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
-  0x00016980 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
-  0x00016990 47542433 666d7431 37683939 35626638 GT$3fmt17h995bf8
-  0x000169a0 62613632 32326530 37624500 5f5a4e37 ba6222e07bE._ZN7
-  0x000169b0 335f244c 54247079 6f332e2e 65786365 3_$LT$pyo3..exce
-  0x000169c0 7074696f 6e732e2e 50794174 74726962 ptions..PyAttrib
-  0x000169d0 75746545 72726f72 24753230 24617324 uteError$u20$as$
-  0x000169e0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x000169f0 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
-  0x00016a00 68323166 36383431 38643064 65346331 h21f68418d0de4c1
-  0x00016a10 3745005f 5a4e3463 6f726533 73747235 7E._ZN4core3str5
-  0x00016a20 6c6f7373 79313055 74663843 68756e6b lossy10Utf8Chunk
-  0x00016a30 73336e65 77313768 62333439 30616234 s3new17hb3490ab4
-  0x00016a40 66316635 63613936 45005f5a 4e34636f f1f5ca96E._ZN4co
-  0x00016a50 72653373 74723139 736c6963 655f6572 re3str19slice_er
-  0x00016a60 726f725f 6661696c 5f727431 37686464 ror_fail_rt17hdd
-  0x00016a70 61343962 65643464 37313631 62384500 a49bed4d7161b8E.
-  0x00016a80 5f5a4e34 70796f33 35747970 65733766 _ZN4pyo35types7f
-  0x00016a90 6c6f6174 6f623131 355f244c 5424696d loatob115_$LT$im
-  0x00016aa0 706c2475 32302470 796f332e 2e636f6e pl$u20$pyo3..con
-  0x00016ab0 76657273 696f6e2e 2e496e74 6f507924 version..IntoPy$
-  0x00016ac0 4c542470 796f332e 2e696e73 74616e63 LT$pyo3..instanc
-  0x00016ad0 652e2e50 79244c54 2470796f 332e2e74 e..Py$LT$pyo3..t
-  0x00016ae0 79706573 2e2e616e 792e2e50 79416e79 ypes..any..PyAny
-  0x00016af0 24475424 24475424 24753230 24666f72 $GT$$GT$$u20$for
-  0x00016b00 24753230 24663332 24475424 37696e74 $u20$f32$GT$7int
-  0x00016b10 6f5f7079 31376830 65396230 30396361 o_py17h0e9b009ca
-  0x00016b20 63333630 64646645 005f5a4e 37395f24 c360ddfE._ZN79_$
-  0x00016b30 4c542470 796f332e 2e747970 65732e2e LT$pyo3..types..
-  0x00016b40 73747269 6e672e2e 50795374 72696e67 string..PyString
-  0x00016b50 24753230 24617324 75323024 70796f33 $u20$as$u20$pyo3
-  0x00016b60 2e2e7479 70655f6f 626a6563 742e2e50 ..type_object..P
-  0x00016b70 79547970 65496e66 6f244754 24313069 yTypeInfo$GT$10i
-  0x00016b80 735f7479 70655f6f 66313768 31633665 s_type_of17h1c6e
-  0x00016b90 34643135 61313461 32653234 45005f5a 4d15a14a2e24E._Z
-  0x00016ba0 4e347079 6f333574 79706573 35747570 N4pyo35types5tup
-  0x00016bb0 6c653750 79547570 6c653469 74657231 le7PyTuple4iter1
-  0x00016bc0 37686366 35336336 33353433 63333264 7hcf53c63543c32d
-  0x00016bd0 63634500 616e6f6e 2e396531 31346564 ccE.anon.9e114ed
-  0x00016be0 35303130 64363235 33626432 36313132 5010d6253bd26112
-  0x00016bf0 39343733 63643138 382e302e 6c6c766d 9473cd188.0.llvm
-  0x00016c00 2e383336 34373335 31373237 30333437 .836473517270347
-  0x00016c10 36333534 005f5a4e 3567696d 6c693472 6354._ZN5gimli4r
-  0x00016c20 65616434 6c696e65 374c696e 65526f77 ead4line7LineRow
-  0x00016c30 31386170 706c795f 6c696e65 5f616476 18apply_line_adv
-  0x00016c40 616e6365 31376866 32313832 33646663 ance17hf21823dfc
-  0x00016c50 61373961 63383645 005f5a4e 34636f72 a79ac86E._ZN4cor
-  0x00016c60 6533666d 7439466f 726d6174 74657232 e3fmt9Formatter2
-  0x00016c70 36646562 75675f73 74727563 745f6669 6debug_struct_fi
-  0x00016c80 656c6431 5f66696e 69736831 37686537 eld1_finish17he7
-  0x00016c90 39336463 61343639 38316535 31614500 93dca46981e51aE.
-  0x00016ca0 5f5a4e34 70796f33 33657272 35507945 _ZN4pyo33err5PyE
-  0x00016cb0 72723135 6d616b65 5f6e6f72 6d616c69 rr15make_normali
-  0x00016cc0 7a656431 37683936 65646461 62623732 zed17h96eddabb72
-  0x00016cd0 32623365 63354500 5f5a4e35 67696d6c 2b3ec5E._ZN5giml
-  0x00016ce0 69347265 61643475 6e697432 30616c6c i4read4unit20all
-  0x00016cf0 6f775f73 65637469 6f6e5f6f 66667365 ow_section_offse
-  0x00016d00 74313768 63326262 65666439 35343939 t17hc2bbefd95499
-  0x00016d10 66666539 45005f5a 4e347079 6f333367 ffe9E._ZN4pyo33g
-  0x00016d20 696c3133 4f574e45 445f4f42 4a454354 il13OWNED_OBJECT
-  0x00016d30 53375f5f 67657469 74313768 39646136 S7__getit17h9da6
-  0x00016d40 35333963 31613066 37306663 452e6c6c 539c1a0f70fcE.ll
-  0x00016d50 766d2e31 33323338 38393334 33323230 vm.1323889343220
-  0x00016d60 30363932 32323600 5f5a4e34 636f7265 0692226._ZN4core
-  0x00016d70 33666d74 35777269 74653137 68356134 3fmt5write17h5a4
-  0x00016d80 62616166 66316263 64336562 35450061 baaff1bcd3eb5E.a
-  0x00016d90 6e6f6e2e 35313035 62646437 39663233 non.5105bdd79f23
-  0x00016da0 62313137 31663338 37343266 65616163 b1171f38742feaac
-  0x00016db0 35643137 2e33332e 6c6c766d 2e333136 5d17.33.llvm.316
-  0x00016dc0 30393037 32383138 38303738 31313233 0907281880781123
-  0x00016dd0 005f5a4e 39315f24 4c542473 74642e2e ._ZN91_$LT$std..
-  0x00016de0 70616e69 636b696e 672e2e62 6567696e panicking..begin
-  0x00016df0 5f70616e 69632e2e 50616e69 63506179 _panic..PanicPay
-  0x00016e00 6c6f6164 244c5424 41244754 24247532 load$LT$A$GT$$u2
-  0x00016e10 30246173 24753230 24636f72 652e2e70 0$as$u20$core..p
-  0x00016e20 616e6963 2e2e426f 784d6555 70244754 anic..BoxMeUp$GT
-  0x00016e30 24387461 6b655f62 6f783137 68643063 $8take_box17hd0c
-  0x00016e40 39393538 35373639 33663337 6145005f 995857693f37aE._
-  0x00016e50 5a4e3731 5f244c54 2470796f 332e2e69 ZN71_$LT$pyo3..i
-  0x00016e60 6d706c5f 2e2e7061 6e69632e 2e50616e mpl_..panic..Pan
-  0x00016e70 69635472 61702475 32302461 73247532 icTrap$u20$as$u2
-  0x00016e80 3024636f 72652e2e 6f70732e 2e64726f 0$core..ops..dro
-  0x00016e90 702e2e44 726f7024 47542434 64726f70 p..Drop$GT$4drop
-  0x00016ea0 31376834 35613364 36343235 31383636 17h45a3d64251866
-  0x00016eb0 36313145 005f5a4e 37325f24 4c542470 611E._ZN72_$LT$p
-  0x00016ec0 796f332e 2e747970 65732e2e 74726163 yo3..types..trac
-  0x00016ed0 65626163 6b2e2e50 79547261 63656261 eback..PyTraceba
-  0x00016ee0 636b2475 32302461 73247532 3024636f ck$u20$as$u20$co
-  0x00016ef0 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
-  0x00016f00 54243366 6d743137 68313066 65303636 T$3fmt17h10fe066
-  0x00016f10 33663666 36353734 3945005f 5a4e3131 3f6f65749E._ZN11
-  0x00016f20 6d696e69 7a5f6f78 69646537 696e666c miniz_oxide7infl
-  0x00016f30 61746534 636f7265 31306465 636f6d70 ate4core10decomp
-  0x00016f40 72657373 31376837 39353534 64323166 ress17h79554d21f
-  0x00016f50 32356537 39313245 005f5a4e 37305f24 25e7912E._ZN70_$
-  0x00016f60 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x00016f70 6f6e732e 2e507947 656e6572 61746f72 ons..PyGenerator
-  0x00016f80 45786974 24753230 24617324 75323024 Exit$u20$as$u20$
-  0x00016f90 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00016fa0 24475424 33666d74 31376831 33336432 $GT$3fmt17h133d2
-  0x00016fb0 36363436 63356539 30383545 005f5a4e 6646c5e9085E._ZN
-  0x00016fc0 36345f24 4c542472 75737463 5f64656d 64_$LT$rustc_dem
-  0x00016fd0 616e676c 652e2e76 302e2e49 64656e74 angle..v0..Ident
-  0x00016fe0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00016ff0 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x00017000 54243366 6d743137 68386538 33323666 T$3fmt17h8e8326f
-  0x00017010 61373339 65646335 3445005f 5a4e3463 a739edc54E._ZN4c
-  0x00017020 6f726533 666d7435 57726974 65397772 ore3fmt5Write9wr
-  0x00017030 6974655f 666d7431 37683263 63653531 ite_fmt17h2cce51
-  0x00017040 31316137 31613665 62614500 5f5a4e39 11a71a6ebaE._ZN9
-  0x00017050 325f244c 54247079 6f332e2e 6572722e 2_$LT$pyo3..err.
-  0x00017060 2e507944 6f776e63 61737445 72726f72 .PyDowncastError
-  0x00017070 41726775 6d656e74 73247532 30246173 Arguments$u20$as
-  0x00017080 24753230 2470796f 332e2e65 72722e2e $u20$pyo3..err..
-  0x00017090 6572725f 73746174 652e2e50 79457272 err_state..PyErr
-  0x000170a0 41726775 6d656e74 73244754 24396172 Arguments$GT$9ar
-  0x000170b0 67756d65 6e747331 37686434 33326262 guments17hd432bb
-  0x000170c0 66363661 32353231 63314500 616e6f6e f66a2521c1E.anon
-  0x000170d0 2e353130 35626464 37396632 33623131 .5105bdd79f23b11
-  0x000170e0 37316633 38373432 66656161 63356431 71f38742feaac5d1
-  0x000170f0 372e3139 2e6c6c76 6d2e3331 36303930 7.19.llvm.316090
-  0x00017100 37323831 38383037 38313132 33005f5a 7281880781123._Z
-  0x00017110 4e35616c 6c6f6335 616c6c6f 6338626f N5alloc5alloc8bo
-  0x00017120 785f6672 65653137 68366436 30646532 x_free17h6d60de2
-  0x00017130 65386537 30376264 64452e6c 6c766d2e e8e707bddE.llvm.
-  0x00017140 31383335 36373530 34383536 31343531 1835675048561451
-  0x00017150 33313239 005f5a4e 31317061 726b696e 3129._ZN11parkin
-  0x00017160 675f6c6f 74346f6e 6365344f 6e636531 g_lot4once4Once1
-  0x00017170 3463616c 6c5f6f6e 63655f73 6c6f7731 4call_once_slow1
-  0x00017180 37683539 39303562 65363366 33383836 7h59905be63f3886
-  0x00017190 31634500 616e6f6e 2e333437 64323634 1cE.anon.347d264
-  0x000171a0 65333465 62336130 63373462 65356138 e34eb3a0c74be5a8
-  0x000171b0 39663839 35616337 652e3133 2e6c6c76 9f895ac7e.13.llv
-  0x000171c0 6d2e3137 36393537 36323334 31373831 m.17695762341781
-  0x000171d0 34353330 31320061 6e6f6e2e 39376164 453012.anon.97ad
-  0x000171e0 39333163 35346338 38356361 39366466 931c54c885ca96df
-  0x000171f0 64373265 66313061 62303338 2e362e6c d72ef10ab038.6.l
-  0x00017200 6c766d2e 33303431 33393339 35383536 lvm.304139395856
-  0x00017210 39393734 33343900 5f5a4e34 636f7265 9974349._ZN4core
-  0x00017220 33666d74 336e756d 35335f24 4c542469 3fmt3num53_$LT$i
-  0x00017230 6d706c24 75323024 636f7265 2e2e666d mpl$u20$core..fm
-  0x00017240 742e2e4c 6f776572 48657824 75323024 t..LowerHex$u20$
-  0x00017250 666f7224 75323024 75363424 47542433 for$u20$u64$GT$3
-  0x00017260 666d7431 37686364 61376439 62313134 fmt17hcda7d9b114
-  0x00017270 38303135 37634500 5f5a4e37 345f244c 80157cE._ZN74_$L
-  0x00017280 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
-  0x00017290 6e732e2e 6173796e 63696f2e 2e517565 ns..asyncio..Que
-  0x000172a0 7565456d 70747924 75323024 61732475 ueEmpty$u20$as$u
-  0x000172b0 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
-  0x000172c0 62756724 47542433 666d7431 37683735 bug$GT$3fmt17h75
-  0x000172d0 32373236 64386566 32326130 33324500 2726d8ef22a032E.
-  0x000172e0 5f5a4e33 73746433 73797334 756e6978 _ZN3std3sys4unix
-  0x000172f0 356c6f63 6b733131 66757465 785f6d75 5locks11futex_mu
-  0x00017300 74657835 4d757465 7831346c 6f636b5f tex5Mutex14lock_
-  0x00017310 636f6e74 656e6465 64313768 30343334 contended17h0434
-  0x00017320 61646466 63363362 61383062 45005f5a addfc63ba80bE._Z
-  0x00017330 4e36355f 244c5424 70796f33 2e2e6578 N65_$LT$pyo3..ex
-  0x00017340 63657074 696f6e73 2e2e5079 454f4645 ceptions..PyEOFE
-  0x00017350 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x00017360 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
-  0x00017370 24475424 33666d74 31376838 35323861 $GT$3fmt17h8528a
-  0x00017380 39393764 36393933 66326545 005f5a4e 997d6993f2eE._ZN
-  0x00017390 34636f72 65336666 6935635f 73747234 4core3ffi5c_str4
-  0x000173a0 43537472 3866726f 6d5f7074 72397374 CStr8from_ptr9st
-  0x000173b0 726c656e 5f727431 37686261 35353065 rlen_rt17hba550e
-  0x000173c0 35616336 36613361 61384500 5f5a4e39 5ac66a3aa8E._ZN9
-  0x000173d0 315f244c 54247374 642e2e70 616e6963 1_$LT$std..panic
-  0x000173e0 6b696e67 2e2e7275 73745f70 616e6963 king..rust_panic
-  0x000173f0 5f776974 686f7574 5f686f6f 6b2e2e52 _without_hook..R
-  0x00017400 65777261 70426f78 24753230 24617324 ewrapBox$u20$as$
-  0x00017410 75323024 636f7265 2e2e7061 6e69632e u20$core..panic.
-  0x00017420 2e426f78 4d655570 24475424 3874616b .BoxMeUp$GT$8tak
-  0x00017430 655f626f 78313768 37653339 65643930 e_box17h7e39ed90
-  0x00017440 61366238 65313964 45005f5a 4e35616c a6b8e19dE._ZN5al
-  0x00017450 6c6f6335 616c6c6f 6338626f 785f6672 loc5alloc8box_fr
-  0x00017460 65653137 68366436 30646532 65386537 ee17h6d60de2e8e7
-  0x00017470 30376264 64452e6c 6c766d2e 33313630 07bddE.llvm.3160
-  0x00017480 39303732 38313838 30373831 31323300 907281880781123.
-  0x00017490 5f5a4e36 345f244c 54247079 6f332e2e _ZN64_$LT$pyo3..
-  0x000174a0 65786365 7074696f 6e732e2e 50795761 exceptions..PyWa
-  0x000174b0 726e696e 67247532 30246173 24753230 rning$u20$as$u20
-  0x000174c0 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x000174d0 67244754 2433666d 74313768 34373033 g$GT$3fmt17h4703
-  0x000174e0 35373165 38643763 65633566 45005f5a 571e8d7cec5fE._Z
-  0x000174f0 4e337374 6433656e 76313163 75727265 N3std3env11curre
-  0x00017500 6e745f64 69723137 68356662 32656537 nt_dir17h5fb2ee7
-  0x00017510 66393065 36623636 3945005f 5a4e3732 f90e6b669E._ZN72
-  0x00017520 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
-  0x00017530 74696f6e 732e2e50 79496d70 6f727457 tions..PyImportW
-  0x00017540 61726e69 6e672475 32302461 73247532 arning$u20$as$u2
-  0x00017550 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
-  0x00017560 706c6179 24475424 33666d74 31376831 play$GT$3fmt17h1
-  0x00017570 39656333 61366234 62636138 64623845 9ec3a6b4bca8db8E
-  0x00017580 005f5a4e 33737464 3970616e 69636b69 ._ZN3std9panicki
-  0x00017590 6e673374 72793763 6c65616e 75703137 ng3try7cleanup17
-  0x000175a0 68306136 34356435 34393934 32636433 h0a645d549942cd3
-  0x000175b0 3145005f 5a4e3561 6c6c6f63 37726177 1E._ZN5alloc7raw
-  0x000175c0 5f766563 31316669 6e697368 5f67726f _vec11finish_gro
-  0x000175d0 77313768 37643239 66383834 62316230 w17h7d29f884b1b0
-  0x000175e0 66383132 452e6c6c 766d2e35 37363737 f812E.llvm.57677
-  0x000175f0 39303736 34373638 30373130 3334005f 90764768071034._
-  0x00017600 5a4e3373 74643365 6e763131 63757272 ZN3std3env11curr
-  0x00017610 656e745f 65786531 37686635 66613634 ent_exe17hf5fa64
-  0x00017620 37336339 65383931 66654500 5f5a4e34 73c9e891feE._ZN4
-  0x00017630 636f7265 33666d74 336e756d 35355f24 core3fmt3num55_$
-  0x00017640 4c542469 6d706c24 75323024 636f7265 LT$impl$u20$core
-  0x00017650 2e2e666d 742e2e4c 6f776572 48657824 ..fmt..LowerHex$
-  0x00017660 75323024 666f7224 75323024 6973697a u20$for$u20$isiz
-  0x00017670 65244754 2433666d 74313768 38626434 e$GT$3fmt17h8bd4
-  0x00017680 63633133 63353231 65633934 45005f5a cc13c521ec94E._Z
-  0x00017690 4e37345f 244c5424 70796f33 2e2e6578 N74_$LT$pyo3..ex
-  0x000176a0 63657074 696f6e73 2e2e5079 5265736f ceptions..PyReso
-  0x000176b0 75726365 5761726e 696e6724 75323024 urceWarning$u20$
-  0x000176c0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x000176d0 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
-  0x000176e0 74313768 61303861 30386334 65386433 t17ha08a08c4e8d3
-  0x000176f0 38383235 45005f5a 4e37345f 244c5424 8825E._ZN74_$LT$
-  0x00017700 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x00017710 2e2e5079 4368696c 6450726f 63657373 ..PyChildProcess
-  0x00017720 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x00017730 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
-  0x00017740 67244754 2433666d 74313768 31356136 g$GT$3fmt17h15a6
-  0x00017750 30613761 30653037 63636635 45005f5a 0a7a0e07ccf5E._Z
-  0x00017760 4e37325f 244c5424 70796f33 2e2e6578 N72_$LT$pyo3..ex
-  0x00017770 63657074 696f6e73 2e2e5079 4f766572 ceptions..PyOver
-  0x00017780 666c6f77 4572726f 72247532 30246173 flowError$u20$as
-  0x00017790 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x000177a0 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x000177b0 37683134 63306538 35336130 35356261 7h14c0e853a055ba
-  0x000177c0 35634500 616e6f6e 2e376239 34366165 5cE.anon.7b946ae
-  0x000177d0 31643361 36363637 39376532 64623166 1d3a666797e2db1f
-  0x000177e0 33366534 63643665 372e372e 6c6c766d 36e4cd6e7.7.llvm
-  0x000177f0 2e313833 35363735 30343835 36313435 .183567504856145
-  0x00017800 31333132 3900616e 6f6e2e65 39313336 13129.anon.e9136
-  0x00017810 64346363 32663262 66373333 64353932 d4cc2f2bf733d592
-  0x00017820 62356466 38383935 3230372e 342e6c6c b5df8895207.4.ll
-  0x00017830 766d2e31 37333638 37353432 34303436 vm.1736875424046
-  0x00017840 38303333 35363000 5f5a4e35 67696d6c 8033560._ZN5giml
-  0x00017850 69347265 61643661 62627265 76313041 i4read6abbrev10A
-  0x00017860 74747269 62757465 73347075 73683137 ttributes4push17
-  0x00017870 68383162 35343861 32653261 65623836 h81b548a2e2aeb86
-  0x00017880 6445005f 5a4e3732 5f244c54 2470796f dE._ZN72_$LT$pyo
-  0x00017890 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
-  0x000178a0 7947656e 65726174 6f724578 69742475 yGeneratorExit$u
-  0x000178b0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
-  0x000178c0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
-  0x000178d0 33666d74 31376837 34613333 30613665 3fmt17h74a330a6e
-  0x000178e0 66323930 31323645 00616e6f 6e2e6539 f290126E.anon.e9
-  0x000178f0 65623233 37636635 30613433 62363564 eb237cf50a43b65d
-  0x00017900 36333662 30663437 37306230 34652e32 636b0f4770b04e.2
-  0x00017910 332e6c6c 766d2e31 33383631 38353237 3.llvm.138618527
-  0x00017920 31313339 30323734 3736005f 5a4e3636 1139027476._ZN66
-  0x00017930 5f244c54 24636f72 652e2e6f 7074696f _$LT$core..optio
-  0x00017940 6e2e2e4f 7074696f 6e244c54 24542447 n..Option$LT$T$G
-  0x00017950 54242475 32302461 73247532 3024636f T$$u20$as$u20$co
-  0x00017960 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
-  0x00017970 54243366 6d743137 68303962 66323131 T$3fmt17h09bf211
-  0x00017980 30626462 61386134 3445005f 5a4e3638 0bdba8a44E._ZN68
-  0x00017990 5f244c54 24245246 24247535 62247538 _$LT$$RF$$u5b$u8
-  0x000179a0 24753564 24247532 30246173 24753230 $u5d$$u20$as$u20
-  0x000179b0 246f626a 6563742e 2e726561 642e2e72 $object..read..r
-  0x000179c0 6561645f 7265662e 2e526561 64526566 ead_ref..ReadRef
-  0x000179d0 24475424 31337265 61645f62 79746573 $GT$13read_bytes
-  0x000179e0 5f617431 37686633 61356263 31366534 _at17hf3a5bc16e4
-  0x000179f0 37613236 65364500 5f5a4e34 70796f33 7a26e6E._ZN4pyo3
-  0x00017a00 35747970 65733766 6c6f6174 6f623634 5types7floatob64
-  0x00017a10 5f244c54 24696d70 6c247532 30247079 _$LT$impl$u20$py
-  0x00017a20 6f332e2e 636f6e76 65727369 6f6e2e2e o3..conversion..
-  0x00017a30 46726f6d 50794f62 6a656374 24753230 FromPyObject$u20
-  0x00017a40 24666f72 24753230 24663332 24475424 $for$u20$f32$GT$
-  0x00017a50 37657874 72616374 31376866 38373366 7extract17hf873f
-  0x00017a60 33663930 34363732 62313045 005f5a4e 3f904672b10E._ZN
-  0x00017a70 36385f24 4c542470 796f332e 2e657863 68_$LT$pyo3..exc
-  0x00017a80 65707469 6f6e732e 2e50794e 616d6545 eptions..PyNameE
-  0x00017a90 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x00017aa0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x00017ab0 61792447 54243366 6d743137 68383266 ay$GT$3fmt17h82f
-  0x00017ac0 39623634 35336333 63643462 3745005f 9b6453c3cd4b7E._
-  0x00017ad0 5a4e3638 5f244c54 2470796f 332e2e65 ZN68_$LT$pyo3..e
-  0x00017ae0 78636570 74696f6e 732e2e50 794d656d xceptions..PyMem
-  0x00017af0 6f727945 72726f72 24753230 24617324 oryError$u20$as$
-  0x00017b00 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00017b10 65627567 24475424 33666d74 31376835 ebug$GT$3fmt17h5
-  0x00017b20 39633436 33623337 66346366 34386145 9c463b37f4cf48aE
-  0x00017b30 005f5a4e 36335f24 4c542472 75737463 ._ZN63_$LT$rustc
-  0x00017b40 5f64656d 616e676c 652e2e44 656d616e _demangle..Deman
-  0x00017b50 676c6524 75323024 61732475 32302463 gle$u20$as$u20$c
-  0x00017b60 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
-  0x00017b70 79244754 2433666d 74313768 39373939 y$GT$3fmt17h9799
-  0x00017b80 64333531 38633632 31636539 45005f5a d3518c621ce9E._Z
-  0x00017b90 4e34636f 72653373 74723674 72616974 N4core3str6trait
-  0x00017ba0 73323373 74725f69 6e646578 5f6f7665 s23str_index_ove
-  0x00017bb0 72666c6f 775f6661 696c3137 68373632 rflow_fail17h762
-  0x00017bc0 33336339 39323538 64363935 3745005f 33c99258d6957E._
-  0x00017bd0 5a4e3470 796f3333 65727235 50794572 ZN4pyo33err5PyEr
-  0x00017be0 72397365 745f6361 75736531 37683330 r9set_cause17h30
-  0x00017bf0 35383065 66376164 64646566 30644500 580ef7adddef0dE.
-  0x00017c00 5f5a4e33 73746434 70617468 3130436f _ZN3std4path10Co
-  0x00017c10 6d706f6e 656e7473 3761735f 70617468 mponents7as_path
-  0x00017c20 31376833 63633365 36383865 33313037 17h3cc3e688e3107
-  0x00017c30 37303445 005f5a4e 36335f24 4c542463 704E._ZN63_$LT$c
-  0x00017c40 6f72652e 2e63656c 6c2e2e42 6f72726f ore..cell..Borro
-  0x00017c50 774d7574 4572726f 72247532 30246173 wMutError$u20$as
-  0x00017c60 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x00017c70 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
-  0x00017c80 38383438 62626137 62383964 33663861 8848bba7b89d3f8a
-  0x00017c90 45005f5a 4e34636f 72653366 6d74336e E._ZN4core3fmt3n
-  0x00017ca0 756d3533 5f244c54 24696d70 6c247532 um53_$LT$impl$u2
-  0x00017cb0 3024636f 72652e2e 666d742e 2e557070 0$core..fmt..Upp
-  0x00017cc0 65724865 78247532 3024666f 72247532 erHex$u20$for$u2
-  0x00017cd0 30246933 32244754 2433666d 74313768 0$i32$GT$3fmt17h
-  0x00017ce0 66613831 64316435 61323739 34623764 fa81d1d5a2794b7d
-  0x00017cf0 45005f5a 4e34636f 72653370 74723132 E._ZN4core3ptr12
-  0x00017d00 3564726f 705f696e 5f706c61 6365244c 5drop_in_place$L
-  0x00017d10 54247079 6f332e2e 6572722e 2e657272 T$pyo3..err..err
-  0x00017d20 5f737461 74652e2e 626f7865 645f6172 _state..boxed_ar
-  0x00017d30 6773244c 54247079 6f332e2e 6572722e gs$LT$pyo3..err.
-  0x00017d40 2e507944 6f776e63 61737445 72726f72 .PyDowncastError
-  0x00017d50 41726775 6d656e74 73244754 242e2e24 Arguments$GT$..$
-  0x00017d60 75376224 24753762 24636c6f 73757265 u7b$$u7b$closure
-  0x00017d70 24753764 24247537 64242447 54243137 $u7d$$u7d$$GT$17
-  0x00017d80 68383736 64353966 65336231 33306230 h876d59fe3b130b0
-  0x00017d90 37452e6c 6c766d2e 33313630 39303732 7E.llvm.31609072
-  0x00017da0 38313838 30373831 31323300 5f5a4e31 81880781123._ZN1
-  0x00017db0 30335f24 4c542473 74642e2e 73796e63 03_$LT$std..sync
-  0x00017dc0 2e2e6d70 73632e2e 54727952 65637645 ..mpsc..TryRecvE
-  0x00017dd0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x00017de0 636f7265 2e2e636f 6e766572 742e2e46 core..convert..F
-  0x00017df0 726f6d24 4c542473 74642e2e 73796e63 rom$LT$std..sync
-  0x00017e00 2e2e6d70 73632e2e 52656376 4572726f ..mpsc..RecvErro
-  0x00017e10 72244754 24244754 24346672 6f6d3137 r$GT$$GT$4from17
-  0x00017e20 68623263 66383033 66333631 62363265 hb2cf803f361b62e
-  0x00017e30 31450061 6e6f6e2e 65396562 32333763 1E.anon.e9eb237c
-  0x00017e40 66353061 34336236 35643633 36623066 f50a43b65d636b0f
-  0x00017e50 34373730 62303465 2e32392e 6c6c766d 4770b04e.29.llvm
-  0x00017e60 2e313338 36313835 32373131 33393032 .138618527113902
-  0x00017e70 37343736 005f5a4e 37375f24 4c542470 7476._ZN77_$LT$p
-  0x00017e80 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
-  0x00017e90 2e50794e 6f744144 69726563 746f7279 .PyNotADirectory
-  0x00017ea0 4572726f 72247532 30246173 24753230 Error$u20$as$u20
-  0x00017eb0 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
-  0x00017ec0 6c617924 47542433 666d7431 37683132 lay$GT$3fmt17h12
-  0x00017ed0 39383462 31306530 65626665 38344500 984b10e0ebfe84E.
-  0x00017ee0 5f5a4e36 305f244c 54247374 642e2e69 _ZN60_$LT$std..i
-  0x00017ef0 6f2e2e65 72726f72 2e2e4572 726f7224 o..error..Error$
-  0x00017f00 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x00017f10 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
-  0x00017f20 2433666d 74313768 33653334 32393266 $3fmt17h3e34292f
-  0x00017f30 36636435 66633430 45005f5f 72646c5f 6cd5fc40E.__rdl_
-  0x00017f40 7265616c 6c6f6300 616e6f6e 2e363832 realloc.anon.682
-  0x00017f50 66303533 62613364 36643134 61663562 f053ba3d6d14af5b
-  0x00017f60 32376366 63626264 31363336 332e3431 27cfcbbd16363.41
-  0x00017f70 2e6c6c76 6d2e3536 39373932 39373639 .llvm.5697929769
-  0x00017f80 31333330 35373437 36005f5a 4e34636f 133057476._ZN4co
-  0x00017f90 72653370 74723132 3364726f 705f696e re3ptr123drop_in
-  0x00017fa0 5f706c61 6365244c 54247079 6f332e2e _place$LT$pyo3..
-  0x00017fb0 6572722e 2e657272 5f737461 74652e2e err..err_state..
-  0x00017fc0 626f7865 645f6172 6773244c 5424636f boxed_args$LT$co
-  0x00017fd0 72652e2e 6e65742e 2e706172 7365722e re..net..parser.
-  0x00017fe0 2e416464 72506172 73654572 726f7224 .AddrParseError$
-  0x00017ff0 4754242e 2e247537 62242475 37622463 GT$..$u7b$$u7b$c
-  0x00018000 6c6f7375 72652475 37642424 75376424 losure$u7d$$u7d$
-  0x00018010 24475424 31376861 63383366 35343931 $GT$17hac83f5491
-  0x00018020 62633137 64333545 2e6c6c76 6d2e3331 bc17d35E.llvm.31
-  0x00018030 36303930 37323831 38383037 38313132 6090728188078112
-  0x00018040 33005f5a 4e35395f 244c5424 636f7265 3._ZN59_$LT$core
-  0x00018050 2e2e666d 742e2e41 7267756d 656e7473 ..fmt..Arguments
-  0x00018060 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00018070 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
-  0x00018080 54243366 6d743137 68343137 35623035 T$3fmt17h4175b05
-  0x00018090 36656430 66616232 3645005f 5a4e3373 6ed0fab26E._ZN3s
-  0x000180a0 74643373 79733475 6e697835 6c6f636b td3sys4unix5lock
-  0x000180b0 73313266 75746578 5f72776c 6f636b36 s12futex_rwlock6
-  0x000180c0 52774c6f 636b3232 77616b65 5f777269 RwLock22wake_wri
-  0x000180d0 7465725f 6f725f72 65616465 72733137 ter_or_readers17
-  0x000180e0 68356261 34623766 38303063 62643034 h5ba4b7f800cbd04
-  0x000180f0 34450061 6e6f6e2e 33343764 32363465 4E.anon.347d264e
-  0x00018100 33346562 33613063 37346265 35613839 34eb3a0c74be5a89
-  0x00018110 66383935 61633765 2e36312e 6c6c766d f895ac7e.61.llvm
-  0x00018120 2e313736 39353736 32333431 37383134 .176957623417814
-  0x00018130 35333031 3200616e 6f6e2e36 38326630 53012.anon.682f0
-  0x00018140 35336261 33643664 31346166 35623237 53ba3d6d14af5b27
-  0x00018150 63666362 62643136 3336332e 31312e6c cfcbbd16363.11.l
-  0x00018160 6c766d2e 35363937 39323937 36393133 lvm.569792976913
-  0x00018170 33303537 34373600 5f5a4e34 636f7265 3057476._ZN4core
-  0x00018180 37756e69 636f6465 39707269 6e746162 7unicode9printab
-  0x00018190 6c653132 69735f70 72696e74 61626c65 le12is_printable
-  0x000181a0 31376839 61363637 33343263 37313236 17h9a667342c7126
-  0x000181b0 34663945 005f5a4e 3470796f 33357479 4f9E._ZN4pyo35ty
-  0x000181c0 70657336 6d6f6475 6c653850 794d6f64 pes6module8PyMod
-  0x000181d0 756c6534 6e616d65 31376837 31326234 ule4name17h712b4
-  0x000181e0 63383366 38343238 35373045 005f5a4e c83f8428570E._ZN
-  0x000181f0 3567696d 6c693472 65616436 61626272 5gimli4read6abbr
-  0x00018200 65763132 41626272 65766961 74696f6e ev12Abbreviation
-  0x00018210 336e6577 31376831 38616338 35306234 3new17h18ac850b4
-  0x00018220 35643833 66646445 005f5a4e 37305f24 5d83fddE._ZN70_$
-  0x00018230 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x00018240 6f6e732e 2e50794d 656d6f72 79457272 ons..PyMemoryErr
-  0x00018250 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
-  0x00018260 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x00018270 24475424 33666d74 31376861 62636131 $GT$3fmt17habca1
-  0x00018280 39636365 35616663 39656645 005f5a4e 9cce5afc9efE._ZN
-  0x00018290 35375f24 4c542463 6f72652e 2e666d74 57_$LT$core..fmt
-  0x000182a0 2e2e466f 726d6174 74657224 75323024 ..Formatter$u20$
-  0x000182b0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x000182c0 2e2e5772 69746524 47542439 77726974 ..Write$GT$9writ
-  0x000182d0 655f666d 74313768 36356431 34633933 e_fmt17h65d14c93
-  0x000182e0 35636437 31656662 45005f5a 4e347079 5cd71efbE._ZN4py
-  0x000182f0 6f333367 696c3133 52656665 72656e63 o33gil13Referenc
-  0x00018300 65506f6f 6c313375 70646174 655f636f ePool13update_co
-  0x00018310 756e7473 31376833 34383764 38663537 unts17h3487d8f57
-  0x00018320 30303237 63313545 005f5a4e 37365f24 0027c15E._ZN76_$
-  0x00018330 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
-  0x00018340 6f6e732e 2e617379 6e63696f 2e2e5469 ons..asyncio..Ti
-  0x00018350 6d656f75 74457272 6f722475 32302461 meoutError$u20$a
-  0x00018360 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
-  0x00018370 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
-  0x00018380 68353536 32643437 31636634 31303732 h5562d471cf41072
-  0x00018390 6445005f 5a4e3463 6f726533 70747237 dE._ZN4core3ptr7
-  0x000183a0 3864726f 705f696e 5f706c61 6365244c 8drop_in_place$L
-  0x000183b0 54247079 6f332e2e 696e7374 616e6365 T$pyo3..instance
-  0x000183c0 2e2e5079 244c5424 70796f33 2e2e7479 ..Py$LT$pyo3..ty
-  0x000183d0 7065732e 2e747970 656f626a 6563742e pes..typeobject.
-  0x000183e0 2e507954 79706524 47542424 47542431 .PyType$GT$$GT$1
-  0x000183f0 37683232 31356433 61396230 62653936 7h2215d3a9b0be96
-  0x00018400 3963452e 6c6c766d 2e313338 36313835 9cE.llvm.1386185
-  0x00018410 32373131 33393032 37343736 005f5a4e 271139027476._ZN
-  0x00018420 3470796f 3335696d 706c5f31 36657874 4pyo35impl_16ext
-  0x00018430 72616374 5f617267 756d656e 74313946 ract_argument19F
-  0x00018440 756e6374 696f6e44 65736372 69707469 unctionDescripti
-  0x00018450 6f6e3239 746f6f5f 6d616e79 5f706f73 on29too_many_pos
-  0x00018460 6974696f 6e616c5f 61726775 6d656e74 itional_argument
-  0x00018470 73313768 37393534 33666639 34393666 s17h79543ff9496f
-  0x00018480 61646236 45005f5a 4e37325f 244c5424 adb6E._ZN72_$LT$
-  0x00018490 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
-  0x000184a0 2e2e5079 53746f70 49746572 6174696f ..PyStopIteratio
-  0x000184b0 6e247532 30246173 24753230 24636f72 n$u20$as$u20$cor
-  0x000184c0 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
-  0x000184d0 47542433 666d7431 37683630 36656662 GT$3fmt17h606efb
-  0x000184e0 64393438 35366462 36664500 5f5a4e34 d94856db6fE._ZN4
-  0x000184f0 636f7265 336f7073 3866756e 6374696f core3ops8functio
-  0x00018500 6e36466e 4f6e6365 34306361 6c6c5f6f n6FnOnce40call_o
-  0x00018510 6e636524 75376224 24753762 24767461 nce$u7b$$u7b$vta
-  0x00018520 626c652e 7368696d 24753764 24247537 ble.shim$u7d$$u7
-  0x00018530 64243137 68373365 37613937 36353562 d$17h73e7a97655b
-  0x00018540 64376661 30452e6c 6c766d2e 33313630 d7fa0E.llvm.3160
-  0x00018550 39303732 38313838 30373831 31323300 907281880781123.
-  0x00018560 5f5a4e33 73746432 696f3573 7464696f _ZN3std2io5stdio
-  0x00018570 375f6570 72696e74 31376832 31393263 7_eprint17h2192c
-  0x00018580 66386532 33336364 36616145 005f5a4e f8e233cd6aaE._ZN
-  0x00018590 37375f24 4c542470 796f332e 2e657863 77_$LT$pyo3..exc
-  0x000185a0 65707469 6f6e732e 2e507955 6e69636f eptions..PyUnico
-  0x000185b0 6465456e 636f6465 4572726f 72247532 deEncodeError$u2
-  0x000185c0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x000185d0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
-  0x000185e0 666d7431 37686661 35393535 36313237 fmt17hfa59556127
-  0x000185f0 38626333 36664500 5f5a4e38 345f244c 8bc36fE._ZN84_$L
-  0x00018600 5424636f 72652e2e 63686172 2e2e4573 T$core..char..Es
-  0x00018610 63617065 44656661 756c7424 75323024 capeDefault$u20$
-  0x00018620 61732475 32302463 6f72652e 2e697465 as$u20$core..ite
-  0x00018630 722e2e74 72616974 732e2e69 74657261 r..traits..itera
-  0x00018640 746f722e 2e497465 7261746f 72244754 tor..Iterator$GT
-  0x00018650 24346e65 78743137 68383566 36366538 $4next17h85f66e8
-  0x00018660 35343663 35626435 3845005f 5a4e3463 546c5bd58E._ZN4c
-  0x00018670 6f726535 70616e69 63313070 616e6963 ore5panic10panic
-  0x00018680 5f696e66 6f395061 6e696349 6e666f31 _info9PanicInfo1
-  0x00018690 3063616e 5f756e77 696e6431 37686362 0can_unwind17hcb
-  0x000186a0 62383633 36363862 36373033 65664500 b863668b6703efE.
-  0x000186b0 5f5a4e36 385f244c 5424636f 72652e2e _ZN68_$LT$core..
-  0x000186c0 666d742e 2e627569 6c646572 732e2e50 fmt..builders..P
-  0x000186d0 61644164 61707465 72247532 30246173 adAdapter$u20$as
-  0x000186e0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x000186f0 57726974 65244754 24397772 6974655f Write$GT$9write_
-  0x00018700 73747231 37686233 31633035 34353462 str17hb31c05454b
-  0x00018710 36383061 61324500 616e6f6e 2e613830 680aa2E.anon.a80
-  0x00018720 39303264 36626230 38373733 62663637 902d6bb08773bf67
-  0x00018730 34336430 32336337 64663733 652e3137 43d023c7df73e.17
-  0x00018740 2e6c6c76 6d2e3131 39343036 32313336 .llvm.1194062136
-  0x00018750 37353630 36363238 30350061 6e6f6e2e 7560662805.anon.
-  0x00018760 33343764 32363465 33346562 33613063 347d264e34eb3a0c
-  0x00018770 37346265 35613839 66383935 61633765 74be5a89f895ac7e
-  0x00018780 2e31352e 6c6c766d 2e313736 39353736 .15.llvm.1769576
-  0x00018790 32333431 37383134 35333031 32005f5a 2341781453012._Z
-  0x000187a0 4e34636f 72653366 66693563 5f737472 N4core3ffi5c_str
-  0x000187b0 34435374 72313966 726f6d5f 62797465 4CStr19from_byte
-  0x000187c0 735f7769 74685f6e 756c3137 68363062 s_with_nul17h60b
-  0x000187d0 61366237 39333633 32353663 6345005f a6b79363256ccE._
-  0x000187e0 5a4e3638 5f244c54 2470796f 332e2e65 ZN68_$LT$pyo3..e
-  0x000187f0 78636570 74696f6e 732e2e50 79427566 xceptions..PyBuf
-  0x00018800 66657245 72726f72 24753230 24617324 ferError$u20$as$
-  0x00018810 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
-  0x00018820 65627567 24475424 33666d74 31376831 ebug$GT$3fmt17h1
-  0x00018830 65336662 34613330 65303965 64353445 e3fb4a30e09ed54E
-  0x00018840 00616e6f 6e2e6239 61303438 36633030 .anon.b9a0486c00
-  0x00018850 61343137 32623762 31616335 32623331 a4172b7b1ac52b31
-  0x00018860 35616134 61332e32 352e6c6c 766d2e31 5aa4a3.25.llvm.1
-  0x00018870 33323338 38393334 33323230 30363932 3238893432200692
-  0x00018880 32323600 616e6f6e 2e376239 34366165 226.anon.7b946ae
-  0x00018890 31643361 36363637 39376532 64623166 1d3a666797e2db1f
-  0x000188a0 33366534 63643665 372e3238 2e6c6c76 36e4cd6e7.28.llv
-  0x000188b0 6d2e3138 33353637 35303438 35363134 m.18356750485614
-  0x000188c0 35313331 3239005f 5f706f77 69736632 513129.__powisf2
-  0x000188d0 005f5a4e 3470796f 33336769 6c355354 ._ZN4pyo33gil5ST
-  0x000188e0 41525431 37683538 35323366 30383462 ART17h58523f084b
-  0x000188f0 38666339 3138452e 6c6c766d 2e313332 8fc918E.llvm.132
-  0x00018900 33383839 33343332 32303036 39323232 3889343220069222
-  0x00018910 3600616e 6f6e2e37 62393436 61653164 6.anon.7b946ae1d
-  0x00018920 33613636 36373937 65326462 31663336 3a666797e2db1f36
-  0x00018930 65346364 3665372e 32392e6c 6c766d2e e4cd6e7.29.llvm.
-  0x00018940 31383335 36373530 34383536 31343531 1835675048561451
-  0x00018950 33313239 005f5a4e 3470796f 3335696d 3129._ZN4pyo35im
-  0x00018960 706c5f31 36657874 72616374 5f617267 pl_16extract_arg
-  0x00018970 756d656e 74313946 756e6374 696f6e44 ument19FunctionD
-  0x00018980 65736372 69707469 6f6e3237 756e6578 escription27unex
-  0x00018990 70656374 65645f6b 6579776f 72645f61 pected_keyword_a
-  0x000189a0 7267756d 656e7431 37686332 65613033 rgument17hc2ea03
-  0x000189b0 31363534 39623763 62314500 5f5a4e33 16549b7cb1E._ZN3
-  0x000189c0 365f244c 54245424 75323024 61732475 6_$LT$T$u20$as$u
-  0x000189d0 32302463 6f72652e 2e616e79 2e2e416e 20$core..any..An
-  0x000189e0 79244754 24377479 70655f69 64313768 y$GT$7type_id17h
-  0x000189f0 33376433 30383166 61376539 31323837 37d3081fa7e91287
-  0x00018a00 45005f5a 4e34636f 72653366 6d743946 E._ZN4core3fmt9F
-  0x00018a10 6f726d61 74746572 336e6577 31376864 ormatter3new17hd
-  0x00018a20 39343336 36643361 65366362 63646645 94366d3ae6cbcdfE
-  0x00018a30 005f5a4e 34636f72 65357061 6e696331 ._ZN4core5panic1
-  0x00018a40 3070616e 69635f69 6e666f39 50616e69 0panic_info9Pani
-  0x00018a50 63496e66 6f377061 796c6f61 64313768 cInfo7payload17h
-  0x00018a60 62336432 31333434 38373839 34646538 b3d2134487894de8
-  0x00018a70 45005f5f 72757374 5f616c6c 6f635f65 E.__rust_alloc_e
-  0x00018a80 72726f72 5f68616e 646c6572 005f5a4e rror_handler._ZN
-  0x00018a90 34636f72 65337074 72353264 726f705f 4core3ptr52drop_
-  0x00018aa0 696e5f70 6c616365 244c5424 7374642e in_place$LT$std.
-  0x00018ab0 2e746872 6561642e 2e6c6f63 616c2e2e .thread..local..
-  0x00018ac0 41636365 73734572 726f7224 47542431 AccessError$GT$1
-  0x00018ad0 37683639 37626434 35346464 33626131 7h697bd454dd3ba1
-  0x00018ae0 6662452e 6c6c766d 2e313833 35363735 fbE.llvm.1835675
-  0x00018af0 30343835 36313435 31333132 39005f5a 0485614513129._Z
-  0x00018b00 4e347079 6f333574 79706573 36737472 N4pyo35types6str
-  0x00018b10 696e6738 50795374 72696e67 3135746f ing8PyString15to
-  0x00018b20 5f737472 696e675f 6c6f7373 79313768 _string_lossy17h
-  0x00018b30 64393966 32306366 30633832 35623262 d99f20cf0c825b2b
-  0x00018b40 45005f5a 4e34636f 72653370 74723131 E._ZN4core3ptr11
-  0x00018b50 3964726f 705f696e 5f706c61 6365244c 9drop_in_place$L
-  0x00018b60 54247079 6f332e2e 6572722e 2e657272 T$pyo3..err..err
-  0x00018b70 5f737461 74652e2e 626f7865 645f6172 _state..boxed_ar
-  0x00018b80 6773244c 5424616c 6c6f632e 2e737472 gs$LT$alloc..str
-  0x00018b90 696e672e 2e46726f 6d557466 31364572 ing..FromUtf16Er
-  0x00018ba0 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
-  0x00018bb0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
-  0x00018bc0 75376424 24475424 31376839 34383131 u7d$$GT$17h94811
-  0x00018bd0 66653461 63653734 61663245 2e6c6c76 fe4ace74af2E.llv
-  0x00018be0 6d2e3331 36303930 37323831 38383037 m.31609072818807
-  0x00018bf0 38313132 33005f5a 4e347079 6f333574 81123._ZN4pyo35t
-  0x00018c00 79706573 35747570 6c653132 375f244c ypes5tuple127_$L
-  0x00018c10 5424696d 706c2475 32302470 796f332e T$impl$u20$pyo3.
-  0x00018c20 2e636f6e 76657273 696f6e2e 2e496e74 .conversion..Int
-  0x00018c30 6f507924 4c542470 796f332e 2e696e73 oPy$LT$pyo3..ins
-  0x00018c40 74616e63 652e2e50 79244c54 2470796f tance..Py$LT$pyo
-  0x00018c50 332e2e74 79706573 2e2e616e 792e2e50 3..types..any..P
-  0x00018c60 79416e79 24475424 24475424 24753230 yAny$GT$$GT$$u20
-  0x00018c70 24666f72 24753230 24244c50 24543024 $for$u20$$LP$T0$
-  0x00018c80 43245431 24525024 24475424 37696e74 C$T1$RP$$GT$7int
-  0x00018c90 6f5f7079 31376832 30613830 35346331 o_py17h20a8054c1
-  0x00018ca0 61323463 62643345 005f5a4e 33737464 a24cbd3E._ZN3std
-  0x00018cb0 32696f35 57726974 65397772 6974655f 2io5Write9write_
-  0x00018cc0 666d7431 37686238 39363132 63646163 fmt17hb89612cdac
-  0x00018cd0 66313735 65654500 5f5a4e34 70796f33 f175eeE._ZN4pyo3
-  0x00018ce0 35696d70 6c5f3136 65787472 6163745f 5impl_16extract_
-  0x00018cf0 61726775 6d656e74 31394675 6e637469 argument19Functi
-  0x00018d00 6f6e4465 73637269 7074696f 6e333370 onDescription33p
-  0x00018d10 6f736974 696f6e61 6c5f6f6e 6c795f6b ositional_only_k
-  0x00018d20 6579776f 72645f61 7267756d 656e7473 eyword_arguments
-  0x00018d30 31376836 39643939 33643062 39326264 17h69d993d0b92bd
-  0x00018d40 61396445 005f5a4e 3470796f 33336572 a9dE._ZN4pyo33er
-  0x00018d50 72313770 616e6963 5f616674 65725f65 r17panic_after_e
-  0x00018d60 72726f72 31376865 37616466 64336163 rror17he7adfd3ac
-  0x00018d70 38643164 38616345 00616e6f 6e2e3762 8d1d8acE.anon.7b
-  0x00018d80 39343661 65316433 61363636 37393765 946ae1d3a666797e
-  0x00018d90 32646231 66333665 34636436 65372e33 2db1f36e4cd6e7.3
-  0x00018da0 312e6c6c 766d2e31 38333536 37353034 1.llvm.183567504
-  0x00018db0 38353631 34353133 31323900 5f5a4e35 85614513129._ZN5
-  0x00018dc0 616c6c6f 63313163 6f6c6c65 6374696f alloc11collectio
-  0x00018dd0 6e733562 74726565 346e6f64 65313073 ns5btree4node10s
-  0x00018de0 706c6974 706f696e 74313768 33363535 plitpoint17h3655
-  0x00018df0 35333230 64663739 37326465 45005f5a 5320df7972deE._Z
-  0x00018e00 4e34636f 72653370 74723931 64726f70 N4core3ptr91drop
-  0x00018e10 5f696e5f 706c6163 65244c54 24636f72 _in_place$LT$cor
-  0x00018e20 652e2e63 656c6c2e 2e526566 4d757424 e..cell..RefMut$
-  0x00018e30 4c542461 6c6c6f63 2e2e7665 632e2e56 LT$alloc..vec..V
-  0x00018e40 6563244c 54247374 642e2e74 68726561 ec$LT$std..threa
-  0x00018e50 642e2e54 68726561 64496424 47542424 d..ThreadId$GT$$
-  0x00018e60 47542424 47542431 37683636 39613835 GT$$GT$17h669a85
-  0x00018e70 34643131 65323135 6362452e 6c6c766d 4d11e215cbE.llvm
-  0x00018e80 2e313833 35363735 30343835 36313435 .183567504856145
-  0x00018e90 31333132 39005f5a 4e34636f 72653370 13129._ZN4core3p
-  0x00018ea0 74723337 64726f70 5f696e5f 706c6163 tr37drop_in_plac
-  0x00018eb0 65244c54 2470796f 332e2e65 72722e2e e$LT$pyo3..err..
-  0x00018ec0 50794572 72244754 24313768 62643734 PyErr$GT$17hbd74
-  0x00018ed0 35376230 32303537 33643162 452e6c6c 57b020573d1bE.ll
-  0x00018ee0 766d2e31 33383631 38353237 31313339 vm.1386185271139
-  0x00018ef0 30323734 3736005f 5a4e3635 5f244c54 027476._ZN65_$LT
-  0x00018f00 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
-  0x00018f10 732e2e50 794b6579 4572726f 72247532 s..PyKeyError$u2
-  0x00018f20 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
-  0x00018f30 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
-  0x00018f40 74313768 31346533 61306137 30353961 t17h14e3a0a7059a
-  0x00018f50 33343666 4500616e 6f6e2e62 39613034 346fE.anon.b9a04
-  0x00018f60 38366330 30613431 37326237 62316163 86c00a4172b7b1ac
-  0x00018f70 35326233 31356161 3461332e 33362e6c 52b315aa4a3.36.l
-  0x00018f80 6c766d2e 31333233 38383933 34333232 lvm.132388934322
-  0x00018f90 30303639 32323236 00616e6f 6e2e3334 00692226.anon.34
-  0x00018fa0 37643236 34653334 65623361 30633734 7d264e34eb3a0c74
-  0x00018fb0 62653561 38396638 39356163 37652e31 be5a89f895ac7e.1
-  0x00018fc0 342e6c6c 766d2e31 37363935 37363233 4.llvm.176957623
-  0x00018fd0 34313738 31343533 30313200 5f5a4e34 41781453012._ZN4
-  0x00018fe0 636f7265 33737472 3136736c 6963655f core3str16slice_
-  0x00018ff0 6572726f 725f6661 696c3137 68333363 error_fail17h33c
-  0x00019000 63323164 37653865 64313465 63450061 c21d7e8ed14ecE.a
-  0x00019010 6e6f6e2e 33343764 32363465 33346562 non.347d264e34eb
-  0x00019020 33613063 37346265 35613839 66383935 3a0c74be5a89f895
-  0x00019030 61633765 2e36302e 6c6c766d 2e313736 ac7e.60.llvm.176
-  0x00019040 39353736 32333431 37383134 35333031 9576234178145301
-  0x00019050 32005f5a 4e35375f 244c5424 636f7265 2._ZN57_$LT$core
-  0x00019060 2e2e666d 742e2e46 6f726d61 74746572 ..fmt..Formatter
-  0x00019070 24753230 24617324 75323024 636f7265 $u20$as$u20$core
-  0x00019080 2e2e666d 742e2e57 72697465 24475424 ..fmt..Write$GT$
-  0x00019090 31307772 6974655f 63686172 31376864 10write_char17hd
-  0x000190a0 30646335 33343439 39373431 35623945 0dc5344997415b9E
-  0x000190b0 005f5a4e 33737464 32696f35 57726974 ._ZN3std2io5Writ
-  0x000190c0 65397772 6974655f 616c6c31 37683064 e9write_all17h0d
-  0x000190d0 62386437 37326233 30326630 30624500 b8d772b302f00bE.
-  0x000190e0 5f5a4e33 73746433 73797334 756e6978 _ZN3std3sys4unix
-  0x000190f0 34617267 7333696d 70313541 5247565f 4args3imp15ARGV_
-  0x00019100 494e4954 5f415252 41593137 68333034 INIT_ARRAY17h304
-  0x00019110 31326132 32666331 37363439 3045005f 12a22fc176490E._
-  0x00019120 5a4e3373 74643373 79733475 6e697834 ZN3std3sys4unix4
-  0x00019130 61726773 33696d70 31354152 47565f49 args3imp15ARGV_I
-  0x00019140 4e49545f 41525241 59313269 6e69745f NIT_ARRAY12init_
-  0x00019150 77726170 70657231 37683565 64373139 wrapper17h5ed719
-  0x00019160 32356636 34373032 30324500 5f5a4e39 25f6470202E._ZN9
-  0x00019170 315f244c 54246164 6472326c 696e652e 1_$LT$addr2line.
-  0x00019180 2e4c6f63 6174696f 6e52616e 6765556e .LocationRangeUn
-  0x00019190 69744974 65722475 32302461 73247532 itIter$u20$as$u2
-  0x000191a0 3024636f 72652e2e 69746572 2e2e7472 0$core..iter..tr
-  0x000191b0 61697473 2e2e6974 65726174 6f722e2e aits..iterator..
-  0x000191c0 49746572 61746f72 24475424 346e6578 Iterator$GT$4nex
-  0x000191d0 74313768 33323639 61633431 37346432 t17h3269ac4174d2
-  0x000191e0 38353862 45005f5a 4e34636f 72653370 858bE._ZN4core3p
-  0x000191f0 74723132 3264726f 705f696e 5f706c61 tr122drop_in_pla
-  0x00019200 6365244c 54247079 6f332e2e 6572722e ce$LT$pyo3..err.
-  0x00019210 2e657272 5f737461 74652e2e 626f7865 .err_state..boxe
-  0x00019220 645f6172 6773244c 5424636f 72652e2e d_args$LT$core..
-  0x00019230 7374722e 2e657272 6f722e2e 50617273 str..error..Pars
-  0x00019240 65426f6f 6c457272 6f722447 54242e2e eBoolError$GT$..
-  0x00019250 24753762 24247537 6224636c 6f737572 $u7b$$u7b$closur
-  0x00019260 65247537 64242475 37642424 47542431 e$u7d$$u7d$$GT$1
-  0x00019270 37683033 61373430 34666638 63383165 7h03a7404ff8c81e
-  0x00019280 6230452e 6c6c766d 2e333136 30393037 b0E.llvm.3160907
-  0x00019290 32383138 38303738 31313233 005f5a4e 281880781123._ZN
-  0x000192a0 35616c6c 6f633561 6c6c6f63 38626f78 5alloc5alloc8box
-  0x000192b0 5f667265 65313768 37363036 31616361 _free17h76061aca
-  0x000192c0 38306662 33393930 452e6c6c 766d2e31 80fb3990E.llvm.1
-  0x000192d0 31323336 35373238 35333530 39363932 1236572853509692
-  0x000192e0 34313600 5f5a4e35 61646c65 72374164 416._ZN5adler7Ad
-  0x000192f0 6c657233 32313177 72697465 5f736c69 ler3211write_sli
-  0x00019300 63653137 68653234 30346636 66323764 ce17he2404f6f27d
-  0x00019310 32656630 3945005f 5a4e3561 6c6c6f63 2ef09E._ZN5alloc
-  0x00019320 37726177 5f766563 31395261 77566563 7raw_vec19RawVec
-  0x00019330 244c5424 54244324 41244754 24313672 $LT$T$C$A$GT$16r
-  0x00019340 65736572 76655f66 6f725f70 75736831 eserve_for_push1
-  0x00019350 37683861 62643431 36386161 30376564 7h8abd4168aa07ed
-  0x00019360 64304500 5f5a4e34 70796f33 35747970 d0E._ZN4pyo35typ
-  0x00019370 65733361 6e793550 79416e79 37736574 es3any5PyAny7set
-  0x00019380 61747472 31376834 61656566 38316430 attr17h4aeef81d0
-  0x00019390 32663862 37666145 005f5a4e 37395f24 2f8b7faE._ZN79_$
-  0x000193a0 4c542473 74642e2e 6261636b 74726163 LT$std..backtrac
-  0x000193b0 655f7273 2e2e7379 6d626f6c 697a652e e_rs..symbolize.
-  0x000193c0 2e53796d 626f6c4e 616d6524 75323024 .SymbolName$u20$
-  0x000193d0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
-  0x000193e0 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
-  0x000193f0 74313768 34333461 63623737 32326333 t17h434acb7722c3
-  0x00019400 64656362 45005f5a 4e36385f 244c5424 decbE._ZN68_$LT$
-  0x00019410 24524624 24753562 24753824 75356424 $RF$$u5b$u8$u5d$
-  0x00019420 24753230 24617324 75323024 6f626a65 $u20$as$u20$obje
-  0x00019430 63742e2e 72656164 2e2e7265 61645f72 ct..read..read_r
-  0x00019440 65662e2e 52656164 52656624 47542431 ef..ReadRef$GT$1
-  0x00019450 39726561 645f6279 7465735f 61745f75 9read_bytes_at_u
-  0x00019460 6e74696c 31376831 37306234 30363064 ntil17h170b4060d
-  0x00019470 62636165 37376145 005f5a4e 34636f72 bcae77aE._ZN4cor
-  0x00019480 65337374 72356c6f 73737939 55746638 e3str5lossy9Utf8
-  0x00019490 4368756e 6b357661 6c696431 37683135 Chunk5valid17h15
-  0x000194a0 64316539 38636331 34353031 38624500 d1e98cc145018bE.
-  0x000194b0 5f5a4e38 315f244c 54247079 6f332e2e _ZN81_$LT$pyo3..
-  0x000194c0 65786365 7074696f 6e732e2e 5079436f exceptions..PyCo
-  0x000194d0 6e6e6563 74696f6e 52656675 73656445 nnectionRefusedE
-  0x000194e0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
-  0x000194f0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
-  0x00019500 61792447 54243366 6d743137 68616134 ay$GT$3fmt17haa4
-  0x00019510 66383065 36393764 30363966 3445005f f80e697d069f4E._
-  0x00019520 5a4e3463 6f726535 736c6963 6535696e ZN4core5slice5in
-  0x00019530 64657832 36736c69 63655f73 74617274 dex26slice_start
-  0x00019540 5f696e64 65785f6c 656e5f66 61696c31 _index_len_fail1
-  0x00019550 37683662 65653430 35626163 36643364 7h6bee405bac6d3d
-  0x00019560 32364500 616e6f6e 2e376239 34366165 26E.anon.7b946ae
-  0x00019570 31643361 36363637 39376532 64623166 1d3a666797e2db1f
-  0x00019580 33366534 63643665 372e3334 2e6c6c76 36e4cd6e7.34.llv
-  0x00019590 6d2e3138 33353637 35303438 35363134 m.18356750485614
-  0x000195a0 35313331 3239005f 5a4e3463 6f726533 513129._ZN4core3
-  0x000195b0 70747234 3264726f 705f696e 5f706c61 ptr42drop_in_pla
-  0x000195c0 6365244c 54247374 642e2e69 6f2e2e65 ce$LT$std..io..e
-  0x000195d0 72726f72 2e2e4572 726f7224 47542431 rror..Error$GT$1
-  0x000195e0 37686334 38646466 32643230 37376665 7hc48ddf2d2077fe
-  0x000195f0 6264452e 6c6c766d 2e383336 34373335 bdE.llvm.8364735
-  0x00019600 31373237 30333437 36333534 005f5a4e 172703476354._ZN
-  0x00019610 34636f72 65397061 6e69636b 696e6735 4core9panicking5
-  0x00019620 70616e69 63313768 39353333 62326665 panic17h9533b2fe
-  0x00019630 65393062 39393965 45005f5a 4e34636f e90b999eE._ZN4co
-  0x00019640 72653366 6d743557 72697465 39777269 re3fmt5Write9wri
-  0x00019650 74655f66 6d743137 68393461 63323432 te_fmt17h94ac242
-  0x00019660 61353465 34373363 3745005f 44594e41 a54e473c7E._DYNA
-  0x00019670 4d494300 5f696e69 74005f5a 4e37365f MIC._init._ZN76_
-  0x00019680 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
-  0x00019690 696f6e73 2e2e5079 49734144 69726563 ions..PyIsADirec
-  0x000196a0 746f7279 4572726f 72247532 30246173 toryError$u20$as
-  0x000196b0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
-  0x000196c0 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
-  0x000196d0 37686433 34343935 37303632 65366130 7hd344957062e6a0
-  0x000196e0 36654500 5f5a4e37 355f244c 54247079 6eE._ZN75_$LT$py
-  0x000196f0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
-  0x00019700 5079496e 74657272 75707465 64457272 PyInterruptedErr
-  0x00019710 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
-  0x00019720 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
-  0x00019730 24475424 33666d74 31376866 37613264 $GT$3fmt17hf7a2d
-  0x00019740 34616465 30393938 36356445 005f5a4e 4ade099865dE._ZN
-  0x00019750 34636f72 6533666d 74313770 6f696e74 4core3fmt17point
-  0x00019760 65725f66 6d745f69 6e6e6572 31376839 er_fmt_inner17h9
-  0x00019770 37623133 61363132 61383061 34353645 7b13a612a80a456E
-  0x00019780 00616e6f 6e2e3334 37643236 34653334 .anon.347d264e34
-  0x00019790 65623361 30633734 62653561 38396638 eb3a0c74be5a89f8
-  0x000197a0 39356163 37652e36 342e6c6c 766d2e31 95ac7e.64.llvm.1
-  0x000197b0 37363935 37363233 34313738 31343533 7695762341781453
-  0x000197c0 30313200 5f5a4e39 335f244c 5424616c 012._ZN93_$LT$al
-  0x000197d0 6c6f632e 2e636f6c 6c656374 696f6e73 loc..collections
-  0x000197e0 2e2e6274 7265652e 2e6d656d 2e2e7265 ..btree..mem..re
-  0x000197f0 706c6163 652e2e50 616e6963 47756172 place..PanicGuar
-  0x00019800 64247532 30246173 24753230 24636f72 d$u20$as$u20$cor
-  0x00019810 652e2e6f 70732e2e 64726f70 2e2e4472 e..ops..drop..Dr
-  0x00019820 6f702447 54243464 726f7031 37683431 op$GT$4drop17h41
-  0x00019830 38336631 33326662 36343862 30614500 83f132fb648b0aE.
-  0x00019840 5f5a4e34 325f244c 54242452 46245424 _ZN42_$LT$$RF$T$
-  0x00019850 75323024 61732475 32302463 6f72652e u20$as$u20$core.
-  0x00019860 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
-  0x00019870 666d7431 37683463 35383062 63376436 fmt17h4c580bc7d6
-  0x00019880 38306237 30384500 616e6f6e 2e623961 80b708E.anon.b9a
-  0x00019890 30343836 63303061 34313732 62376231 0486c00a4172b7b1
-  0x000198a0 61633532 62333135 61613461 332e3335 ac52b315aa4a3.35
-  0x000198b0 2e6c6c76 6d2e3133 32333838 39333433 .llvm.1323889343
-  0x000198c0 32323030 36393232 32360061 6e6f6e2e 2200692226.anon.
-  0x000198d0 33343764 32363465 33346562 33613063 347d264e34eb3a0c
-  0x000198e0 37346265 35613839 66383935 61633765 74be5a89f895ac7e
-  0x000198f0 2e382e6c 6c766d2e 31373639 35373632 .8.llvm.17695762
-  0x00019900 33343137 38313435 33303132 005f5a4e 341781453012._ZN
-  0x00019910 34636f72 65336e75 6d32315f 244c5424 4core3num21_$LT$
-  0x00019920 696d706c 24753230 24753332 24475424 impl$u20$u32$GT$
-  0x00019930 31346672 6f6d5f73 74725f72 61646978 14from_str_radix
-  0x00019940 31376832 64393733 61663033 63363663 17h2d973af03c66c
-  0x00019950 36326245 00507945 78635f42 61736545 62bE.PyExc_BaseE
-  0x00019960 78636570 74696f6e 00507945 78635f49 xception.PyExc_I
-  0x00019970 6d706f72 74457272 6f720070 74687265 mportError.pthre
-  0x00019980 61645f67 65747370 65636966 69634040 ad_getspecific@@
-  0x00019990 474c4942 435f322e 322e3500 73696e63 GLIBC_2.2.5.sinc
-  0x000199a0 6f736640 40474c49 42435f32 2e322e35 osf@@GLIBC_2.2.5
-  0x000199b0 00507955 6e69636f 64655f41 73456e63 .PyUnicode_AsEnc
-  0x000199c0 6f646564 53747269 6e67005f 556e7769 odedString._Unwi
-  0x000199d0 6e645f47 65745265 67696f6e 53746172 nd_GetRegionStar
-  0x000199e0 74404047 43435f33 2e30006d 656d7365 t@@GCC_3.0.memse
-  0x000199f0 74404047 4c494243 5f322e32 2e350050 t@@GLIBC_2.2.5.P
-  0x00019a00 79457863 65707469 6f6e5f53 65744361 yException_SetCa
-  0x00019a10 75736500 5f556e77 696e645f 53657447 use._Unwind_SetG
-  0x00019a20 52404047 43435f33 2e300070 6f736978 R@@GCC_3.0.posix
-  0x00019a30 5f6d656d 616c6967 6e404047 4c494243 _memalign@@GLIBC
-  0x00019a40 5f322e32 2e350063 6c6f7365 4040474c _2.2.5.close@@GL
-  0x00019a50 4942435f 322e322e 35005f55 6e77696e IBC_2.2.5._Unwin
-  0x00019a60 645f4765 74446174 6152656c 42617365 d_GetDataRelBase
-  0x00019a70 40404743 435f332e 30005079 4578635f @@GCC_3.0.PyExc_
-  0x00019a80 56616c75 65457272 6f720061 626f7274 ValueError.abort
-  0x00019a90 4040474c 4942435f 322e322e 35007074 @@GLIBC_2.2.5.pt
-  0x00019aa0 68726561 645f7365 74737065 63696669 hread_setspecifi
-  0x00019ab0 63404047 4c494243 5f322e32 2e350050 c@@GLIBC_2.2.5.P
-  0x00019ac0 79457863 5f537973 74656d45 72726f72 yExc_SystemError
-  0x00019ad0 005f5f67 6d6f6e5f 73746172 745f5f00 .__gmon_start__.
-  0x00019ae0 50794749 4c537461 74655f52 656c6561 PyGILState_Relea
-  0x00019af0 73650050 79427974 65735f53 697a6500 se.PyBytes_Size.
-  0x00019b00 50794578 63657074 696f6e5f 47657443 PyException_GetC
-  0x00019b10 61757365 006d616c 6c6f6340 40474c49 ause.malloc@@GLI
-  0x00019b20 42435f32 2e322e35 00507945 78635f54 BC_2.2.5.PyExc_T
-  0x00019b30 79706545 72726f72 00507945 72725f47 ypeError.PyErr_G
-  0x00019b40 6976656e 45786365 7074696f 6e4d6174 ivenExceptionMat
-  0x00019b50 63686573 00736368 65645f79 69656c64 ches.sched_yield
-  0x00019b60 4040474c 4942435f 322e322e 35005f55 @@GLIBC_2.2.5._U
-  0x00019b70 6e77696e 645f4465 6c657465 45786365 nwind_DeleteExce
-  0x00019b80 7074696f 6e404047 43435f33 2e300050 ption@@GCC_3.0.P
-  0x00019b90 794f626a 6563745f 53747200 5079556e yObject_Str.PyUn
-  0x00019ba0 69636f64 655f4173 55544638 416e6453 icode_AsUTF8AndS
-  0x00019bb0 697a6500 5079496e 69745f67 656f7267 ize.PyInit_georg
-  0x00019bc0 696f0050 794c6f6e 675f4173 4c6f6e67 io.PyLong_AsLong
-  0x00019bd0 005f5f63 78615f74 68726561 645f6174 .__cxa_thread_at
-  0x00019be0 65786974 5f696d70 6c005f5f 66787374 exit_impl.__fxst
-  0x00019bf0 61743634 4040474c 4942435f 322e322e at64@@GLIBC_2.2.
-  0x00019c00 35005f49 544d5f64 65726567 69737465 5._ITM_deregiste
-  0x00019c10 72544d43 6c6f6e65 5461626c 65005079 rTMCloneTable.Py
-  0x00019c20 466c6f61 745f4672 6f6d446f 75626c65 Float_FromDouble
-  0x00019c30 00617461 6e326640 40474c49 42435f32 .atan2f@@GLIBC_2
-  0x00019c40 2e322e35 005f556e 77696e64 5f476574 .2.5._Unwind_Get
-  0x00019c50 4c616e67 75616765 53706563 69666963 LanguageSpecific
-  0x00019c60 44617461 40404743 435f332e 30005079 Data@@GCC_3.0.Py
-  0x00019c70 4f626a65 63745f47 65744174 74720066 Object_GetAttr.f
-  0x00019c80 72656540 40474c49 42435f32 2e322e35 ree@@GLIBC_2.2.5
-  0x00019c90 00737472 6c656e40 40474c49 42435f32 .strlen@@GLIBC_2
-  0x00019ca0 2e322e35 005f4954 4d5f7265 67697374 .2.5._ITM_regist
-  0x00019cb0 6572544d 436c6f6e 65546162 6c65005f erTMCloneTable._
-  0x00019cc0 556e7769 6e645f52 61697365 45786365 Unwind_RaiseExce
-  0x00019cd0 7074696f 6e404047 43435f33 2e30005f ption@@GCC_3.0._
-  0x00019ce0 5f637861 5f66696e 616c697a 65404047 _cxa_finalize@@G
-  0x00019cf0 4c494243 5f322e32 2e350072 65616c70 LIBC_2.2.5.realp
-  0x00019d00 61746840 40474c49 42435f32 2e330070 ath@@GLIBC_2.3.p
-  0x00019d10 74687265 61645f6b 65795f64 656c6574 thread_key_delet
-  0x00019d20 65404047 4c494243 5f322e32 2e350050 e@@GLIBC_2.2.5.P
-  0x00019d30 79427974 65735f41 73537472 696e6700 yBytes_AsString.
-  0x00019d40 5f5f746c 735f6765 745f6164 64724040 __tls_get_addr@@
-  0x00019d50 474c4942 435f322e 33007379 7363616c GLIBC_2.3.syscal
-  0x00019d60 6c404047 4c494243 5f322e32 2e35005f l@@GLIBC_2.2.5._
-  0x00019d70 556e7769 6e645f47 65744950 40404743 Unwind_GetIP@@GC
-  0x00019d80 435f332e 30005f55 6e77696e 645f4261 C_3.0._Unwind_Ba
-  0x00019d90 636b7472 61636540 40474343 5f332e33 cktrace@@GCC_3.3
-  0x00019da0 006f7065 6e363440 40474c49 42435f32 .open64@@GLIBC_2
-  0x00019db0 2e322e35 00507945 72725f52 6573746f .2.5.PyErr_Resto
-  0x00019dc0 72650062 636d7040 40474c49 42435f32 re.bcmp@@GLIBC_2
-  0x00019dd0 2e322e35 00726561 646c696e 6b404047 .2.5.readlink@@G
-  0x00019de0 4c494243 5f322e32 2e350050 79457272 LIBC_2.2.5.PyErr
-  0x00019df0 5f4e6577 45786365 7074696f 6e576974 _NewExceptionWit
-  0x00019e00 68446f63 00507947 494c5374 6174655f hDoc.PyGILState_
-  0x00019e10 456e7375 72650050 79457272 5f4e6f72 Ensure.PyErr_Nor
-  0x00019e20 6d616c69 7a654578 63657074 696f6e00 malizeException.
-  0x00019e30 6d656d6d 6f766540 40474c49 42435f32 memmove@@GLIBC_2
-  0x00019e40 2e322e35 00507945 72725f46 65746368 .2.5.PyErr_Fetch
-  0x00019e50 0050794d 6f64756c 655f4765 744e616d .PyModule_GetNam
-  0x00019e60 65006174 616e6640 40474c49 42435f32 e.atanf@@GLIBC_2
-  0x00019e70 2e322e35 00507946 6c6f6174 5f417344 .2.5.PyFloat_AsD
-  0x00019e80 6f75626c 65006765 74656e76 4040474c ouble.getenv@@GL
-  0x00019e90 4942435f 322e322e 35005f55 6e77696e IBC_2.2.5._Unwin
-  0x00019ea0 645f4765 74495049 6e666f40 40474343 d_GetIPInfo@@GCC
-  0x00019eb0 5f342e32 2e300064 6c5f6974 65726174 _4.2.0.dl_iterat
-  0x00019ec0 655f7068 64724040 474c4942 435f322e e_phdr@@GLIBC_2.
-  0x00019ed0 322e3500 5f5f6572 726e6f5f 6c6f6361 2.5.__errno_loca
-  0x00019ee0 74696f6e 4040474c 4942435f 322e322e tion@@GLIBC_2.2.
-  0x00019ef0 35005079 4578635f 4f766572 666c6f77 5.PyExc_Overflow
-  0x00019f00 4572726f 72005079 4c697374 5f417070 Error.PyList_App
-  0x00019f10 656e6400 50794f62 6a656374 5f536574 end.PyObject_Set
-  0x00019f20 41747472 00676574 63776440 40474c49 Attr.getcwd@@GLI
-  0x00019f30 42435f32 2e322e35 00507945 72725f50 BC_2.2.5.PyErr_P
-  0x00019f40 72696e74 00507945 78635f41 74747269 rint.PyExc_Attri
-  0x00019f50 62757465 4572726f 72007374 61747800 buteError.statx.
-  0x00019f60 63616c6c 6f634040 474c4942 435f322e calloc@@GLIBC_2.
-  0x00019f70 322e3500 6d756e6d 61704040 474c4942 2.5.munmap@@GLIB
-  0x00019f80 435f322e 322e3500 5f5f7870 675f7374 C_2.2.5.__xpg_st
-  0x00019f90 72657272 6f725f72 4040474c 4942435f rerror_r@@GLIBC_
-  0x00019fa0 322e332e 34005f50 795f4465 616c6c6f 2.3.4._Py_Deallo
-  0x00019fb0 63007772 69746576 4040474c 4942435f c.writev@@GLIBC_
-  0x00019fc0 322e322e 35005079 4d6f6475 6c655f43 2.2.5.PyModule_C
-  0x00019fd0 72656174 65320050 79547570 6c655f4e reate2.PyTuple_N
-  0x00019fe0 6577005f 5f787374 61743634 4040474c ew.__xstat64@@GL
-  0x00019ff0 4942435f 322e322e 35005079 434d6574 IBC_2.2.5.PyCMet
-  0x0001a000 686f645f 4e657700 5f556e77 696e645f hod_New._Unwind_
-  0x0001a010 47657454 65787452 656c4261 73654040 GetTextRelBase@@
-  0x0001a020 4743435f 332e3000 50795475 706c655f GCC_3.0.PyTuple_
-  0x0001a030 53657449 74656d00 6173696e 66404047 SetItem.asinf@@G
-  0x0001a040 4c494243 5f322e32 2e350050 79556e69 LIBC_2.2.5.PyUni
-  0x0001a050 636f6465 5f46726f 6d537472 696e6741 code_FromStringA
-  0x0001a060 6e645369 7a650072 65616c6c 6f634040 ndSize.realloc@@
-  0x0001a070 474c4942 435f322e 322e3500 70746872 GLIBC_2.2.5.pthr
-  0x0001a080 6561645f 6b65795f 63726561 74654040 ead_key_create@@
-  0x0001a090 474c4942 435f322e 322e3500 77726974 GLIBC_2.2.5.writ
-  0x0001a0a0 65404047 4c494243 5f322e32 2e350073 e@@GLIBC_2.2.5.s
-  0x0001a0b0 696e6866 4040474c 4942435f 322e322e inhf@@GLIBC_2.2.
-  0x0001a0c0 35005f55 6e77696e 645f5265 73756d65 5._Unwind_Resume
-  0x0001a0d0 40404743 435f332e 3000636c 6f636b5f @@GCC_3.0.clock_
-  0x0001a0e0 67657474 696d6540 40474c49 42435f32 gettime@@GLIBC_2
-  0x0001a0f0 2e322e35 0050794c 6973745f 4e657700 .2.5.PyList_New.
-  0x0001a100 50794572 725f5072 696e7445 78006d65 PyErr_PrintEx.me
-  0x0001a110 6d637079 4040474c 4942435f 322e3134 mcpy@@GLIBC_2.14
-  0x0001a120 00507955 6e69636f 64655f49 6e746572 .PyUnicode_Inter
-  0x0001a130 6e496e50 6c616365 0050795f 4973496e nInPlace.Py_IsIn
-  0x0001a140 69746961 6c697a65 64005079 4e756d62 itialized.PyNumb
-  0x0001a150 65725f49 6e646578 006d6d61 70404047 er_Index.mmap@@G
-  0x0001a160 4c494243 5f322e32 2e35005f 556e7769 LIBC_2.2.5._Unwi
-  0x0001a170 6e645f53 65744950 40404743 435f332e nd_SetIP@@GCC_3.
-  0x0001a180 30005079 4f626a65 63745f52 65707200 0.PyObject_Repr.
+  0x0000b800 005f5a4e 34636f72 65367265 73756c74 ._ZN4core6result
+  0x0000b810 3133756e 77726170 5f666169 6c656431 13unwrap_failed1
+  0x0000b820 37686466 66353436 35643734 35373462 7hdff5465d74574b
+  0x0000b830 34344500 5f5a4e31 31706172 6b696e67 44E._ZN11parking
+  0x0000b840 5f6c6f74 346f6e63 65344f6e 63653135 _lot4once4Once15
+  0x0000b850 63616c6c 5f6f6e63 655f666f 72636532 call_once_force2
+  0x0000b860 385f2475 37622424 75376224 636c6f73 8_$u7b$$u7b$clos
+  0x0000b870 75726524 75376424 24753764 24313768 ure$u7d$$u7d$17h
+  0x0000b880 66663031 32336334 65636265 36393562 ff0123c4ecbe695b
+  0x0000b890 452e6c6c 766d2e31 33323338 38393334 E.llvm.132388934
+  0x0000b8a0 33323230 30363932 32323600 5f5a4e31 32200692226._ZN1
+  0x0000b8b0 34727573 74635f64 656d616e 676c6531 4rustc_demangle1
+  0x0000b8c0 32747279 5f64656d 616e676c 65313768 2try_demangle17h
+  0x0000b8d0 61333864 30363766 30623536 65396234 a38d067f0b56e9b4
+  0x0000b8e0 45005f5a 4e37315f 244c5424 70796f33 E._ZN71_$LT$pyo3
+  0x0000b8f0 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x0000b900 52656375 7273696f 6e457272 6f722475 RecursionError$u
+  0x0000b910 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x0000b920 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
+  0x0000b930 6d743137 68626333 35613131 65616232 mt17hbc35a11eab2
+  0x0000b940 39653837 6245005f 5a4e3930 5f244c54 9e87bE._ZN90_$LT
+  0x0000b950 24737464 2e2e7061 6e69636b 696e672e $std..panicking.
+  0x0000b960 2e626567 696e5f70 616e6963 5f68616e .begin_panic_han
+  0x0000b970 646c6572 2e2e5061 6e696350 61796c6f dler..PanicPaylo
+  0x0000b980 61642475 32302461 73247532 3024636f ad$u20$as$u20$co
+  0x0000b990 72652e2e 70616e69 632e2e42 6f784d65 re..panic..BoxMe
+  0x0000b9a0 55702447 54243367 65743137 68623633 Up$GT$3get17hb63
+  0x0000b9b0 65313236 63653561 31396266 6145005f e126ce5a19bfaE._
+  0x0000b9c0 5a4e3470 796f3331 31747970 655f6f62 ZN4pyo311type_ob
+  0x0000b9d0 6a656374 31305079 54797065 496e666f ject10PyTypeInfo
+  0x0000b9e0 31317479 70655f6f 626a6563 74313768 11type_object17h
+  0x0000b9f0 36363665 33333037 65393533 32363161 666e3307e953261a
+  0x0000ba00 45005f5a 4e37305f 244c5424 70796f33 E._ZN70_$LT$pyo3
+  0x0000ba10 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x0000ba20 496d706f 72744572 726f7224 75323024 ImportError$u20$
+  0x0000ba30 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x0000ba40 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
+  0x0000ba50 74313768 61643437 35666462 61393636 t17had475fdba966
+  0x0000ba60 38343030 45005f5a 4e347079 6f333570 8400E._ZN4pyo35p
+  0x0000ba70 616e6963 31345061 6e696345 78636570 anic14PanicExcep
+  0x0000ba80 74696f6e 31386672 6f6d5f70 616e6963 tion18from_panic
+  0x0000ba90 5f706179 6c6f6164 31376834 33306334 _payload17h430c4
+  0x0000baa0 32373961 64666338 64383845 005f5a4e 279adfc8d88E._ZN
+  0x0000bab0 36305f24 4c542470 796f332e 2e67696c 60_$LT$pyo3..gil
+  0x0000bac0 2e2e4749 4c506f6f 6c247532 30246173 ..GILPool$u20$as
+  0x0000bad0 24753230 24636f72 652e2e6f 70732e2e $u20$core..ops..
+  0x0000bae0 64726f70 2e2e4472 6f702447 54243464 drop..Drop$GT$4d
+  0x0000baf0 726f7031 37683038 65313335 61333338 rop17h08e135a338
+  0x0000bb00 39313662 31364500 5f5a4e37 315f244c 916b16E._ZN71_$L
+  0x0000bb10 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x0000bb20 6e732e2e 50795265 66657265 6e636545 ns..PyReferenceE
+  0x0000bb30 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x0000bb40 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
+  0x0000bb50 24475424 33666d74 31376839 30316462 $GT$3fmt17h901db
+  0x0000bb60 62653462 32353063 62653845 005f5a4e be4b250cbe8E._ZN
+  0x0000bb70 31317061 726b696e 675f6c6f 74397261 11parking_lot9ra
+  0x0000bb80 775f6d75 74657838 5261774d 75746578 w_mutex8RawMutex
+  0x0000bb90 3131756e 6c6f636b 5f736c6f 77313768 11unlock_slow17h
+  0x0000bba0 31303366 65363762 61323265 39356532 103fe67ba22e95e2
+  0x0000bbb0 45005f5a 4e34636f 72653370 74723233 E._ZN4core3ptr23
+  0x0000bbc0 3364726f 705f696e 5f706c61 6365244c 3drop_in_place$L
+  0x0000bbd0 5424616c 6c6f632e 2e626f78 65642e2e T$alloc..boxed..
+  0x0000bbe0 426f7824 4c542464 796e2475 32302463 Box$LT$dyn$u20$c
+  0x0000bbf0 6f72652e 2e6f7073 2e2e6675 6e637469 ore..ops..functi
+  0x0000bc00 6f6e2e2e 466e244c 5424244c 50242452 on..Fn$LT$$LP$$R
+  0x0000bc10 46247079 6f332e2e 7079636c 6173732e F$pyo3..pyclass.
+  0x0000bc20 2e637265 6174655f 74797065 5f6f626a .create_type_obj
+  0x0000bc30 6563742e 2e507954 79706542 75696c64 ect..PyTypeBuild
+  0x0000bc40 65722443 24244250 246d7574 24753230 er$C$$BP$mut$u20
+  0x0000bc50 2470796f 335f6666 692e2e63 70797468 $pyo3_ffi..cpyth
+  0x0000bc60 6f6e2e2e 6f626a65 63742e2e 50795479 on..object..PyTy
+  0x0000bc70 70654f62 6a656374 24525024 24475424 peObject$RP$$GT$
+  0x0000bc80 24753262 244f7574 70757424 75323024 $u2b$Output$u20$
+  0x0000bc90 24753364 24247532 3024244c 50242452 $u3d$$u20$$LP$$R
+  0x0000bca0 50242447 54242447 54243137 68653331 P$$GT$$GT$17he31
+  0x0000bcb0 36616530 62353335 64663133 38452e6c 6ae0b535df138E.l
+  0x0000bcc0 6c766d2e 31313231 33383839 37363336 lvm.112138897636
+  0x0000bcd0 30353633 33343933 005f5a4e 34636f72 05633493._ZN4cor
+  0x0000bce0 6533666d 74336e75 6d35335f 244c5424 e3fmt3num53_$LT$
+  0x0000bcf0 696d706c 24753230 24636f72 652e2e66 impl$u20$core..f
+  0x0000bd00 6d742e2e 4c6f7765 72486578 24753230 mt..LowerHex$u20
+  0x0000bd10 24666f72 24753230 24753332 24475424 $for$u20$u32$GT$
+  0x0000bd20 33666d74 31376833 38373137 65653830 3fmt17h38717ee80
+  0x0000bd30 65313430 36656545 005f5a4e 35616c6c e1406eeE._ZN5all
+  0x0000bd40 6f633561 6c6c6f63 38626f78 5f667265 oc5alloc8box_fre
+  0x0000bd50 65313768 35356436 32333466 36396666 e17h55d6234f69ff
+  0x0000bd60 62643637 452e6c6c 766d2e31 31323133 bd67E.llvm.11213
+  0x0000bd70 38383937 36333630 35363333 34393300 889763605633493.
+  0x0000bd80 5f5a4e37 315f244c 54247079 6f332e2e _ZN71_$LT$pyo3..
+  0x0000bd90 65786365 7074696f 6e732e2e 50795469 exceptions..PyTi
+  0x0000bda0 6d656f75 74457272 6f722475 32302461 meoutError$u20$a
+  0x0000bdb0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x0000bdc0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x0000bdd0 31376839 37313239 35396562 64666339 17h9712959ebdfc9
+  0x0000bde0 32613345 005f5a4e 34636f72 65337074 2a3E._ZN4core3pt
+  0x0000bdf0 72313137 64726f70 5f696e5f 706c6163 r117drop_in_plac
+  0x0000be00 65244c54 2470796f 332e2e65 72722e2e e$LT$pyo3..err..
+  0x0000be10 6572725f 73746174 652e2e62 6f786564 err_state..boxed
+  0x0000be20 5f617267 73244c54 24636f72 652e2e73 _args$LT$core..s
+  0x0000be30 74722e2e 6572726f 722e2e55 74663845 tr..error..Utf8E
+  0x0000be40 72726f72 24475424 2e2e2475 37622424 rror$GT$..$u7b$$
+  0x0000be50 75376224 636c6f73 75726524 75376424 u7b$closure$u7d$
+  0x0000be60 24753764 24244754 24313768 63343135 $u7d$$GT$17hc415
+  0x0000be70 38336431 66306265 35306262 452e6c6c 83d1f0be50bbE.ll
+  0x0000be80 766d2e33 31363039 30373238 31383830 vm.3160907281880
+  0x0000be90 37383131 3233005f 5a4e3470 796f3335 781123._ZN4pyo35
+  0x0000bea0 70616e69 63313450 616e6963 45786365 panic14PanicExce
+  0x0000beb0 7074696f 6e313574 7970655f 6f626a65 ption15type_obje
+  0x0000bec0 63745f72 61773131 54595045 5f4f424a ct_raw11TYPE_OBJ
+  0x0000bed0 45435431 37686234 64633032 30336630 ECT17hb4dc0203f0
+  0x0000bee0 32663361 3364452e 6c6c766d 2e353639 2f3a3dE.llvm.569
+  0x0000bef0 37393239 37363931 33333035 37343736 7929769133057476
+  0x0000bf00 005f5a4e 35616c6c 6f633366 66693563 ._ZN5alloc3ffi5c
+  0x0000bf10 5f737472 37435374 72696e67 31395f66 _str7CString19_f
+  0x0000bf20 726f6d5f 7665635f 756e6368 65636b65 rom_vec_unchecke
+  0x0000bf30 64313768 36323539 37383433 64386662 d17h62597843d8fb
+  0x0000bf40 65313230 4500616e 6f6e2e65 39656232 e120E.anon.e9eb2
+  0x0000bf50 33376366 35306134 33623635 64363336 37cf50a43b65d636
+  0x0000bf60 62306634 37373062 3034652e 33312e6c b0f4770b04e.31.l
+  0x0000bf70 6c766d2e 31333836 31383532 37313133 lvm.138618527113
+  0x0000bf80 39303237 34373600 5f5a4e37 305f244c 9027476._ZN70_$L
+  0x0000bf90 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x0000bfa0 6e732e2e 5079496d 706f7274 5761726e ns..PyImportWarn
+  0x0000bfb0 696e6724 75323024 61732475 32302463 ing$u20$as$u20$c
+  0x0000bfc0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x0000bfd0 47542433 666d7431 37683365 32646266 GT$3fmt17h3e2dbf
+  0x0000bfe0 62636537 61356438 34344500 5f5a4e33 bce7a5d844E._ZN3
+  0x0000bff0 73746436 74687265 6164356c 6f63616c std6thread5local
+  0x0000c000 34666173 7431324b 6579244c 54245424 4fast12Key$LT$T$
+  0x0000c010 47542431 34747279 5f696e69 7469616c GT$14try_initial
+  0x0000c020 697a6531 37683463 39383530 39383732 ize17h4c98509872
+  0x0000c030 32393936 6539452e 6c6c766d 2e313132 2996e9E.llvm.112
+  0x0000c040 30303731 33353431 34313238 37313538 0071354141287158
+  0x0000c050 39005f5a 4e35385f 244c5424 54247532 9._ZN58_$LT$T$u2
+  0x0000c060 30246173 24753230 2470796f 332e2e65 0$as$u20$pyo3..e
+  0x0000c070 72722e2e 6572725f 73746174 652e2e50 rr..err_state..P
+  0x0000c080 79457272 41726775 6d656e74 73244754 yErrArguments$GT
+  0x0000c090 24396172 67756d65 6e747331 37683066 $9arguments17h0f
+  0x0000c0a0 30653265 39633131 64333836 32364500 0e2e9c11d38626E.
+  0x0000c0b0 5f5a4e34 636f7265 33707472 37316472 _ZN4core3ptr71dr
+  0x0000c0c0 6f705f69 6e5f706c 61636524 4c542463 op_in_place$LT$c
+  0x0000c0d0 6f72652e 2e726573 756c742e 2e526573 ore..result..Res
+  0x0000c0e0 756c7424 4c542475 36342443 2470796f ult$LT$u64$C$pyo
+  0x0000c0f0 332e2e65 72722e2e 50794572 72244754 3..err..PyErr$GT
+  0x0000c100 24244754 24313768 34626632 64303730 $$GT$17h4bf2d070
+  0x0000c110 33323330 34373563 452e6c6c 766d2e31 3230475cE.llvm.1
+  0x0000c120 38333536 37353034 38353631 34353133 8356750485614513
+  0x0000c130 31323900 5f5f7275 73745f72 65616c6c 129.__rust_reall
+  0x0000c140 6f630061 6e6f6e2e 39653131 34656435 oc.anon.9e114ed5
+  0x0000c150 30313064 36323533 62643236 31313239 010d6253bd261129
+  0x0000c160 34373363 64313838 2e362e6c 6c766d2e 473cd188.6.llvm.
+  0x0000c170 38333634 37333531 37323730 33343736 8364735172703476
+  0x0000c180 33353400 5f5a4e33 73746433 73797334 354._ZN3std3sys4
+  0x0000c190 756e6978 32667334 73746174 31376830 unix2fs4stat17h0
+  0x0000c1a0 65386432 30316539 32393338 38356245 e8d201e9293885bE
+  0x0000c1b0 005f5a4e 34636f72 6533666d 74336e75 ._ZN4core3fmt3nu
+  0x0000c1c0 6d35355f 244c5424 696d706c 24753230 m55_$LT$impl$u20
+  0x0000c1d0 24636f72 652e2e66 6d742e2e 55707065 $core..fmt..Uppe
+  0x0000c1e0 72486578 24753230 24666f72 24753230 rHex$u20$for$u20
+  0x0000c1f0 24697369 7a652447 54243366 6d743137 $isize$GT$3fmt17
+  0x0000c200 68633763 34613861 30623433 61396362 hc7c4a8a0b43a9cb
+  0x0000c210 3645005f 5a4e3734 5f244c54 2470796f 6E._ZN74_$LT$pyo
+  0x0000c220 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x0000c230 79497341 44697265 63746f72 79457272 yIsADirectoryErr
+  0x0000c240 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x0000c250 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x0000c260 54243366 6d743137 68666430 39316262 T$3fmt17hfd091bb
+  0x0000c270 64613765 31336461 3645005f 5a4e3831 da7e13da6E._ZN81
+  0x0000c280 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x0000c290 74696f6e 732e2e61 73796e63 696f2e2e tions..asyncio..
+  0x0000c2a0 4c696d69 744f7665 7272756e 4572726f LimitOverrunErro
+  0x0000c2b0 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
+  0x0000c2c0 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
+  0x0000c2d0 2433666d 74313768 31663465 62633365 $3fmt17h1f4ebc3e
+  0x0000c2e0 65633937 32323831 45005f5a 4e37355f ec972281E._ZN75_
+  0x0000c2f0 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x0000c300 696f6e73 2e2e5079 53746f70 4173796e ions..PyStopAsyn
+  0x0000c310 63497465 72617469 6f6e2475 32302461 cIteration$u20$a
+  0x0000c320 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x0000c330 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x0000c340 68633935 30656333 63366561 35353931 hc950ec3c6ea5591
+  0x0000c350 37450061 6e6f6e2e 33343764 32363465 7E.anon.347d264e
+  0x0000c360 33346562 33613063 37346265 35613839 34eb3a0c74be5a89
+  0x0000c370 66383935 61633765 2e322e6c 6c766d2e f895ac7e.2.llvm.
+  0x0000c380 31373639 35373632 33343137 38313435 1769576234178145
+  0x0000c390 33303132 005f5a4e 37305f24 4c542470 3012._ZN70_$LT$p
+  0x0000c3a0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x0000c3b0 2e507953 79737465 6d457272 6f722475 .PySystemError$u
+  0x0000c3c0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x0000c3d0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x0000c3e0 33666d74 31376865 62323461 32343464 3fmt17heb24a244d
+  0x0000c3f0 65326333 63336645 005f5a4e 34636f72 e2c3c3fE._ZN4cor
+  0x0000c400 6535736c 69636535 696e6465 78323273 e5slice5index22s
+  0x0000c410 6c696365 5f696e64 65785f6f 72646572 lice_index_order
+  0x0000c420 5f666169 6c313768 31663861 34666665 _fail17h1f8a4ffe
+  0x0000c430 62316330 30656233 45005f5a 4e337374 b1c00eb3E._ZN3st
+  0x0000c440 64367468 72656164 36546872 65616433 d6thread6Thread3
+  0x0000c450 6e657731 37686237 38356333 38643136 new17hb785c38d16
+  0x0000c460 31633963 35384500 5f5a4e34 636f7265 1c9c58E._ZN4core
+  0x0000c470 33707472 32373264 726f705f 696e5f70 3ptr272drop_in_p
+  0x0000c480 6c616365 244c5424 6c6f636b 5f617069 lace$LT$lock_api
+  0x0000c490 2e2e6d75 7465782e 2e4d7574 65784775 ..mutex..MutexGu
+  0x0000c4a0 61726424 4c542470 61726b69 6e675f6c ard$LT$parking_l
+  0x0000c4b0 6f742e2e 7261775f 6d757465 782e2e52 ot..raw_mutex..R
+  0x0000c4c0 61774d75 74657824 4324244c 5024616c awMutex$C$$LP$al
+  0x0000c4d0 6c6f632e 2e766563 2e2e5665 63244c54 loc..vec..Vec$LT
+  0x0000c4e0 24636f72 652e2e70 74722e2e 6e6f6e5f $core..ptr..non_
+  0x0000c4f0 6e756c6c 2e2e4e6f 6e4e756c 6c244c54 null..NonNull$LT
+  0x0000c500 2470796f 335f6666 692e2e6f 626a6563 $pyo3_ffi..objec
+  0x0000c510 742e2e50 794f626a 65637424 47542424 t..PyObject$GT$$
+  0x0000c520 47542424 4324616c 6c6f632e 2e766563 GT$$C$alloc..vec
+  0x0000c530 2e2e5665 63244c54 24636f72 652e2e70 ..Vec$LT$core..p
+  0x0000c540 74722e2e 6e6f6e5f 6e756c6c 2e2e4e6f tr..non_null..No
+  0x0000c550 6e4e756c 6c244c54 2470796f 335f6666 nNull$LT$pyo3_ff
+  0x0000c560 692e2e6f 626a6563 742e2e50 794f626a i..object..PyObj
+  0x0000c570 65637424 47542424 47542424 52502424 ect$GT$$GT$$RP$$
+  0x0000c580 47542424 47542431 37686661 65326231 GT$$GT$17hfae2b1
+  0x0000c590 33366132 38636663 3865452e 6c6c766d 36a28cfc8eE.llvm
+  0x0000c5a0 2e313332 33383839 33343332 32303036 .132388934322006
+  0x0000c5b0 39323232 3600616e 6f6e2e33 34376432 92226.anon.347d2
+  0x0000c5c0 36346533 34656233 61306337 34626535 64e34eb3a0c74be5
+  0x0000c5d0 61383966 38393561 6337652e 31302e6c a89f895ac7e.10.l
+  0x0000c5e0 6c766d2e 31373639 35373632 33343137 lvm.176957623417
+  0x0000c5f0 38313435 33303132 005f5f72 7573745f 81453012.__rust_
+  0x0000c600 73746172 745f7061 6e696300 616e6f6e start_panic.anon
+  0x0000c610 2e376239 34366165 31643361 36363637 .7b946ae1d3a6667
+  0x0000c620 39376532 64623166 33366534 63643665 97e2db1f36e4cd6e
+  0x0000c630 372e3330 2e6c6c76 6d2e3138 33353637 7.30.llvm.183567
+  0x0000c640 35303438 35363134 35313331 3239005f 50485614513129._
+  0x0000c650 5a4e3734 5f244c54 2470796f 332e2e65 ZN74_$LT$pyo3..e
+  0x0000c660 78636570 74696f6e 732e2e50 7946696c xceptions..PyFil
+  0x0000c670 654e6f74 466f756e 64457272 6f722475 eNotFoundError$u
+  0x0000c680 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x0000c690 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
+  0x0000c6a0 6d743137 68376434 33613133 38656531 mt17h7d43a138ee1
+  0x0000c6b0 65623265 6445005f 5a4e3730 5f244c54 eb2edE._ZN70_$LT
+  0x0000c6c0 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x0000c6d0 732e2e50 794f7665 72666c6f 77457272 s..PyOverflowErr
+  0x0000c6e0 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x0000c6f0 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x0000c700 54243366 6d743137 68663862 61333134 T$3fmt17hf8ba314
+  0x0000c710 39333264 38613337 37450061 6e6f6e2e 932d8a377E.anon.
+  0x0000c720 33343764 32363465 33346562 33613063 347d264e34eb3a0c
+  0x0000c730 37346265 35613839 66383935 61633765 74be5a89f895ac7e
+  0x0000c740 2e352e6c 6c766d2e 31373639 35373632 .5.llvm.17695762
+  0x0000c750 33343137 38313435 33303132 005f5a4e 341781453012._ZN
+  0x0000c760 34636f72 6533666d 74336e75 6d35335f 4core3fmt3num53_
+  0x0000c770 244c5424 696d706c 24753230 24636f72 $LT$impl$u20$cor
+  0x0000c780 652e2e66 6d742e2e 4c6f7765 72486578 e..fmt..LowerHex
+  0x0000c790 24753230 24666f72 24753230 24693634 $u20$for$u20$i64
+  0x0000c7a0 24475424 33666d74 31376861 64616332 $GT$3fmt17hadac2
+  0x0000c7b0 33323139 62336630 32663145 005f5a4e 3219b3f02f1E._ZN
+  0x0000c7c0 3470796f 33357479 70657336 6d6f6475 4pyo35types6modu
+  0x0000c7d0 6c653850 794d6f64 756c6535 696e6465 le8PyModule5inde
+  0x0000c7e0 78313768 65656564 36366132 34663263 x17heeed66a24f2c
+  0x0000c7f0 31376464 45005f5a 4e37315f 244c5424 17ddE._ZN71_$LT$
+  0x0000c800 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x0000c810 2e2e5079 42797465 73576172 6e696e67 ..PyBytesWarning
+  0x0000c820 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x0000c830 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
+  0x0000c840 54243366 6d743137 68623732 30313036 T$3fmt17hb720106
+  0x0000c850 35326231 32616563 6145005f 5a4e3733 52b12aecaE._ZN73
+  0x0000c860 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x0000c870 74696f6e 732e2e50 79526563 75727369 tions..PyRecursi
+  0x0000c880 6f6e4572 726f7224 75323024 61732475 onError$u20$as$u
+  0x0000c890 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
+  0x0000c8a0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
+  0x0000c8b0 65303936 64613863 35623166 36623538 e096da8c5b1f6b58
+  0x0000c8c0 45005f5a 4e35616c 6c6f6337 7261775f E._ZN5alloc7raw_
+  0x0000c8d0 76656331 39526177 56656324 4c542454 vec19RawVec$LT$T
+  0x0000c8e0 24432441 24475424 37726573 65727665 $C$A$GT$7reserve
+  0x0000c8f0 3231646f 5f726573 65727665 5f616e64 21do_reserve_and
+  0x0000c900 5f68616e 646c6531 37683566 64373365 _handle17h5fd73e
+  0x0000c910 35393965 63353166 62644500 5f5a4e34 599ec51fbdE._ZN4
+  0x0000c920 636f7265 33707472 37306472 6f705f69 core3ptr70drop_i
+  0x0000c930 6e5f706c 61636524 4c542470 796f332e n_place$LT$pyo3.
+  0x0000c940 2e696e73 74616e63 652e2e50 79244c54 .instance..Py$LT
+  0x0000c950 2470796f 332e2e74 79706573 2e2e616e $pyo3..types..an
+  0x0000c960 792e2e50 79416e79 24475424 24475424 y..PyAny$GT$$GT$
+  0x0000c970 31376838 63656261 36326462 62303834 17h8ceba62dbb084
+  0x0000c980 65386145 2e6c6c76 6d2e3131 32313338 e8aE.llvm.112138
+  0x0000c990 38393736 33363035 36333334 3933005f 89763605633493._
+  0x0000c9a0 5a4e3561 6c6c6f63 35616c6c 6f633138 ZN5alloc5alloc18
+  0x0000c9b0 68616e64 6c655f61 6c6c6f63 5f657272 handle_alloc_err
+  0x0000c9c0 6f723872 745f6572 726f7231 37683462 or8rt_error17h4b
+  0x0000c9d0 37396638 61373137 37343162 37634500 79f8a717741b7cE.
+  0x0000c9e0 5f5a4e33 73746436 74687265 6164356c _ZN3std6thread5l
+  0x0000c9f0 6f63616c 31374c6f 63616c4b 6579244c ocal17LocalKey$L
+  0x0000ca00 54245424 47542434 77697468 31376837 T$T$GT$4with17h7
+  0x0000ca10 37316430 66643262 32323830 63336145 71d0fd2b2280c3aE
+  0x0000ca20 005f5a4e 34636f72 65337074 72373464 ._ZN4core3ptr74d
+  0x0000ca30 726f705f 696e5f70 6c616365 244c5424 rop_in_place$LT$
+  0x0000ca40 70796f33 2e2e696e 7374616e 63652e2e pyo3..instance..
+  0x0000ca50 5079244c 54247079 6f332e2e 74797065 Py$LT$pyo3..type
+  0x0000ca60 732e2e74 75706c65 2e2e5079 5475706c s..tuple..PyTupl
+  0x0000ca70 65244754 24244754 24313768 36313832 e$GT$$GT$17h6182
+  0x0000ca80 34313266 38383565 62633333 452e6c6c 412f885ebc33E.ll
+  0x0000ca90 766d2e31 31323133 38383937 36333630 vm.1121388976360
+  0x0000caa0 35363333 34393300 5f5a4e36 375f244c 5633493._ZN67_$L
+  0x0000cab0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x0000cac0 6e732e2e 5079496e 64657845 72726f72 ns..PyIndexError
+  0x0000cad0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x0000cae0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
+  0x0000caf0 33666d74 31376832 30646361 65623130 3fmt17h20dcaeb10
+  0x0000cb00 38353632 35303845 005f5a4e 34636f72 8562508E._ZN4cor
+  0x0000cb10 6533666d 7439466f 726d6174 74657231 e3fmt9Formatter1
+  0x0000cb20 35646562 75675f6c 6f776572 5f686578 5debug_lower_hex
+  0x0000cb30 31376865 62356662 30363436 38376331 17heb5fb064687c1
+  0x0000cb40 62336345 005f5a4e 37395f24 4c542470 b3cE._ZN79_$LT$p
+  0x0000cb50 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x0000cb60 2e507943 6f6e6e65 6374696f 6e526566 .PyConnectionRef
+  0x0000cb70 75736564 4572726f 72247532 30246173 usedError$u20$as
+  0x0000cb80 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000cb90 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x0000cba0 65376265 36363932 35663839 63343335 e7be66925f89c435
+  0x0000cbb0 4500616e 6f6e2e65 39656232 33376366 E.anon.e9eb237cf
+  0x0000cbc0 35306134 33623635 64363336 62306634 50a43b65d636b0f4
+  0x0000cbd0 37373062 3034652e 35322e6c 6c766d2e 770b04e.52.llvm.
+  0x0000cbe0 31333836 31383532 37313133 39303237 1386185271139027
+  0x0000cbf0 34373600 5f5a4e37 325f244c 54247079 476._ZN72_$LT$py
+  0x0000cc00 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x0000cc10 50794675 74757265 5761726e 696e6724 PyFutureWarning$
+  0x0000cc20 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x0000cc30 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
+  0x0000cc40 2433666d 74313768 62326332 34633034 $3fmt17hb2c24c04
+  0x0000cc50 64363262 65643635 45005f5a 4e37375f d62bed65E._ZN77_
+  0x0000cc60 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x0000cc70 696f6e73 2e2e5079 53746f70 4173796e ions..PyStopAsyn
+  0x0000cc80 63497465 72617469 6f6e2475 32302461 cIteration$u20$a
+  0x0000cc90 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x0000cca0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x0000ccb0 31376862 65643931 37623035 62356233 17hbed917b05b5b3
+  0x0000ccc0 64633945 005f5a4e 34636f72 65337074 dc9E._ZN4core3pt
+  0x0000ccd0 72343264 726f705f 696e5f70 6c616365 r42drop_in_place
+  0x0000cce0 244c5424 616c6c6f 632e2e73 7472696e $LT$alloc..strin
+  0x0000ccf0 672e2e53 7472696e 67244754 24313768 g..String$GT$17h
+  0x0000cd00 61646139 37616330 65653866 64333563 ada97ac0ee8fd35c
+  0x0000cd10 452e6c6c 766d2e33 30343133 39333935 E.llvm.304139395
+  0x0000cd20 38353639 39373433 3439005f 5a4e3734 8569974349._ZN74
+  0x0000cd30 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x0000cd40 74696f6e 732e2e50 79506572 6d697373 tions..PyPermiss
+  0x0000cd50 696f6e45 72726f72 24753230 24617324 ionError$u20$as$
+  0x0000cd60 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x0000cd70 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
+  0x0000cd80 68656163 34616636 33643964 61386530 heac4af63d9da8e0
+  0x0000cd90 6345005f 5a4e3639 5f244c54 2470796f cE._ZN69_$LT$pyo
+  0x0000cda0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x0000cdb0 7954696d 656f7574 4572726f 72247532 yTimeoutError$u2
+  0x0000cdc0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x0000cdd0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x0000cde0 74313768 34336265 61636365 32373065 t17h43beacce270e
+  0x0000cdf0 66396230 45005f5a 4e34636f 72653573 f9b0E._ZN4core5s
+  0x0000ce00 6c696365 366d656d 63687231 346d656d lice6memchr14mem
+  0x0000ce10 6368725f 616c6967 6e656431 37683034 chr_aligned17h04
+  0x0000ce20 32356463 35333532 38326630 30314500 25dc535282f001E.
+  0x0000ce30 5f5a4e34 636f7265 366f7074 696f6e31 _ZN4core6option1
+  0x0000ce40 33657870 6563745f 6661696c 65643137 3expect_failed17
+  0x0000ce50 68303962 39383236 33393333 36653765 h09b982639336e7e
+  0x0000ce60 6145005f 5a4e3734 5f244c54 2470796f aE._ZN74_$LT$pyo
+  0x0000ce70 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x0000ce80 79556e62 6f756e64 4c6f6361 6c457272 yUnboundLocalErr
+  0x0000ce90 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x0000cea0 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x0000ceb0 54243366 6d743137 68643666 38363233 T$3fmt17hd6f8623
+  0x0000cec0 35616261 63613537 3745005f 5a4e3463 5abaca577E._ZN4c
+  0x0000ced0 6f726533 666d7438 6275696c 64657273 ore3fmt8builders
+  0x0000cee0 31304465 62756754 75706c65 35666965 10DebugTuple5fie
+  0x0000cef0 6c643137 68626330 64303632 34393337 ld17hbc0d0624937
+  0x0000cf00 39633262 3045005f 5a4e3136 7061726b 9c2b0E._ZN16park
+  0x0000cf10 696e675f 6c6f745f 636f7265 39776f72 ing_lot_core9wor
+  0x0000cf20 645f6c6f 636b3857 6f72644c 6f636b31 d_lock8WordLock1
+  0x0000cf30 31756e6c 6f636b5f 736c6f77 31376861 1unlock_slow17ha
+  0x0000cf40 32643766 35383433 65316332 61303445 2d7f5843e1c2a04E
+  0x0000cf50 005f5a4e 34636f72 65337074 72313230 ._ZN4core3ptr120
+  0x0000cf60 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
+  0x0000cf70 2470796f 332e2e65 72722e2e 6572725f $pyo3..err..err_
+  0x0000cf80 73746174 652e2e62 6f786564 5f617267 state..boxed_arg
+  0x0000cf90 73244c54 24636f72 652e2e61 72726179 s$LT$core..array
+  0x0000cfa0 2e2e5472 7946726f 6d536c69 63654572 ..TryFromSliceEr
+  0x0000cfb0 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
+  0x0000cfc0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
+  0x0000cfd0 75376424 24475424 31376835 32346133 u7d$$GT$17h524a3
+  0x0000cfe0 32623333 30386232 64343245 2e6c6c76 2b3308b2d42E.llv
+  0x0000cff0 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x0000d000 38313132 3300616e 6f6e2e37 62393436 81123.anon.7b946
+  0x0000d010 61653164 33613636 36373937 65326462 ae1d3a666797e2db
+  0x0000d020 31663336 65346364 3665372e 32312e6c 1f36e4cd6e7.21.l
+  0x0000d030 6c766d2e 31383335 36373530 34383536 lvm.183567504856
+  0x0000d040 31343531 33313239 00616e6f 6e2e3965 14513129.anon.9e
+  0x0000d050 31313465 64353031 30643632 35336264 114ed5010d6253bd
+  0x0000d060 32363131 32393437 33636431 38382e34 261129473cd188.4
+  0x0000d070 2e6c6c76 6d2e3833 36343733 35313732 .llvm.8364735172
+  0x0000d080 37303334 37363335 34005f5a 4e37315f 703476354._ZN71_
+  0x0000d090 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x0000d0a0 696f6e73 2e2e5079 556e6963 6f646545 ions..PyUnicodeE
+  0x0000d0b0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x0000d0c0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
+  0x0000d0d0 61792447 54243366 6d743137 68373865 ay$GT$3fmt17h78e
+  0x0000d0e0 33353861 34326239 37353332 6445005f 358a42b97532dE._
+  0x0000d0f0 5a4e3733 5f244c54 2470796f 332e2e65 ZN73_$LT$pyo3..e
+  0x0000d100 78636570 74696f6e 732e2e50 79456e76 xceptions..PyEnv
+  0x0000d110 69726f6e 6d656e74 4572726f 72247532 ironmentError$u2
+  0x0000d120 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x0000d130 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x0000d140 74313768 61376137 64373561 64336634 t17ha7a7d75ad3f4
+  0x0000d150 63613336 45005f5a 4e37385f 244c5424 ca36E._ZN78_$LT$
+  0x0000d160 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x0000d170 2e2e5079 4d6f6475 6c654e6f 74466f75 ..PyModuleNotFou
+  0x0000d180 6e644572 726f7224 75323024 61732475 ndError$u20$as$u
+  0x0000d190 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
+  0x0000d1a0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
+  0x0000d1b0 62343265 61303665 36306236 34636433 b42ea06e60b64cd3
+  0x0000d1c0 45005f5a 4e347079 6f333473 796e6332 E._ZN4pyo34sync2
+  0x0000d1d0 3047494c 4f6e6365 43656c6c 244c5424 0GILOnceCell$LT$
+  0x0000d1e0 54244754 2434696e 69743137 68633138 T$GT$4init17hc18
+  0x0000d1f0 39316262 61653139 39383230 6145005f 91bbae199820aE._
+  0x0000d200 5a4e3833 5f244c54 2470796f 332e2e65 ZN83_$LT$pyo3..e
+  0x0000d210 78636570 74696f6e 732e2e61 73796e63 xceptions..async
+  0x0000d220 696f2e2e 496e636f 6d706c65 74655265 io..IncompleteRe
+  0x0000d230 61644572 726f7224 75323024 61732475 adError$u20$as$u
+  0x0000d240 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x0000d250 62756724 47542433 666d7431 37683237 bug$GT$3fmt17h27
+  0x0000d260 37386433 37313437 64343034 65314500 78d37147d404e1E.
+  0x0000d270 5f5a4e34 636f7265 33707472 33376472 _ZN4core3ptr37dr
+  0x0000d280 6f705f69 6e5f706c 61636524 4c542470 op_in_place$LT$p
+  0x0000d290 796f332e 2e657272 2e2e5079 45727224 yo3..err..PyErr$
+  0x0000d2a0 47542431 37686264 37343537 62303230 GT$17hbd7457b020
+  0x0000d2b0 35373364 3162452e 6c6c766d 2e313736 573d1bE.llvm.176
+  0x0000d2c0 39353736 32333431 37383134 35333031 9576234178145301
+  0x0000d2d0 32005f5a 4e36365f 244c5424 70796f33 2._ZN66_$LT$pyo3
+  0x0000d2e0 2e2e7479 7065732e 2e707973 75706572 ..types..pysuper
+  0x0000d2f0 2e2e5079 53757065 72247532 30246173 ..PySuper$u20$as
+  0x0000d300 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000d310 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x0000d320 66613736 39316231 62313730 63383561 fa7691b1b170c85a
+  0x0000d330 45005f5a 4e35616c 6c6f6335 616c6c6f E._ZN5alloc5allo
+  0x0000d340 6338626f 785f6672 65653137 68653830 c8box_free17he80
+  0x0000d350 61646532 35653737 35613464 63452e6c ade25e775a4dcE.l
+  0x0000d360 6c766d2e 38333634 37333531 37323730 lvm.836473517270
+  0x0000d370 33343736 33353400 5f5a4e39 305f244c 3476354._ZN90_$L
+  0x0000d380 54247079 6f332e2e 6572722e 2e507945 T$pyo3..err..PyE
+  0x0000d390 72722475 32302461 73247532 3024636f rr$u20$as$u20$co
+  0x0000d3a0 72652e2e 636f6e76 6572742e 2e46726f re..convert..Fro
+  0x0000d3b0 6d244c54 2470796f 332e2e65 72722e2e m$LT$pyo3..err..
+  0x0000d3c0 5079446f 776e6361 73744572 726f7224 PyDowncastError$
+  0x0000d3d0 47542424 47542434 66726f6d 31376837 GT$$GT$4from17h7
+  0x0000d3e0 62663630 36336134 64616362 66353445 bf6063a4dacbf54E
+  0x0000d3f0 005f5a4e 36365f24 4c542461 6c6c6f63 ._ZN66_$LT$alloc
+  0x0000d400 2e2e626f 72726f77 2e2e436f 77244c54 ..borrow..Cow$LT
+  0x0000d410 24422447 54242475 32302461 73247532 $B$GT$$u20$as$u2
+  0x0000d420 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x0000d430 706c6179 24475424 33666d74 31376861 play$GT$3fmt17ha
+  0x0000d440 31383662 33633066 37623732 65646145 186b3c0f7b72edaE
+  0x0000d450 005f5a4e 31367061 726b696e 675f6c6f ._ZN16parking_lo
+  0x0000d460 745f636f 72653131 7061726b 696e675f t_core11parking_
+  0x0000d470 6c6f7431 36776974 685f7468 72656164 lot16with_thread
+  0x0000d480 5f646174 61313154 48524541 445f4441 _data11THREAD_DA
+  0x0000d490 5441375f 5f676574 6974355f 5f4b4559 TA7__getit5__KEY
+  0x0000d4a0 31376866 63323461 65646165 35333033 17hfc24aedae5303
+  0x0000d4b0 61616545 005f5a4e 34636f72 65337074 aaeE._ZN4core3pt
+  0x0000d4c0 72333764 726f705f 696e5f70 6c616365 r37drop_in_place
+  0x0000d4d0 244c5424 70796f33 2e2e6572 722e2e50 $LT$pyo3..err..P
+  0x0000d4e0 79457272 24475424 31376862 64373435 yErr$GT$17hbd745
+  0x0000d4f0 37623032 30353733 64316245 2e6c6c76 7b020573d1bE.llv
+  0x0000d500 6d2e3138 33353637 35303438 35363134 m.18356750485614
+  0x0000d510 35313331 32390061 6e6f6e2e 33343764 513129.anon.347d
+  0x0000d520 32363465 33346562 33613063 37346265 264e34eb3a0c74be
+  0x0000d530 35613839 66383935 61633765 2e392e6c 5a89f895ac7e.9.l
+  0x0000d540 6c766d2e 31373639 35373632 33343137 lvm.176957623417
+  0x0000d550 38313435 33303132 005f5a4e 34636f72 81453012._ZN4cor
+  0x0000d560 65337074 72363564 726f705f 696e5f70 e3ptr65drop_in_p
+  0x0000d570 6c616365 244c5424 636f7265 2e2e6f70 lace$LT$core..op
+  0x0000d580 74696f6e 2e2e4f70 74696f6e 244c5424 tion..Option$LT$
+  0x0000d590 70796f33 2e2e6572 722e2e50 79457272 pyo3..err..PyErr
+  0x0000d5a0 24475424 24475424 31376866 62346162 $GT$$GT$17hfb4ab
+  0x0000d5b0 37386461 34643239 32616445 2e6c6c76 78da4d292adE.llv
+  0x0000d5c0 6d2e3133 38363138 35323731 31333930 m.13861852711390
+  0x0000d5d0 32373437 36005f5a 4e34636f 72653370 27476._ZN4core3p
+  0x0000d5e0 74723831 64726f70 5f696e5f 706c6163 tr81drop_in_plac
+  0x0000d5f0 65244c54 24616c6c 6f632e2e 7665632e e$LT$alloc..vec.
+  0x0000d600 2e566563 244c5424 7061726b 696e675f .Vec$LT$parking_
+  0x0000d610 6c6f745f 636f7265 2e2e7061 726b696e lot_core..parkin
+  0x0000d620 675f6c6f 742e2e42 75636b65 74244754 g_lot..Bucket$GT
+  0x0000d630 24244754 24313768 33303664 63613836 $$GT$17h306dca86
+  0x0000d640 63636537 30626362 452e6c6c 766d2e31 cce70bcbE.llvm.1
+  0x0000d650 31393236 34333536 39363733 33363137 1926435696733617
+  0x0000d660 37303300 5f5a4e34 636f7265 33666d74 703._ZN4core3fmt
+  0x0000d670 336e756d 35335f24 4c542469 6d706c24 3num53_$LT$impl$
+  0x0000d680 75323024 636f7265 2e2e666d 742e2e55 u20$core..fmt..U
+  0x0000d690 70706572 48657824 75323024 666f7224 pperHex$u20$for$
+  0x0000d6a0 75323024 69363424 47542433 666d7431 u20$i64$GT$3fmt1
+  0x0000d6b0 37686265 64656364 32626634 36643131 7hbedecd2bf46d11
+  0x0000d6c0 30394500 5f5a4e34 636f7265 33666d74 09E._ZN4core3fmt
+  0x0000d6d0 35577269 74653130 77726974 655f6368 5Write10write_ch
+  0x0000d6e0 61723137 68666166 63393236 31663461 ar17hfafc9261f4a
+  0x0000d6f0 35323462 3345005f 5a4e3567 696d6c69 524b3E._ZN5gimli
+  0x0000d700 34726561 64366162 62726576 31304174 4read6abbrev10At
+  0x0000d710 74726962 75746573 336e6577 31376831 tributes3new17h1
+  0x0000d720 62393961 38383765 36336663 66363545 b99a887e63fcf65E
+  0x0000d730 005f5f72 646c5f64 65616c6c 6f63005f .__rdl_dealloc._
+  0x0000d740 5a4e3463 6f726533 70747233 3764726f ZN4core3ptr37dro
+  0x0000d750 705f696e 5f706c61 6365244c 5424636f p_in_place$LT$co
+  0x0000d760 72652e2e 666d742e 2e457272 6f722447 re..fmt..Error$G
+  0x0000d770 54243137 68653230 63633361 36386336 T$17he20cc3a68c6
+  0x0000d780 31626231 39452e6c 6c766d2e 31333233 1bb19E.llvm.1323
+  0x0000d790 38383933 34333232 30303639 32323236 8893432200692226
+  0x0000d7a0 005f5f72 646c5f61 6c6c6f63 5f7a6572 .__rdl_alloc_zer
+  0x0000d7b0 6f656400 5f5a4e34 636f7265 37756e69 oed._ZN4core7uni
+  0x0000d7c0 636f6465 3132756e 69636f64 655f6461 code12unicode_da
+  0x0000d7d0 74613135 67726170 68656d65 5f657874 ta15grapheme_ext
+  0x0000d7e0 656e6436 6c6f6f6b 75703137 68643736 end6lookup17hd76
+  0x0000d7f0 39343635 66393565 34663137 6545005f 9465f95e4f17eE._
+  0x0000d800 5a4e3470 796f3335 696d706c 5f313665 ZN4pyo35impl_16e
+  0x0000d810 78747261 63745f61 7267756d 656e7431 xtract_argument1
+  0x0000d820 3946756e 6374696f 6e446573 63726970 9FunctionDescrip
+  0x0000d830 74696f6e 33376d69 7373696e 675f7265 tion37missing_re
+  0x0000d840 71756972 65645f70 6f736974 696f6e61 quired_positiona
+  0x0000d850 6c5f6172 67756d65 6e747331 37683461 l_arguments17h4a
+  0x0000d860 61616232 64383064 34316161 30364500 aab2d80d41aa06E.
+  0x0000d870 5f5a4e36 355f244c 5424736d 616c6c76 _ZN65_$LT$smallv
+  0x0000d880 65632e2e 436f6c6c 65637469 6f6e416c ec..CollectionAl
+  0x0000d890 6c6f6345 72722475 32302461 73247532 locErr$u20$as$u2
+  0x0000d8a0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x0000d8b0 75672447 54243366 6d743137 68333438 ug$GT$3fmt17h348
+  0x0000d8c0 64343037 36613738 64666130 3545005f d4076a78dfa05E._
+  0x0000d8d0 5a4e3632 5f244c54 24737464 2e2e696f ZN62_$LT$std..io
+  0x0000d8e0 2e2e6572 726f722e 2e457272 6f724b69 ..error..ErrorKi
+  0x0000d8f0 6e642475 32302461 73247532 3024636f nd$u20$as$u20$co
+  0x0000d900 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x0000d910 54243366 6d743137 68633038 33353736 T$3fmt17hc083576
+  0x0000d920 39323137 62623932 3345005f 5a4e3470 9217bb923E._ZN4p
+  0x0000d930 796f3333 65727235 50794572 72347461 yo33err5PyErr4ta
+  0x0000d940 6b653137 68343032 34316137 33303237 ke17h40241a73027
+  0x0000d950 34353233 3445005f 5a4e3734 5f244c54 45234E._ZN74_$LT
+  0x0000d960 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x0000d970 732e2e50 79426c6f 636b696e 67494f45 s..PyBlockingIOE
+  0x0000d980 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x0000d990 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
+  0x0000d9a0 61792447 54243366 6d743137 68313631 ay$GT$3fmt17h161
+  0x0000d9b0 37633063 63653331 65653338 3145005f 7c0cce31ee381E._
+  0x0000d9c0 5a4e3933 5f244c54 24737464 2e2e7061 ZN93_$LT$std..pa
+  0x0000d9d0 6e69636b 696e672e 2e626567 696e5f70 nicking..begin_p
+  0x0000d9e0 616e6963 5f68616e 646c6572 2e2e5374 anic_handler..St
+  0x0000d9f0 7250616e 69635061 796c6f61 64247532 rPanicPayload$u2
+  0x0000da00 30246173 24753230 24636f72 652e2e70 0$as$u20$core..p
+  0x0000da10 616e6963 2e2e426f 784d6555 70244754 anic..BoxMeUp$GT
+  0x0000da20 24387461 6b655f62 6f783137 68623533 $8take_box17hb53
+  0x0000da30 36653831 65633036 61663638 64450061 6e81ec06af68dE.a
+  0x0000da40 6e6f6e2e 65396562 32333763 66353061 non.e9eb237cf50a
+  0x0000da50 34336236 35643633 36623066 34373730 43b65d636b0f4770
+  0x0000da60 62303465 2e33302e 6c6c766d 2e313338 b04e.30.llvm.138
+  0x0000da70 36313835 32373131 33393032 37343736 6185271139027476
+  0x0000da80 005f5a4e 34636f72 6535736c 69636535 ._ZN4core5slice5
+  0x0000da90 696e6465 78323473 6c696365 5f656e64 index24slice_end
+  0x0000daa0 5f696e64 65785f6c 656e5f66 61696c31 _index_len_fail1
+  0x0000dab0 37683935 34616338 37636364 61353463 7h954ac87ccda54c
+  0x0000dac0 36324500 5f5a4e31 36706172 6b696e67 62E._ZN16parking
+  0x0000dad0 5f6c6f74 5f636f72 65313170 61726b69 _lot_core11parki
+  0x0000dae0 6e675f6c 6f743131 46616972 54696d65 ng_lot11FairTime
+  0x0000daf0 6f757437 67656e5f 75333231 37686139 out7gen_u3217ha9
+  0x0000db00 62393266 66353465 63343737 38364500 b92ff54ec47786E.
+  0x0000db10 5f5a4e37 335f244c 54247079 6f332e2e _ZN73_$LT$pyo3..
+  0x0000db20 65786365 7074696f 6e732e2e 5079556e exceptions..PyUn
+  0x0000db30 69636f64 65576172 6e696e67 24753230 icodeWarning$u20
+  0x0000db40 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x0000db50 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x0000db60 6d743137 68333430 65643865 63333534 mt17h340ed8ec354
+  0x0000db70 65643661 3845005f 5a4e3739 5f244c54 ed6a8E._ZN79_$LT
+  0x0000db80 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x0000db90 732e2e50 79436f6e 6e656374 696f6e52 s..PyConnectionR
+  0x0000dba0 65736574 4572726f 72247532 30246173 esetError$u20$as
+  0x0000dbb0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000dbc0 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x0000dbd0 37683839 37366435 38373933 36623637 7h8976d587936b67
+  0x0000dbe0 30334500 5f5a4e34 70796f33 35696d70 03E._ZN4pyo35imp
+  0x0000dbf0 6c5f3136 65787472 6163745f 61726775 l_16extract_argu
+  0x0000dc00 6d656e74 32356172 67756d65 6e745f65 ment25argument_e
+  0x0000dc10 78747261 6374696f 6e5f6572 726f7231 xtraction_error1
+  0x0000dc20 37686363 35383436 65396238 33363961 7hcc5846e9b8369a
+  0x0000dc30 62634500 5f5a4e34 636f7265 33737472 bcE._ZN4core3str
+  0x0000dc40 35636f75 6e743134 646f5f63 6f756e74 5count14do_count
+  0x0000dc50 5f636861 72733137 68376561 30326566 _chars17h7ea02ef
+  0x0000dc60 66666533 62326131 65450061 6e6f6e2e ffe3b2a1eE.anon.
+  0x0000dc70 65396562 32333763 66353061 34336236 e9eb237cf50a43b6
+  0x0000dc80 35643633 36623066 34373730 62303465 5d636b0f4770b04e
+  0x0000dc90 2e32372e 6c6c766d 2e313338 36313835 .27.llvm.1386185
+  0x0000dca0 32373131 33393032 37343736 005f5a4e 271139027476._ZN
+  0x0000dcb0 3470796f 33336769 6c313572 65676973 4pyo33gil15regis
+  0x0000dcc0 7465725f 64656372 65663137 68363333 ter_decref17h633
+  0x0000dcd0 66393438 63343964 36386364 3745005f f948c49d68cd7E._
+  0x0000dce0 5a4e3731 5f244c54 24727573 74635f64 ZN71_$LT$rustc_d
+  0x0000dcf0 656d616e 676c652e 2e6c6567 6163792e emangle..legacy.
+  0x0000dd00 2e44656d 616e676c 65247532 30246173 .Demangle$u20$as
+  0x0000dd10 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000dd20 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x0000dd30 37683261 39633235 32316639 38656561 7h2a9c2521f98eea
+  0x0000dd40 66634500 5f5a4e34 345f244c 54242452 fcE._ZN44_$LT$$R
+  0x0000dd50 46245424 75323024 61732475 32302463 F$T$u20$as$u20$c
+  0x0000dd60 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x0000dd70 79244754 2433666d 74313768 38653230 y$GT$3fmt17h8e20
+  0x0000dd80 33656139 37646530 31626465 45005f5a 3ea97de01bdeE._Z
+  0x0000dd90 4e34636f 72653970 616e6963 6b696e67 N4core9panicking
+  0x0000dda0 31337061 6e69635f 64697370 6c617931 13panic_display1
+  0x0000ddb0 37683065 35326632 64346461 37666332 7h0e52f2d4da7fc2
+  0x0000ddc0 3131452e 6c6c766d 2e313833 35363735 11E.llvm.1835675
+  0x0000ddd0 30343835 36313435 31333132 39005f5f 0485614513129.__
+  0x0000dde0 72757374 5f70726f 62657374 61636b00 rust_probestack.
+  0x0000ddf0 5f5a4e37 365f244c 54247079 6f332e2e _ZN76_$LT$pyo3..
+  0x0000de00 65786365 7074696f 6e732e2e 50794e6f exceptions..PyNo
+  0x0000de10 74496d70 6c656d65 6e746564 4572726f tImplementedErro
+  0x0000de20 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
+  0x0000de30 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
+  0x0000de40 2433666d 74313768 36626162 39626263 $3fmt17h6bab9bbc
+  0x0000de50 37376630 32656230 45005f5a 4e347079 77f02eb0E._ZN4py
+  0x0000de60 6f333131 74797065 5f6f626a 65637431 o311type_object1
+  0x0000de70 30507954 79706549 6e666f31 31747970 0PyTypeInfo11typ
+  0x0000de80 655f6f62 6a656374 31376863 64366364 e_object17hcd6cd
+  0x0000de90 66653930 61616165 30356445 005f5a4e fe90aaae05dE._ZN
+  0x0000dea0 36395f24 4c542470 796f332e 2e657863 69_$LT$pyo3..exc
+  0x0000deb0 65707469 6f6e732e 2e507942 79746573 eptions..PyBytes
+  0x0000dec0 5761726e 696e6724 75323024 61732475 Warning$u20$as$u
+  0x0000ded0 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x0000dee0 62756724 47542433 666d7431 37683231 bug$GT$3fmt17h21
+  0x0000def0 31313664 61313233 38376435 31624500 116da12387d51bE.
+  0x0000df00 616e6f6e 2e396531 31346564 35303130 anon.9e114ed5010
+  0x0000df10 64363235 33626432 36313132 39343733 d6253bd261129473
+  0x0000df20 63643138 382e312e 6c6c766d 2e383336 cd188.1.llvm.836
+  0x0000df30 34373335 31373237 30333437 36333534 4735172703476354
+  0x0000df40 005f5a4e 3470796f 3335696d 706c5f31 ._ZN4pyo35impl_1
+  0x0000df50 36657874 72616374 5f617267 756d656e 6extract_argumen
+  0x0000df60 74313665 78747261 63745f61 7267756d t16extract_argum
+  0x0000df70 656e7431 37683336 33653334 34336639 ent17h363e3443f9
+  0x0000df80 35333439 30374500 5f5f474e 555f4548 534907E.__GNU_EH
+  0x0000df90 5f465241 4d455f48 4452005f 5a4e366f _FRAME_HDR._ZN6o
+  0x0000dfa0 626a6563 7433656c 66313245 4c465f4e bject3elf12ELF_N
+  0x0000dfb0 4f54455f 474e5531 37686661 34303936 OTE_GNU17hfa4096
+  0x0000dfc0 62336634 62373162 36644500 5f5a4e34 b3f4b71b6dE._ZN4
+  0x0000dfd0 636f7265 33666d74 336e756d 33696d70 core3fmt3num3imp
+  0x0000dfe0 35345f24 4c542469 6d706c24 75323024 54_$LT$impl$u20$
+  0x0000dff0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
+  0x0000e000 61792475 32302466 6f722475 32302475 ay$u20$for$u20$u
+  0x0000e010 73697a65 24475424 33666d74 31376833 size$GT$3fmt17h3
+  0x0000e020 37396637 39393634 65646365 64323945 79f79964edced29E
+  0x0000e030 005f5a4e 34636f72 65337074 72343264 ._ZN4core3ptr42d
+  0x0000e040 726f705f 696e5f70 6c616365 244c5424 rop_in_place$LT$
+  0x0000e050 616c6c6f 632e2e73 7472696e 672e2e53 alloc..string..S
+  0x0000e060 7472696e 67244754 24313768 61646139 tring$GT$17hada9
+  0x0000e070 37616330 65653866 64333563 452e6c6c 7ac0ee8fd35cE.ll
+  0x0000e080 766d2e35 36393739 32393736 39313333 vm.5697929769133
+  0x0000e090 30353734 3736005f 5a4e3470 796f3331 057476._ZN4pyo31
+  0x0000e0a0 31636f6e 76657273 696f6e73 33737464 1conversions3std
+  0x0000e0b0 336e756d 36345f24 4c542469 6d706c24 3num64_$LT$impl$
+  0x0000e0c0 75323024 70796f33 2e2e636f 6e766572 u20$pyo3..conver
+  0x0000e0d0 73696f6e 2e2e4672 6f6d5079 4f626a65 sion..FromPyObje
+  0x0000e0e0 63742475 32302466 6f722475 32302475 ct$u20$for$u20$u
+  0x0000e0f0 33322447 54243765 78747261 63743137 32$GT$7extract17
+  0x0000e100 68653339 30323233 32326238 62653330 he39022322b8be30
+  0x0000e110 38450061 6e6f6e2e 37623934 36616531 8E.anon.7b946ae1
+  0x0000e120 64336136 36363739 37653264 62316633 d3a666797e2db1f3
+  0x0000e130 36653463 64366537 2e382e6c 6c766d2e 6e4cd6e7.8.llvm.
+  0x0000e140 31383335 36373530 34383536 31343531 1835675048561451
+  0x0000e150 33313239 005f6669 6e69005f 5a4e3634 3129._fini._ZN64
+  0x0000e160 5f244c54 24737464 2e2e7379 732e2e75 _$LT$std..sys..u
+  0x0000e170 6e69782e 2e737464 696f2e2e 53746465 nix..stdio..Stde
+  0x0000e180 72722475 32302461 73247532 30247374 rr$u20$as$u20$st
+  0x0000e190 642e2e69 6f2e2e57 72697465 24475424 d..io..Write$GT$
+  0x0000e1a0 35666c75 73683137 68316134 34616530 5flush17h1a44ae0
+  0x0000e1b0 34626436 66343463 3045005f 5a4e3136 4bd6f44c0E._ZN16
+  0x0000e1c0 7061726b 696e675f 6c6f745f 636f7265 parking_lot_core
+  0x0000e1d0 31317061 726b696e 675f6c6f 74313054 11parking_lot10T
+  0x0000e1e0 68726561 64446174 61336e65 77313768 hreadData3new17h
+  0x0000e1f0 65333130 63613230 39633638 66323361 e310ca209c68f23a
+  0x0000e200 45005f5a 4e37315f 244c5424 70796f33 E._ZN71_$LT$pyo3
+  0x0000e210 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x0000e220 52756e74 696d6557 61726e69 6e672475 RuntimeWarning$u
+  0x0000e230 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x0000e240 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
+  0x0000e250 6d743137 68306366 32616531 30346364 mt17h0cf2ae104cd
+  0x0000e260 63303764 64450044 572e7265 662e7275 c07ddE.DW.ref.ru
+  0x0000e270 73745f65 685f7065 72736f6e 616c6974 st_eh_personalit
+  0x0000e280 79005f5a 4e34636f 7265336f 70733866 y._ZN4core3ops8f
+  0x0000e290 756e6374 696f6e36 466e4f6e 63653430 unction6FnOnce40
+  0x0000e2a0 63616c6c 5f6f6e63 65247537 62242475 call_once$u7b$$u
+  0x0000e2b0 37622476 7461626c 652e7368 696d2475 7b$vtable.shim$u
+  0x0000e2c0 37642424 75376424 31376832 32306163 7d$$u7d$17h220ac
+  0x0000e2d0 33383135 66666332 63376445 2e6c6c76 3815ffc2c7dE.llv
+  0x0000e2e0 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x0000e2f0 38313132 33005f5a 4e34636f 72653366 81123._ZN4core3f
+  0x0000e300 6d743862 75696c64 65727339 44656275 mt8builders9Debu
+  0x0000e310 674c6973 7435656e 74727931 37686239 gList5entry17hb9
+  0x0000e320 66666636 62306331 31343035 31624500 fff6b0c114051bE.
+  0x0000e330 5f5a4e35 616c6c6f 63337665 63313656 _ZN5alloc3vec16V
+  0x0000e340 6563244c 54245424 43244124 47542431 ec$LT$T$C$A$GT$1
+  0x0000e350 36696e74 6f5f626f 7865645f 736c6963 6into_boxed_slic
+  0x0000e360 65313768 37316534 34336266 34653837 e17h71e443bf4e87
+  0x0000e370 36633932 45005f5f 72646c5f 616c6c6f 6c92E.__rdl_allo
+  0x0000e380 63005f5a 4e34636f 7265336f 70733866 c._ZN4core3ops8f
+  0x0000e390 756e6374 696f6e36 466e4f6e 63653430 unction6FnOnce40
+  0x0000e3a0 63616c6c 5f6f6e63 65247537 62242475 call_once$u7b$$u
+  0x0000e3b0 37622476 7461626c 652e7368 696d2475 7b$vtable.shim$u
+  0x0000e3c0 37642424 75376424 31376865 66613165 7d$$u7d$17hefa1e
+  0x0000e3d0 33653339 36306430 34373845 2e6c6c76 3e3960d0478E.llv
+  0x0000e3e0 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x0000e3f0 38313132 33006673 74617436 34005f5a 81123.fstat64._Z
+  0x0000e400 4e337374 64367468 72656164 356c6f63 N3std6thread5loc
+  0x0000e410 616c3466 61737431 324b6579 244c5424 al4fast12Key$LT$
+  0x0000e420 54244754 24313474 72795f69 6e697469 T$GT$14try_initi
+  0x0000e430 616c697a 65313768 34303537 30363065 alize17h4057060e
+  0x0000e440 33363831 35386434 452e6c6c 766d2e31 368158d4E.llvm.1
+  0x0000e450 31343939 39373739 39393837 30343439 1499977999870449
+  0x0000e460 31363100 5f5a4e38 315f244c 54247079 161._ZN81_$LT$py
+  0x0000e470 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x0000e480 5079436f 6e6e6563 74696f6e 41626f72 PyConnectionAbor
+  0x0000e490 74656445 72726f72 24753230 24617324 tedError$u20$as$
+  0x0000e4a0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x0000e4b0 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
+  0x0000e4c0 68636466 36383965 38346438 33303533 hcdf689e84d83053
+  0x0000e4d0 3145005f 5a4e3638 5f244c54 2470796f 1E._ZN68_$LT$pyo
+  0x0000e4e0 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x0000e4f0 79537973 74656d45 72726f72 24753230 ySystemError$u20
+  0x0000e500 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x0000e510 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x0000e520 31376836 35343838 32316362 34396633 17h6548821cb49f3
+  0x0000e530 34636145 005f5a4e 34636f72 6533666d 4caE._ZN4core3fm
+  0x0000e540 7439466f 726d6174 74657231 35646562 t9Formatter15deb
+  0x0000e550 75675f75 70706572 5f686578 31376834 ug_upper_hex17h4
+  0x0000e560 61653561 64346636 66326161 31643045 ae5ad4f6f2aa1d0E
+  0x0000e570 005f5a4e 38305f24 4c542473 74642e2e ._ZN80_$LT$std..
+  0x0000e580 696f2e2e 57726974 652e2e77 72697465 io..Write..write
+  0x0000e590 5f666d74 2e2e4164 61707465 72244c54 _fmt..Adapter$LT
+  0x0000e5a0 24542447 54242475 32302461 73247532 $T$GT$$u20$as$u2
+  0x0000e5b0 3024636f 72652e2e 666d742e 2e577269 0$core..fmt..Wri
+  0x0000e5c0 74652447 54243977 72697465 5f737472 te$GT$9write_str
+  0x0000e5d0 31376861 39626534 36373639 63336238 17ha9be46769c3b8
+  0x0000e5e0 35366645 005f5a4e 37335f24 4c542470 56fE._ZN73_$LT$p
+  0x0000e5f0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x0000e600 2e507952 756e7469 6d655761 726e696e .PyRuntimeWarnin
+  0x0000e610 67247532 30246173 24753230 24636f72 g$u20$as$u20$cor
+  0x0000e620 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
+  0x0000e630 47542433 666d7431 37683961 36653338 GT$3fmt17h9a6e38
+  0x0000e640 62303735 65333539 33384500 5f5a4e34 b075e35938E._ZN4
+  0x0000e650 70796f33 33657272 39657272 5f737461 pyo33err9err_sta
+  0x0000e660 74653130 626f7865 645f6172 67733137 te10boxed_args17
+  0x0000e670 68333462 37383138 33376565 37386361 h34b781837ee78ca
+  0x0000e680 37450061 6e6f6e2e 39653131 34656435 7E.anon.9e114ed5
+  0x0000e690 30313064 36323533 62643236 31313239 010d6253bd261129
+  0x0000e6a0 34373363 64313838 2e322e6c 6c766d2e 473cd188.2.llvm.
+  0x0000e6b0 38333634 37333531 37323730 33343736 8364735172703476
+  0x0000e6c0 33353400 616e6f6e 2e653931 33366434 354.anon.e9136d4
+  0x0000e6d0 63633266 32626637 33336435 39326235 cc2f2bf733d592b5
+  0x0000e6e0 64663838 39353230 372e322e 6c6c766d df8895207.2.llvm
+  0x0000e6f0 2e313733 36383735 34323430 34363830 .173687542404680
+  0x0000e700 33333536 30005f5a 4e347079 6f333574 33560._ZN4pyo35t
+  0x0000e710 79706573 36737472 696e6738 50795374 ypes6string8PySt
+  0x0000e720 72696e67 336e6577 31376832 39393935 ring3new17h29995
+  0x0000e730 39656464 34303332 31613245 005f5a4e 9edd40321a2E._ZN
+  0x0000e740 36395f24 4c542463 6f72652e 2e616c6c 69_$LT$core..all
+  0x0000e750 6f632e2e 6c61796f 75742e2e 4c61796f oc..layout..Layo
+  0x0000e760 75744572 726f7224 75323024 61732475 utError$u20$as$u
+  0x0000e770 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x0000e780 62756724 47542433 666d7431 37683035 bug$GT$3fmt17h05
+  0x0000e790 66633930 34353661 33373535 31664500 fc90456a37551fE.
+  0x0000e7a0 5f5a4e37 325f244c 54242452 46247374 _ZN72_$LT$$RF$st
+  0x0000e7b0 72247532 30246173 24753230 24616c6c r$u20$as$u20$all
+  0x0000e7c0 6f632e2e 6666692e 2e635f73 74722e2e oc..ffi..c_str..
+  0x0000e7d0 43537472 696e672e 2e6e6577 2e2e5370 CString..new..Sp
+  0x0000e7e0 65634e65 77496d70 6c244754 24313373 ecNewImpl$GT$13s
+  0x0000e7f0 7065635f 6e65775f 696d706c 31376834 pec_new_impl17h4
+  0x0000e800 66363363 62663535 64613663 39626645 f63cbf55da6c9bfE
+  0x0000e810 005f5a4e 34636f72 6535736c 69636532 ._ZN4core5slice2
+  0x0000e820 395f244c 5424696d 706c2475 32302424 9_$LT$impl$u20$$
+  0x0000e830 75356224 54247535 64242447 54243135 u5b$T$u5d$$GT$15
+  0x0000e840 636f7079 5f66726f 6d5f736c 69636531 copy_from_slice1
+  0x0000e850 376c656e 5f6d6973 6d617463 685f6661 7len_mismatch_fa
+  0x0000e860 696c3137 68353734 31383430 34313032 il17h57418404102
+  0x0000e870 37616665 6545005f 5a4e3634 5f244c54 7afeeE._ZN64_$LT
+  0x0000e880 24737464 2e2e7379 732e2e75 6e69782e $std..sys..unix.
+  0x0000e890 2e737464 696f2e2e 53746465 72722475 .stdio..Stderr$u
+  0x0000e8a0 32302461 73247532 30247374 642e2e69 20$as$u20$std..i
+  0x0000e8b0 6f2e2e57 72697465 24475424 35777269 o..Write$GT$5wri
+  0x0000e8c0 74653137 68626335 34316163 61396138 te17hbc541aca9a8
+  0x0000e8d0 33393532 3545005f 5a4e3470 796f3334 39525E._ZN4pyo34
+  0x0000e8e0 73796e63 32304749 4c4f6e63 6543656c sync20GILOnceCel
+  0x0000e8f0 6c244c54 24542447 54243469 6e697431 l$LT$T$GT$4init1
+  0x0000e900 37686637 35396636 66623261 39656138 7hf759f6fb2a9ea8
+  0x0000e910 64354500 5f5a4e34 70796f33 3367696c d5E._ZN4pyo33gil
+  0x0000e920 31347265 67697374 65725f6f 776e6564 14register_owned
+  0x0000e930 31376865 30373638 31636161 66303331 17he07681caaf031
+  0x0000e940 61383845 005f5a4e 37325f24 4c542470 a88E._ZN72_$LT$p
+  0x0000e950 796f332e 2e747970 65732e2e 62797465 yo3..types..byte
+  0x0000e960 61727261 792e2e50 79427974 65417272 array..PyByteArr
+  0x0000e970 61792475 32302461 73247532 3024636f ay$u20$as$u20$co
+  0x0000e980 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x0000e990 54243366 6d743137 68396564 36393439 T$3fmt17h9ed6949
+  0x0000e9a0 39323164 37663734 3045005f 5a4e3136 921d7f740E._ZN16
+  0x0000e9b0 7061726b 696e675f 6c6f745f 636f7265 parking_lot_core
+  0x0000e9c0 39776f72 645f6c6f 636b3857 6f72644c 9word_lock8WordL
+  0x0000e9d0 6f636b39 6c6f636b 5f736c6f 77313768 ock9lock_slow17h
+  0x0000e9e0 61383738 35623030 64643266 63366434 a8785b00dd2fc6d4
+  0x0000e9f0 45005f5a 4e36315f 244c5424 7374642e E._ZN61_$LT$std.
+  0x0000ea00 2e696f2e 2e737464 696f2e2e 53746465 .io..stdio..Stde
+  0x0000ea10 72724c6f 636b2475 32302461 73247532 rrLock$u20$as$u2
+  0x0000ea20 30247374 642e2e69 6f2e2e57 72697465 0$std..io..Write
+  0x0000ea30 24475424 39777269 74655f61 6c6c3137 $GT$9write_all17
+  0x0000ea40 68333534 61376434 34396631 30316631 h354a7d449f101f1
+  0x0000ea50 3045005f 5a4e3561 6c6c6f63 33666d74 0E._ZN5alloc3fmt
+  0x0000ea60 36666f72 6d617431 32666f72 6d61745f 6format12format_
+  0x0000ea70 696e6e65 72313768 62386137 63633965 inner17hb8a7cc9e
+  0x0000ea80 61643634 64663932 45005f5a 4e36345f ad64df92E._ZN64_
+  0x0000ea90 244c5424 616c6c6f 632e2e66 66692e2e $LT$alloc..ffi..
+  0x0000eaa0 635f7374 722e2e4e 756c4572 726f7224 c_str..NulError$
+  0x0000eab0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x0000eac0 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x0000ead0 666d7431 37683332 30363831 30316161 fmt17h32068101aa
+  0x0000eae0 65353437 34394500 5f5a4e34 636f7265 e54749E._ZN4core
+  0x0000eaf0 33666d74 38627569 6c646572 73313144 3fmt8builders11D
+  0x0000eb00 65627567 53747275 63743666 696e6973 ebugStruct6finis
+  0x0000eb10 68313768 32363834 62623465 62373333 h17h2684bb4eb733
+  0x0000eb20 62386265 45007275 73745f70 616e6963 b8beE.rust_panic
+  0x0000eb30 005f5a4e 31347275 7374635f 64656d61 ._ZN14rustc_dema
+  0x0000eb40 6e676c65 3844656d 616e676c 65366173 ngle8Demangle6as
+  0x0000eb50 5f737472 31376837 61633965 35363238 _str17h7ac9e5628
+  0x0000eb60 64666532 37623445 005f5a4e 39315f24 dfe27b4E._ZN91_$
+  0x0000eb70 4c542473 74642e2e 70616e69 636b696e LT$std..panickin
+  0x0000eb80 672e2e62 6567696e 5f70616e 69632e2e g..begin_panic..
+  0x0000eb90 50616e69 63506179 6c6f6164 244c5424 PanicPayload$LT$
+  0x0000eba0 41244754 24247532 30246173 24753230 A$GT$$u20$as$u20
+  0x0000ebb0 24636f72 652e2e70 616e6963 2e2e426f $core..panic..Bo
+  0x0000ebc0 784d6555 70244754 24336765 74313768 xMeUp$GT$3get17h
+  0x0000ebd0 37373135 34623061 34376230 32663035 77154b0a47b02f05
+  0x0000ebe0 45005f5a 4e34636f 72653366 6d743946 E._ZN4core3fmt9F
+  0x0000ebf0 6f726d61 74746572 39616c74 65726e61 ormatter9alterna
+  0x0000ec00 74653137 68316133 38303564 31313362 te17h1a3805d113b
+  0x0000ec10 39303037 6645005f 5a4e3336 5f244c54 9007fE._ZN36_$LT
+  0x0000ec20 24542475 32302461 73247532 3024636f $T$u20$as$u20$co
+  0x0000ec30 72652e2e 616e792e 2e416e79 24475424 re..any..Any$GT$
+  0x0000ec40 37747970 655f6964 31376833 62323235 7type_id17h3b225
+  0x0000ec50 36656166 35623264 38363445 005f5a4e 6eaf5b2d864E._ZN
+  0x0000ec60 34636f72 65337074 72373064 726f705f 4core3ptr70drop_
+  0x0000ec70 696e5f70 6c616365 244c5424 70796f33 in_place$LT$pyo3
+  0x0000ec80 2e2e696e 7374616e 63652e2e 5079244c ..instance..Py$L
+  0x0000ec90 54247079 6f332e2e 74797065 732e2e61 T$pyo3..types..a
+  0x0000eca0 6e792e2e 5079416e 79244754 24244754 ny..PyAny$GT$$GT
+  0x0000ecb0 24313768 38636562 61363264 62623038 $17h8ceba62dbb08
+  0x0000ecc0 34653861 452e6c6c 766d2e31 31393430 4e8aE.llvm.11940
+  0x0000ecd0 36323133 36373536 30363632 38303500 621367560662805.
+  0x0000ece0 5f5a4e33 73746433 73797334 756e6978 _ZN3std3sys4unix
+  0x0000ecf0 32667331 3263616e 6f6e6963 616c697a 2fs12canonicaliz
+  0x0000ed00 65313768 62623761 39373765 61333539 e17hbb7a977ea359
+  0x0000ed10 36383036 45005f5a 4e36375f 244c5424 6806E._ZN67_$LT$
+  0x0000ed20 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x0000ed30 2e2e5079 454f4645 72726f72 24753230 ..PyEOFError$u20
+  0x0000ed40 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x0000ed50 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x0000ed60 6d743137 68363633 30316364 62353164 mt17h66301cdb51d
+  0x0000ed70 31343463 64450061 6e6f6e2e 33343764 144cdE.anon.347d
+  0x0000ed80 32363465 33346562 33613063 37346265 264e34eb3a0c74be
+  0x0000ed90 35613839 66383935 61633765 2e31382e 5a89f895ac7e.18.
+  0x0000eda0 6c6c766d 2e313736 39353736 32333431 llvm.17695762341
+  0x0000edb0 37383134 35333031 32005f5a 4e347079 781453012._ZN4py
+  0x0000edc0 6f333574 79706573 31307479 70656f62 o35types10typeob
+  0x0000edd0 6a656374 36507954 79706534 6e616d65 ject6PyType4name
+  0x0000ede0 31376865 65623335 61633939 33336434 17heeb35ac9933d4
+  0x0000edf0 38306445 005f5a4e 37385f24 4c542470 80dE._ZN78_$LT$p
+  0x0000ee00 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x0000ee10 2e617379 6e63696f 2e2e4361 6e63656c .asyncio..Cancel
+  0x0000ee20 6c656445 72726f72 24753230 24617324 ledError$u20$as$
+  0x0000ee30 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x0000ee40 65627567 24475424 33666d74 31376839 ebug$GT$3fmt17h9
+  0x0000ee50 39613034 35303865 65646237 65623245 9a04508eedb7eb2E
+  0x0000ee60 005f5a4e 3470796f 33357479 70657335 ._ZN4pyo35types5
+  0x0000ee70 7475706c 65313337 5f244c54 24696d70 tuple137_$LT$imp
+  0x0000ee80 6c247532 30247079 6f332e2e 636f6e76 l$u20$pyo3..conv
+  0x0000ee90 65727369 6f6e2e2e 496e746f 5079244c ersion..IntoPy$L
+  0x0000eea0 54247079 6f332e2e 696e7374 616e6365 T$pyo3..instance
+  0x0000eeb0 2e2e5079 244c5424 70796f33 2e2e7479 ..Py$LT$pyo3..ty
+  0x0000eec0 7065732e 2e616e79 2e2e5079 416e7924 pes..any..PyAny$
+  0x0000eed0 47542424 47542424 75323024 666f7224 GT$$GT$$u20$for$
+  0x0000eee0 75323024 244c5024 54302443 24543124 u20$$LP$T0$C$T1$
+  0x0000eef0 43245432 24432454 33245250 24244754 C$T2$C$T3$RP$$GT
+  0x0000ef00 2437696e 746f5f70 79313768 37376663 $7into_py17h77fc
+  0x0000ef10 38643365 38663630 32356332 4500616e 8d3e8f6025c2E.an
+  0x0000ef20 6f6e2e39 65313134 65643530 31306436 on.9e114ed5010d6
+  0x0000ef30 32353362 64323631 31323934 37336364 253bd261129473cd
+  0x0000ef40 3138382e 332e6c6c 766d2e38 33363437 188.3.llvm.83647
+  0x0000ef50 33353137 32373033 34373633 3534005f 35172703476354._
+  0x0000ef60 5a4e3463 6f726539 70616e69 636b696e ZN4core9panickin
+  0x0000ef70 67313970 616e6963 5f63616e 6e6f745f g19panic_cannot_
+  0x0000ef80 756e7769 6e643137 68643132 33643963 unwind17hd123d9c
+  0x0000ef90 37313437 33646364 6145005f 5a4e3537 71473dcdaE._ZN57
+  0x0000efa0 5f244c54 24636f72 652e2e66 6d742e2e _$LT$core..fmt..
+  0x0000efb0 466f726d 61747465 72247532 30246173 Formatter$u20$as
+  0x0000efc0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000efd0 57726974 65244754 24397772 6974655f Write$GT$9write_
+  0x0000efe0 73747231 37683331 37633462 65626232 str17h317c4bebb2
+  0x0000eff0 39376634 30314500 5f5a4e34 70796f33 97f401E._ZN4pyo3
+  0x0000f000 33657272 35507945 7272386e 65775f74 3err5PyErr8new_t
+  0x0000f010 79706531 37686164 35633331 61356364 ype17had5c31a5cd
+  0x0000f020 31306533 38304500 5f474c4f 42414c5f 10e380E._GLOBAL_
+  0x0000f030 4f464653 45545f54 41424c45 5f00616e OFFSET_TABLE_.an
+  0x0000f040 6f6e2e65 39656232 33376366 35306134 on.e9eb237cf50a4
+  0x0000f050 33623635 64363336 62306634 37373062 3b65d636b0f4770b
+  0x0000f060 3034652e 33322e6c 6c766d2e 31333836 04e.32.llvm.1386
+  0x0000f070 31383532 37313133 39303237 34373600 185271139027476.
+  0x0000f080 5f5a4e34 70796f33 31317479 70655f6f _ZN4pyo311type_o
+  0x0000f090 626a6563 74313050 79547970 65496e66 bject10PyTypeInf
+  0x0000f0a0 6f313174 7970655f 6f626a65 63743137 o11type_object17
+  0x0000f0b0 68313466 35633735 65373436 38623339 h14f5c75e7468b39
+  0x0000f0c0 3145005f 5a4e3638 5f244c54 2470796f 1E._ZN68_$LT$pyo
+  0x0000f0d0 332e2e74 79706573 2e2e7479 70656f62 3..types..typeob
+  0x0000f0e0 6a656374 2e2e5079 54797065 24753230 ject..PyType$u20
+  0x0000f0f0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x0000f100 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x0000f110 31376833 31356438 38613537 34363133 17h315d88a574613
+  0x0000f120 31333945 005f5a4e 33737464 33737973 139E._ZN3std3sys
+  0x0000f130 34756e69 78313461 626f7274 5f696e74 4unix14abort_int
+  0x0000f140 65726e61 6c313768 65623237 65616365 ernal17heb27eace
+  0x0000f150 65363666 62383466 45005f5a 4e34636f e66fb84fE._ZN4co
+  0x0000f160 7265336e 756d3632 5f244c54 24696d70 re3num62_$LT$imp
+  0x0000f170 6c247532 3024636f 72652e2e 7374722e l$u20$core..str.
+  0x0000f180 2e747261 6974732e 2e46726f 6d537472 .traits..FromStr
+  0x0000f190 24753230 24666f72 24753230 24757369 $u20$for$u20$usi
+  0x0000f1a0 7a652447 54243866 726f6d5f 73747231 ze$GT$8from_str1
+  0x0000f1b0 37683633 30646439 30333965 35343633 7h630dd9039e5463
+  0x0000f1c0 64384500 5f5a4e34 345f244c 54242452 d8E._ZN44_$LT$$R
+  0x0000f1d0 46245424 75323024 61732475 32302463 F$T$u20$as$u20$c
+  0x0000f1e0 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x0000f1f0 79244754 2433666d 74313768 34656330 y$GT$3fmt17h4ec0
+  0x0000f200 39643732 63366463 31393339 45005f5a 9d72c6dc1939E._Z
+  0x0000f210 4e37325f 244c5424 636f7265 2e2e6e75 N72_$LT$core..nu
+  0x0000f220 6d2e2e65 72726f72 2e2e5472 7946726f m..error..TryFro
+  0x0000f230 6d496e74 4572726f 72247532 30246173 mIntError$u20$as
+  0x0000f240 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x0000f250 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x0000f260 37683138 36333934 37366334 31336165 7h18639476c413ae
+  0x0000f270 39664500 5f5a4e36 305f244c 5424616c 9fE._ZN60_$LT$al
+  0x0000f280 6c6f632e 2e737472 696e672e 2e537472 loc..string..Str
+  0x0000f290 696e6724 75323024 61732475 32302463 ing$u20$as$u20$c
+  0x0000f2a0 6f72652e 2e636c6f 6e652e2e 436c6f6e ore..clone..Clon
+  0x0000f2b0 65244754 2435636c 6f6e6531 37686430 e$GT$5clone17hd0
+  0x0000f2c0 30306434 62643335 35373932 35644500 00d4bd3557925dE.
+  0x0000f2d0 5f5a4e34 70796f33 35747970 65733361 _ZN4pyo35types3a
+  0x0000f2e0 6e793550 79416e79 37736574 61747472 ny5PyAny7setattr
+  0x0000f2f0 31376836 62383338 62363761 33663836 17h6b838b67a3f86
+  0x0000f300 33363145 005f5a4e 33737464 3770726f 361E._ZN3std7pro
+  0x0000f310 63657373 3561626f 72743137 68366135 cess5abort17h6a5
+  0x0000f320 37333166 38316438 32666436 3345005f 731f81d82fd63E._
+  0x0000f330 5a4e3561 6c6c6f63 3473796e 63333261 ZN5alloc4sync32a
+  0x0000f340 7263696e 6e65725f 6c61796f 75745f66 rcinner_layout_f
+  0x0000f350 6f725f76 616c7565 5f6c6179 6f757431 or_value_layout1
+  0x0000f360 37683239 65626461 66383335 39353736 7h29ebdaf8359576
+  0x0000f370 35344500 5f5a4e33 73746434 74696d65 54E._ZN3std4time
+  0x0000f380 37496e73 74616e74 336e6f77 31376837 7Instant3now17h7
+  0x0000f390 62313336 39636339 66633435 33643945 b1369cc9fc453d9E
+  0x0000f3a0 00616e6f 6e2e3334 37643236 34653334 .anon.347d264e34
+  0x0000f3b0 65623361 30633734 62653561 38396638 eb3a0c74be5a89f8
+  0x0000f3c0 39356163 37652e31 2e6c6c76 6d2e3137 95ac7e.1.llvm.17
+  0x0000f3d0 36393537 36323334 31373831 34353330 6957623417814530
+  0x0000f3e0 3132005f 5a4e3373 74643373 79733475 12._ZN3std3sys4u
+  0x0000f3f0 6e697831 37646563 6f64655f 6572726f nix17decode_erro
+  0x0000f400 725f6b69 6e643137 68326164 30326437 r_kind17h2ad02d7
+  0x0000f410 30373865 34396331 3045005f 5a4e3463 078e49c10E._ZN4c
+  0x0000f420 6f726533 70747234 3764726f 705f696e ore3ptr47drop_in
+  0x0000f430 5f706c61 6365244c 5424636f 72652e2e _place$LT$core..
+  0x0000f440 63656c6c 2e2e426f 72726f77 4d757445 cell..BorrowMutE
+  0x0000f450 72726f72 24475424 31376862 64653830 rror$GT$17hbde80
+  0x0000f460 65616663 62376563 30326245 2e6c6c76 eafcb7ec02bE.llv
+  0x0000f470 6d2e3137 36393537 36323334 31373831 m.17695762341781
+  0x0000f480 34353330 3132005f 5a4e3470 796f3335 453012._ZN4pyo35
+  0x0000f490 74797065 73357475 706c6531 32375f24 types5tuple127_$
+  0x0000f4a0 4c542469 6d706c24 75323024 70796f33 LT$impl$u20$pyo3
+  0x0000f4b0 2e2e636f 6e766572 73696f6e 2e2e496e ..conversion..In
+  0x0000f4c0 746f5079 244c5424 70796f33 2e2e696e toPy$LT$pyo3..in
+  0x0000f4d0 7374616e 63652e2e 5079244c 54247079 stance..Py$LT$py
+  0x0000f4e0 6f332e2e 74797065 732e2e61 6e792e2e o3..types..any..
+  0x0000f4f0 5079416e 79244754 24244754 24247532 PyAny$GT$$GT$$u2
+  0x0000f500 3024666f 72247532 3024244c 50245430 0$for$u20$$LP$T0
+  0x0000f510 24432454 31245250 24244754 2437696e $C$T1$RP$$GT$7in
+  0x0000f520 746f5f70 79313768 33383132 38323035 to_py17h38128205
+  0x0000f530 34353338 37356135 45005f5a 4e36395f 453875a5E._ZN69_
+  0x0000f540 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x0000f550 696f6e73 2e2e5079 56616c75 65457272 ions..PyValueErr
+  0x0000f560 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x0000f570 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
+  0x0000f580 24475424 33666d74 31376838 31356439 $GT$3fmt17h815d9
+  0x0000f590 64343039 35393030 33656445 00616e6f d40959003edE.ano
+  0x0000f5a0 6e2e6239 61303438 36633030 61343137 n.b9a0486c00a417
+  0x0000f5b0 32623762 31616335 32623331 35616134 2b7b1ac52b315aa4
+  0x0000f5c0 61332e34 312e6c6c 766d2e31 33323338 a3.41.llvm.13238
+  0x0000f5d0 38393334 33323230 30363932 32323600 893432200692226.
+  0x0000f5e0 5f5a4e35 335f244c 54245424 75323024 _ZN53_$LT$T$u20$
+  0x0000f5f0 61732475 32302470 796f332e 2e636f6e as$u20$pyo3..con
+  0x0000f600 76657273 696f6e2e 2e46726f 6d507950 version..FromPyP
+  0x0000f610 6f696e74 65722447 54243231 66726f6d ointer$GT$21from
+  0x0000f620 5f6f776e 65645f70 74725f6f 725f6f70 _owned_ptr_or_op
+  0x0000f630 74313768 39343766 62303365 64363262 t17h947fb03ed62b
+  0x0000f640 31346337 452e6c6c 766d2e31 33323338 14c7E.llvm.13238
+  0x0000f650 38393334 33323230 30363932 32323600 893432200692226.
+  0x0000f660 5f5a4e37 315f244c 54247079 6f332e2e _ZN71_$LT$pyo3..
+  0x0000f670 65786365 7074696f 6e732e2e 50795275 exceptions..PyRu
+  0x0000f680 6e74696d 65457272 6f722475 32302461 ntimeError$u20$a
+  0x0000f690 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x0000f6a0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x0000f6b0 31376833 62323566 66333331 61396164 17h3b25ff331a9ad
+  0x0000f6c0 32373345 005f5a4e 34636f72 65337074 273E._ZN4core3pt
+  0x0000f6d0 72373664 726f705f 696e5f70 6c616365 r76drop_in_place
+  0x0000f6e0 244c5424 70796f33 2e2e696e 7374616e $LT$pyo3..instan
+  0x0000f6f0 63652e2e 5079244c 54247079 6f332e2e ce..Py$LT$pyo3..
+  0x0000f700 74797065 732e2e73 7472696e 672e2e50 types..string..P
+  0x0000f710 79537472 696e6724 47542424 47542431 yString$GT$$GT$1
+  0x0000f720 37686333 33393736 38376233 30643139 7hc3397687b30d19
+  0x0000f730 3333452e 6c6c766d 2e313132 31333838 33E.llvm.1121388
+  0x0000f740 39373633 36303536 33333439 33005f5a 9763605633493._Z
+  0x0000f750 4e36385f 244c5424 70796f33 2e2e6578 N68_$LT$pyo3..ex
+  0x0000f760 63657074 696f6e73 2e2e5079 55736572 ceptions..PyUser
+  0x0000f770 5761726e 696e6724 75323024 61732475 Warning$u20$as$u
+  0x0000f780 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x0000f790 62756724 47542433 666d7431 37683032 bug$GT$3fmt17h02
+  0x0000f7a0 61646161 65613963 62326536 34364500 adaaea9cb2e646E.
+  0x0000f7b0 5f5a4e34 636f7265 33666d74 336e756d _ZN4core3fmt3num
+  0x0000f7c0 35335f24 4c542469 6d706c24 75323024 53_$LT$impl$u20$
+  0x0000f7d0 636f7265 2e2e666d 742e2e55 70706572 core..fmt..Upper
+  0x0000f7e0 48657824 75323024 666f7224 75323024 Hex$u20$for$u20$
+  0x0000f7f0 75363424 47542433 666d7431 37683039 u64$GT$3fmt17h09
+  0x0000f800 62643862 63636636 34313830 33304500 bd8bccf6418030E.
+  0x0000f810 5f5a4e34 70796f33 35747970 6573346c _ZN4pyo35types4l
+  0x0000f820 69737436 50794c69 73743661 7070656e ist6PyList6appen
+  0x0000f830 64313768 33616632 36393433 34376265 d17h3af2694347be
+  0x0000f840 33396566 45005f5a 4e38305f 244c5424 39efE._ZN80_$LT$
+  0x0000f850 7374642e 2e706174 682e2e43 6f6d706f std..path..Compo
+  0x0000f860 6e656e74 73247532 30246173 24753230 nents$u20$as$u20
+  0x0000f870 24636f72 652e2e69 7465722e 2e747261 $core..iter..tra
+  0x0000f880 6974732e 2e697465 7261746f 722e2e49 its..iterator..I
+  0x0000f890 74657261 746f7224 47542434 6e657874 terator$GT$4next
+  0x0000f8a0 31376864 31663235 66613430 35353532 17hd1f25fa405552
+  0x0000f8b0 36613545 00616e6f 6e2e3639 62366439 6a5E.anon.69b6d9
+  0x0000f8c0 36633863 36356437 39343933 33313539 6c8c65d794933159
+  0x0000f8d0 64356662 39313433 39622e31 332e6c6c d5fb91439b.13.ll
+  0x0000f8e0 766d2e35 36383036 33373436 32323735 vm.5680637462275
+  0x0000f8f0 35333837 3632005f 5a4e3470 796f3335 538762._ZN4pyo35
+  0x0000f900 696d706c 5f313665 78747261 63745f61 impl_16extract_a
+  0x0000f910 7267756d 656e7431 3946756e 6374696f rgument19Functio
+  0x0000f920 6e446573 63726970 74696f6e 33346d69 nDescription34mi
+  0x0000f930 7373696e 675f7265 71756972 65645f6b ssing_required_k
+  0x0000f940 6579776f 72645f61 7267756d 656e7473 eyword_arguments
+  0x0000f950 31376839 61616338 32366137 64663739 17h9aac826a7df79
+  0x0000f960 34633145 005f5a4e 34636f72 65397061 4c1E._ZN4core9pa
+  0x0000f970 6e69636b 696e6731 3470616e 69635f6e nicking14panic_n
+  0x0000f980 6f756e77 696e6431 37683365 62336139 ounwind17h3eb3a9
+  0x0000f990 36626565 39656532 34324500 5f5f7275 6bee9ee242E.__ru
+  0x0000f9a0 73745f64 726f705f 70616e69 63005f5a st_drop_panic._Z
+  0x0000f9b0 4e37385f 244c5424 70796f33 2e2e6578 N78_$LT$pyo3..ex
+  0x0000f9c0 63657074 696f6e73 2e2e5079 4e6f7449 ceptions..PyNotI
+  0x0000f9d0 6d706c65 6d656e74 65644572 726f7224 mplementedError$
+  0x0000f9e0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x0000f9f0 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
+  0x0000fa00 2433666d 74313768 36393532 65363865 $3fmt17h6952e68e
+  0x0000fa10 66383739 66616465 45005f5a 4e347079 f879fadeE._ZN4py
+  0x0000fa20 6f333569 6d706c5f 31366578 74726163 o35impl_16extrac
+  0x0000fa30 745f6172 67756d65 6e743139 46756e63 t_argument19Func
+  0x0000fa40 74696f6e 44657363 72697074 696f6e32 tionDescription2
+  0x0000fa50 386d756c 7469706c 655f7661 6c756573 8multiple_values
+  0x0000fa60 5f666f72 5f617267 756d656e 74313768 _for_argument17h
+  0x0000fa70 31646430 38306137 63643564 63393031 1dd080a7cd5dc901
+  0x0000fa80 45005f5a 4e347079 6f333574 79706573 E._ZN4pyo35types
+  0x0000fa90 366d6f64 756c6538 50794d6f 64756c65 6module8PyModule
+  0x0000faa0 31326164 645f6675 6e637469 6f6e3137 12add_function17
+  0x0000fab0 68636138 63663935 66626133 61636161 hca8cf95fba3acaa
+  0x0000fac0 6545005f 5a4e3935 5f244c54 24737464 eE._ZN95_$LT$std
+  0x0000fad0 2e2e7061 74682e2e 436f6d70 6f6e656e ..path..Componen
+  0x0000fae0 74732475 32302461 73247532 3024636f ts$u20$as$u20$co
+  0x0000faf0 72652e2e 69746572 2e2e7472 61697473 re..iter..traits
+  0x0000fb00 2e2e646f 75626c65 5f656e64 65642e2e ..double_ended..
+  0x0000fb10 446f7562 6c65456e 64656449 74657261 DoubleEndedItera
+  0x0000fb20 746f7224 47542439 6e657874 5f626163 tor$GT$9next_bac
+  0x0000fb30 6b313768 30386534 65393631 39386432 k17h08e4e96198d2
+  0x0000fb40 39363233 45005f5a 4e37345f 244c5424 9623E._ZN74_$LT$
+  0x0000fb50 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x0000fb60 2e2e5079 46696c65 45786973 74734572 ..PyFileExistsEr
+  0x0000fb70 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x0000fb80 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x0000fb90 79244754 2433666d 74313768 32303538 y$GT$3fmt17h2058
+  0x0000fba0 66336438 66306535 36663765 45005f5a f3d8f0e56f7eE._Z
+  0x0000fbb0 4e36345f 244c5424 7374642e 2e706174 N64_$LT$std..pat
+  0x0000fbc0 682e2e53 74726970 50726566 69784572 h..StripPrefixEr
+  0x0000fbd0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x0000fbe0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x0000fbf0 47542433 666d7431 37683265 36343133 GT$3fmt17h2e6413
+  0x0000fc00 65393833 31313731 38614500 5f5a4e31 e98311718aE._ZN1
+  0x0000fc10 32305f24 4c542470 796f332e 2e646572 20_$LT$pyo3..der
+  0x0000fc20 6976655f 7574696c 732e2e50 7946756e ive_utils..PyFun
+  0x0000fc30 6374696f 6e417267 756d656e 74732475 ctionArguments$u
+  0x0000fc40 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x0000fc50 636f6e76 6572742e 2e46726f 6d244c54 convert..From$LT
+  0x0000fc60 24245246 2470796f 332e2e74 79706573 $$RF$pyo3..types
+  0x0000fc70 2e2e6d6f 64756c65 2e2e5079 4d6f6475 ..module..PyModu
+  0x0000fc80 6c652447 54242447 54243466 726f6d31 le$GT$$GT$4from1
+  0x0000fc90 37683064 31353536 63656132 64636236 7h0d1556cea2dcb6
+  0x0000fca0 39364500 5f5a4e37 305f244c 54247079 96E._ZN70_$LT$py
+  0x0000fcb0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x0000fcc0 50795374 6f704974 65726174 696f6e24 PyStopIteration$
+  0x0000fcd0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x0000fce0 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x0000fcf0 666d7431 37683535 35313738 37366134 fmt17h55517876a4
+  0x0000fd00 38316465 61384500 5f5a4e34 636f7265 81dea8E._ZN4core
+  0x0000fd10 33707472 31313164 726f705f 696e5f70 3ptr111drop_in_p
+  0x0000fd20 6c616365 244c5424 70796f33 2e2e6572 lace$LT$pyo3..er
+  0x0000fd30 722e2e65 72725f73 74617465 2e2e626f r..err_state..bo
+  0x0000fd40 7865645f 61726773 244c5424 616c6c6f xed_args$LT$allo
+  0x0000fd50 632e2e73 7472696e 672e2e53 7472696e c..string..Strin
+  0x0000fd60 67244754 242e2e24 75376224 24753762 g$GT$..$u7b$$u7b
+  0x0000fd70 24636c6f 73757265 24753764 24247537 $closure$u7d$$u7
+  0x0000fd80 64242447 54243137 68336539 61643964 d$$GT$17h3e9ad9d
+  0x0000fd90 38316261 32613837 37452e6c 6c766d2e 81ba2a877E.llvm.
+  0x0000fda0 33313630 39303732 38313838 30373831 3160907281880781
+  0x0000fdb0 31323300 5f5a4e35 67696d6c 69347265 123._ZN5gimli4re
+  0x0000fdc0 61643661 62627265 76313341 62627265 ad6abbrev13Abbre
+  0x0000fdd0 76696174 696f6e73 36696e73 65727431 viations6insert1
+  0x0000fde0 37683061 37323933 66356535 35623335 7h0a7293f5e55b35
+  0x0000fdf0 35384500 5f5a4e34 636f7265 3570616e 58E._ZN4core5pan
+  0x0000fe00 69633130 70616e69 635f696e 666f3950 ic10panic_info9P
+  0x0000fe10 616e6963 496e666f 376d6573 73616765 anicInfo7message
+  0x0000fe20 31376836 63663565 38376364 34616434 17h6cf5e87cd4ad4
+  0x0000fe30 35363645 005f5a4e 34636f72 6533666d 566E._ZN4core3fm
+  0x0000fe40 7439466f 726d6174 74657233 70616431 t9Formatter3pad1
+  0x0000fe50 37686535 30316233 64393766 65656464 7he501b3d97feedd
+  0x0000fe60 30664500 5f5a4e39 385f244c 5424616c 0fE._ZN98_$LT$al
+  0x0000fe70 6c6f632e 2e766563 2e2e5665 63244c54 loc..vec..Vec$LT
+  0x0000fe80 24542447 54242475 32302461 73247532 $T$GT$$u20$as$u2
+  0x0000fe90 3024616c 6c6f632e 2e766563 2e2e7370 0$alloc..vec..sp
+  0x0000fea0 65635f66 726f6d5f 69746572 2e2e5370 ec_from_iter..Sp
+  0x0000feb0 65634672 6f6d4974 6572244c 54245424 ecFromIter$LT$T$
+  0x0000fec0 43244924 47542424 47542439 66726f6d C$I$GT$$GT$9from
+  0x0000fed0 5f697465 72313768 62363634 61376237 _iter17hb664a7b7
+  0x0000fee0 65626562 34643333 45005f5a 4e35616c ebeb4d33E._ZN5al
+  0x0000fef0 6c6f6335 616c6c6f 6338626f 785f6672 loc5alloc8box_fr
+  0x0000ff00 65653137 68393832 65623666 62353665 ee17h982eb6fb56e
+  0x0000ff10 61386639 36452e6c 6c766d2e 38333634 a8f96E.llvm.8364
+  0x0000ff20 37333531 37323730 33343736 33353400 735172703476354.
+  0x0000ff30 5f5a4e38 305f244c 54247079 6f332e2e _ZN80_$LT$pyo3..
+  0x0000ff40 65786365 7074696f 6e732e2e 5079556e exceptions..PyUn
+  0x0000ff50 69636f64 65547261 6e736c61 74654572 icodeTranslateEr
+  0x0000ff60 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x0000ff70 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x0000ff80 79244754 2433666d 74313768 31303735 y$GT$3fmt17h1075
+  0x0000ff90 37363338 31633961 31636362 4500616e 76381c9a1ccbE.an
+  0x0000ffa0 6f6e2e35 31303562 64643739 66323362 on.5105bdd79f23b
+  0x0000ffb0 31313731 66333837 34326665 61616335 1171f38742feaac5
+  0x0000ffc0 6431372e 34312e6c 6c766d2e 33313630 d17.41.llvm.3160
+  0x0000ffd0 39303732 38313838 30373831 31323300 907281880781123.
+  0x0000ffe0 5f5a4e34 70796f33 33657272 39657272 _ZN4pyo33err9err
+  0x0000fff0 5f737461 74653130 50794572 72537461 _state10PyErrSta
+  0x00010000 74653134 696e746f 5f666669 5f747570 te14into_ffi_tup
+  0x00010010 6c653137 68353164 35643265 34656537 le17h51d5d2e4ee7
+  0x00010020 35336235 3645005f 5a4e3637 5f244c54 53b56E._ZN67_$LT
+  0x00010030 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x00010040 732e2e50 79537973 74656d45 78697424 s..PySystemExit$
+  0x00010050 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x00010060 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x00010070 666d7431 37683735 31613732 66653366 fmt17h751a72fe3f
+  0x00010080 61393263 38614500 5f5a4e37 345f244c a92c8aE._ZN74_$L
+  0x00010090 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x000100a0 6e732e2e 50794172 6974686d 65746963 ns..PyArithmetic
+  0x000100b0 4572726f 72247532 30246173 24753230 Error$u20$as$u20
+  0x000100c0 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
+  0x000100d0 6c617924 47542433 666d7431 37686233 lay$GT$3fmt17hb3
+  0x000100e0 38303736 62616233 35633032 34644500 8076bab35c024dE.
+  0x000100f0 5f5a4e35 335f244c 5424636f 72652e2e _ZN53_$LT$core..
+  0x00010100 666d742e 2e457272 6f722475 32302461 fmt..Error$u20$a
+  0x00010110 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00010120 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x00010130 68626636 30653366 31366238 65323565 hbf60e3f16b8e25e
+  0x00010140 3445005f 5a4e3634 5f244c54 24636f72 4E._ZN64_$LT$cor
+  0x00010150 652e2e73 74722e2e 6572726f 722e2e55 e..str..error..U
+  0x00010160 74663845 72726f72 24753230 24617324 tf8Error$u20$as$
+  0x00010170 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x00010180 65627567 24475424 33666d74 31376837 ebug$GT$3fmt17h7
+  0x00010190 34616562 66316261 33333166 65323045 4aebf1ba331fe20E
+  0x000101a0 005f5a4e 3470796f 3335696d 706c5f39 ._ZN4pyo35impl_9
+  0x000101b0 70796d65 74686f64 73313665 78747261 pymethods16extra
+  0x000101c0 63745f63 5f737472 696e6731 37686435 ct_c_string17hd5
+  0x000101d0 64356665 33323731 66663132 3738452e d5fe3271ff1278E.
+  0x000101e0 6c6c766d 2e353639 37393239 37363931 llvm.56979297691
+  0x000101f0 33333035 37343736 005f5a4e 36395f24 33057476._ZN69_$
+  0x00010200 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
+  0x00010210 6f6e732e 2e507952 756e7469 6d654572 ons..PyRuntimeEr
+  0x00010220 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x00010230 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x00010240 47542433 666d7431 37686632 31643938 GT$3fmt17hf21d98
+  0x00010250 65383231 62643533 38344500 5f5a4e34 e821bd5384E._ZN4
+  0x00010260 636f7265 33666d74 336e756d 35325f24 core3fmt3num52_$
+  0x00010270 4c542469 6d706c24 75323024 636f7265 LT$impl$u20$core
+  0x00010280 2e2e666d 742e2e4c 6f776572 48657824 ..fmt..LowerHex$
+  0x00010290 75323024 666f7224 75323024 69382447 u20$for$u20$i8$G
+  0x000102a0 54243366 6d743137 68366630 61353232 T$3fmt17h6f0a522
+  0x000102b0 64333332 31646234 3845005f 5a4e3636 d3321db48E._ZN66
+  0x000102c0 5f244c54 2470796f 332e2e74 79706573 _$LT$pyo3..types
+  0x000102d0 2e2e7374 72696e67 2e2e5079 53747269 ..string..PyStri
+  0x000102e0 6e672475 32302461 73247532 3024636f ng$u20$as$u20$co
+  0x000102f0 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x00010300 54243366 6d743137 68656132 34616637 T$3fmt17hea24af7
+  0x00010310 37663965 33613333 3145005f 5a4e3470 7f9e3a331E._ZN4p
+  0x00010320 796f3333 67696c34 504f4f4c 31376837 yo33gil4POOL17h7
+  0x00010330 39326465 30643561 62666266 65623745 92de0d5abfbfeb7E
+  0x00010340 00616e6f 6e2e6239 61303438 36633030 .anon.b9a0486c00
+  0x00010350 61343137 32623762 31616335 32623331 a4172b7b1ac52b31
+  0x00010360 35616134 61332e35 322e6c6c 766d2e31 5aa4a3.52.llvm.1
+  0x00010370 33323338 38393334 33323230 30363932 3238893432200692
+  0x00010380 32323600 5f5f7275 73745f64 65616c6c 226.__rust_deall
+  0x00010390 6f630061 6e6f6e2e 35313035 62646437 oc.anon.5105bdd7
+  0x000103a0 39663233 62313137 31663338 37343266 9f23b1171f38742f
+  0x000103b0 65616163 35643137 2e33392e 6c6c766d eaac5d17.39.llvm
+  0x000103c0 2e333136 30393037 32383138 38303738 .316090728188078
+  0x000103d0 31313233 005f5a4e 38315f24 4c542470 1123._ZN81_$LT$p
+  0x000103e0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x000103f0 2e617379 6e63696f 2e2e496e 76616c69 .asyncio..Invali
+  0x00010400 64537461 74654572 726f7224 75323024 dStateError$u20$
+  0x00010410 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00010420 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
+  0x00010430 37683435 63386634 66616362 62323565 7h45c8f4facbb25e
+  0x00010440 38324500 616e6f6e 2e353130 35626464 82E.anon.5105bdd
+  0x00010450 37396632 33623131 37316633 38373432 79f23b1171f38742
+  0x00010460 66656161 63356431 372e3338 2e6c6c76 feaac5d17.38.llv
+  0x00010470 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x00010480 38313132 33005f5a 4e36365f 244c5424 81123._ZN66_$LT$
+  0x00010490 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x000104a0 2e2e5079 45786365 7074696f 6e247532 ..PyException$u2
+  0x000104b0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x000104c0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x000104d0 74313768 39623938 33633830 31373039 t17h9b983c801709
+  0x000104e0 32663930 4500616e 6f6e2e62 39613034 2f90E.anon.b9a04
+  0x000104f0 38366330 30613431 37326237 62316163 86c00a4172b7b1ac
+  0x00010500 35326233 31356161 3461332e 33342e6c 52b315aa4a3.34.l
+  0x00010510 6c766d2e 31333233 38383933 34333232 lvm.132388934322
+  0x00010520 30303639 32323236 005f5a4e 3470796f 00692226._ZN4pyo
+  0x00010530 33357479 70657334 6c697374 3650794c 35types4list6PyL
+  0x00010540 69737433 6c656e31 37683666 39646336 ist3len17h6f9dc6
+  0x00010550 63653534 38386634 31324500 5f5a4e34 ce5488f412E._ZN4
+  0x00010560 636f7265 33707472 31323564 726f705f core3ptr125drop_
+  0x00010570 696e5f70 6c616365 244c5424 70796f33 in_place$LT$pyo3
+  0x00010580 2e2e6572 722e2e65 72725f73 74617465 ..err..err_state
+  0x00010590 2e2e626f 7865645f 61726773 244c5424 ..boxed_args$LT$
+  0x000105a0 636f7265 2e2e6e75 6d2e2e64 65633266 core..num..dec2f
+  0x000105b0 6c742e2e 50617273 65466c6f 61744572 lt..ParseFloatEr
+  0x000105c0 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
+  0x000105d0 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
+  0x000105e0 75376424 24475424 31376838 65323239 u7d$$GT$17h8e229
+  0x000105f0 64386537 39333038 62303345 2e6c6c76 d8e79308b03E.llv
+  0x00010600 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x00010610 38313132 33005f5a 4e34636f 72653366 81123._ZN4core3f
+  0x00010620 6d743946 6f726d61 74746572 31316465 mt9Formatter11de
+  0x00010630 6275675f 7475706c 65313768 34373962 bug_tuple17h479b
+  0x00010640 34366533 35353261 65386332 45005f5a 46e3552ae8c2E._Z
+  0x00010650 4e36385f 244c5424 7374642e 2e746872 N68_$LT$std..thr
+  0x00010660 6561642e 2e6c6f63 616c2e2e 41636365 ead..local..Acce
+  0x00010670 73734572 726f7224 75323024 61732475 ssError$u20$as$u
+  0x00010680 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x00010690 62756724 47542433 666d7431 37683366 bug$GT$3fmt17h3f
+  0x000106a0 35396563 38353634 34343431 65644500 59ec85644441edE.
+  0x000106b0 616e6f6e 2e623961 30343836 63303061 anon.b9a0486c00a
+  0x000106c0 34313732 62376231 61633532 62333135 4172b7b1ac52b315
+  0x000106d0 61613461 332e3337 2e6c6c76 6d2e3133 aa4a3.37.llvm.13
+  0x000106e0 32333838 39333433 32323030 36393232 2388934322006922
+  0x000106f0 3236005f 5a4e3463 6f726533 70747231 26._ZN4core3ptr1
+  0x00010700 33326472 6f705f69 6e5f706c 61636524 32drop_in_place$
+  0x00010710 4c542463 6f72652e 2e63656c 6c2e2e52 LT$core..cell..R
+  0x00010720 65664d75 74244c54 24616c6c 6f632e2e efMut$LT$alloc..
+  0x00010730 7665632e 2e566563 244c5424 636f7265 vec..Vec$LT$core
+  0x00010740 2e2e7074 722e2e6e 6f6e5f6e 756c6c2e ..ptr..non_null.
+  0x00010750 2e4e6f6e 4e756c6c 244c5424 70796f33 .NonNull$LT$pyo3
+  0x00010760 5f666669 2e2e6f62 6a656374 2e2e5079 _ffi..object..Py
+  0x00010770 4f626a65 63742447 54242447 54242447 Object$GT$$GT$$G
+  0x00010780 54242447 54243137 68373366 30656563 T$$GT$17h73f0eec
+  0x00010790 35626361 35396162 33452e6c 6c766d2e 5bca59ab3E.llvm.
+  0x000107a0 31333233 38383933 34333232 30303639 1323889343220069
+  0x000107b0 32323236 005f5a4e 37305f24 4c542463 2226._ZN70_$LT$c
+  0x000107c0 6f72652e 2e70616e 69632e2e 6c6f6361 ore..panic..loca
+  0x000107d0 74696f6e 2e2e4c6f 63617469 6f6e2475 tion..Location$u
+  0x000107e0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x000107f0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x00010800 33666d74 31376866 63613138 33363561 3fmt17hfca18365a
+  0x00010810 64623434 34626345 005f5a4e 33737464 db444bcE._ZN3std
+  0x00010820 3970616e 69636b69 6e673131 62656769 9panicking11begi
+  0x00010830 6e5f7061 6e696331 37686364 61336532 n_panic17hcda3e2
+  0x00010840 38633435 38336635 32304500 5f5a4e37 8c4583f520E._ZN7
+  0x00010850 345f244c 54247079 6f332e2e 65786365 4_$LT$pyo3..exce
+  0x00010860 7074696f 6e732e2e 5079436f 6e6e6563 ptions..PyConnec
+  0x00010870 74696f6e 4572726f 72247532 30246173 tionError$u20$as
+  0x00010880 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00010890 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x000108a0 37683530 62313836 38316466 36396530 7h50b18681df69e0
+  0x000108b0 32634500 616e6f6e 2e653965 62323337 2cE.anon.e9eb237
+  0x000108c0 63663530 61343362 36356436 33366230 cf50a43b65d636b0
+  0x000108d0 66343737 30623034 652e3132 2e6c6c76 f4770b04e.12.llv
+  0x000108e0 6d2e3133 38363138 35323731 31333930 m.13861852711390
+  0x000108f0 32373437 36005f5a 4e38375f 244c5424 27476._ZN87_$LT$
+  0x00010900 636f7265 2e2e7374 722e2e6c 6f737379 core..str..lossy
+  0x00010910 2e2e5574 66384368 756e6b73 24753230 ..Utf8Chunks$u20
+  0x00010920 24617324 75323024 636f7265 2e2e6974 $as$u20$core..it
+  0x00010930 65722e2e 74726169 74732e2e 69746572 er..traits..iter
+  0x00010940 61746f72 2e2e4974 65726174 6f722447 ator..Iterator$G
+  0x00010950 5424346e 65787431 37683838 39353163 T$4next17h88951c
+  0x00010960 63643566 66306438 38624500 5f5a4e37 cd5ff0d88bE._ZN7
+  0x00010970 375f244c 54247079 6f332e2e 65786365 7_$LT$pyo3..exce
+  0x00010980 7074696f 6e732e2e 5079466c 6f617469 ptions..PyFloati
+  0x00010990 6e67506f 696e7445 72726f72 24753230 ngPointError$u20
+  0x000109a0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x000109b0 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x000109c0 6d743137 68333263 38323864 64393231 mt17h32c828dd921
+  0x000109d0 32306162 3345005f 5a4e3634 5f244c54 20ab3E._ZN64_$LT
+  0x000109e0 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x000109f0 732e2e50 794f5345 72726f72 24753230 s..PyOSError$u20
+  0x00010a00 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00010a10 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x00010a20 31376864 37653534 66313762 34303131 17hd7e54f17b4011
+  0x00010a30 35393745 005f5f72 7573745f 616c6c6f 597E.__rust_allo
+  0x00010a40 635f7a65 726f6564 005f5a4e 34636f72 c_zeroed._ZN4cor
+  0x00010a50 65337074 72373564 726f705f 696e5f70 e3ptr75drop_in_p
+  0x00010a60 6c616365 244c5424 636f7265 2e2e7265 lace$LT$core..re
+  0x00010a70 73756c74 2e2e5265 73756c74 244c5424 sult..Result$LT$
+  0x00010a80 24524624 73747224 43247079 6f332e2e $RF$str$C$pyo3..
+  0x00010a90 6572722e 2e507945 72722447 54242447 err..PyErr$GT$$G
+  0x00010aa0 54243137 68383339 62303764 32386335 T$17h839b07d28c5
+  0x00010ab0 30646431 35452e6c 6c766d2e 31333233 0dd15E.llvm.1323
+  0x00010ac0 38383933 34333232 30303639 32323236 8893432200692226
+  0x00010ad0 005f5a4e 37335f24 4c542470 796f332e ._ZN73_$LT$pyo3.
+  0x00010ae0 2e657863 65707469 6f6e732e 2e507941 .exceptions..PyA
+  0x00010af0 73736572 74696f6e 4572726f 72247532 ssertionError$u2
+  0x00010b00 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00010b10 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
+  0x00010b20 666d7431 37686530 35616636 64316436 fmt17he05af6d1d6
+  0x00010b30 64363632 30354500 5f5a4e34 636f7265 d66205E._ZN4core
+  0x00010b40 33666d74 39466f72 6d617474 65723132 3fmt9Formatter12
+  0x00010b50 64656275 675f7374 72756374 31376866 debug_struct17hf
+  0x00010b60 38646436 36383935 34666565 34333245 8dd668954fee432E
+  0x00010b70 00616e6f 6e2e6539 31333664 34636332 .anon.e9136d4cc2
+  0x00010b80 66326266 37333364 35393262 35646638 f2bf733d592b5df8
+  0x00010b90 38393532 30372e35 2e6c6c76 6d2e3137 895207.5.llvm.17
+  0x00010ba0 33363837 35343234 30343638 30333335 3687542404680335
+  0x00010bb0 36300061 6e6f6e2e 36383266 30353362 60.anon.682f053b
+  0x00010bc0 61336436 64313461 66356232 37636663 a3d6d14af5b27cfc
+  0x00010bd0 62626431 36333633 2e312e6c 6c766d2e bbd16363.1.llvm.
+  0x00010be0 35363937 39323937 36393133 33303537 5697929769133057
+  0x00010bf0 34373600 5f5a4e35 305f244c 54242452 476._ZN50_$LT$$R
+  0x00010c00 46246d75 74247532 30245724 75323024 F$mut$u20$W$u20$
+  0x00010c10 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00010c20 2e2e5772 69746524 47542431 30777269 ..Write$GT$10wri
+  0x00010c30 74655f63 68617231 37683937 32336364 te_char17h9723cd
+  0x00010c40 35373635 63343532 3864452e 6c6c766d 5765c4528dE.llvm
+  0x00010c50 2e333034 31333933 39353835 36393937 .304139395856997
+  0x00010c60 34333439 005f5a4e 36395f24 4c542470 4349._ZN69_$LT$p
+  0x00010c70 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00010c80 2e507949 6e646578 4572726f 72247532 .PyIndexError$u2
+  0x00010c90 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00010ca0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
+  0x00010cb0 666d7431 37683663 66396162 35343938 fmt17h6cf9ab5498
+  0x00010cc0 65613135 30394500 5f5a4e37 355f244c ea1509E._ZN75_$L
+  0x00010cd0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x00010ce0 6e732e2e 5079456e 7669726f 6e6d656e ns..PyEnvironmen
+  0x00010cf0 74457272 6f722475 32302461 73247532 tError$u20$as$u2
+  0x00010d00 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00010d10 706c6179 24475424 33666d74 31376863 play$GT$3fmt17hc
+  0x00010d20 64346236 39623165 65363566 33356645 d4b69b1ee65f35fE
+  0x00010d30 00616e6f 6e2e6239 61303438 36633030 .anon.b9a0486c00
+  0x00010d40 61343137 32623762 31616335 32623331 a4172b7b1ac52b31
+  0x00010d50 35616134 61332e33 322e6c6c 766d2e31 5aa4a3.32.llvm.1
+  0x00010d60 33323338 38393334 33323230 30363932 3238893432200692
+  0x00010d70 32323600 616e6f6e 2e376239 34366165 226.anon.7b946ae
+  0x00010d80 31643361 36363637 39376532 64623166 1d3a666797e2db1f
+  0x00010d90 33366534 63643665 372e3333 2e6c6c76 36e4cd6e7.33.llv
+  0x00010da0 6d2e3138 33353637 35303438 35363134 m.18356750485614
+  0x00010db0 35313331 3239005f 5a4e3131 7061726b 513129._ZN11park
+  0x00010dc0 696e675f 6c6f7439 7261775f 6d757465 ing_lot9raw_mute
+  0x00010dd0 78385261 774d7574 6578396c 6f636b5f x8RawMutex9lock_
+  0x00010de0 736c6f77 31376830 38333865 62633832 slow17h0838ebc82
+  0x00010df0 32656130 32666645 005f5a4e 36395f24 2ea02ffE._ZN69_$
+  0x00010e00 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
+  0x00010e10 6f6e732e 2e507953 79737465 6d457869 ons..PySystemExi
+  0x00010e20 74247532 30246173 24753230 24636f72 t$u20$as$u20$cor
+  0x00010e30 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
+  0x00010e40 47542433 666d7431 37686466 30636231 GT$3fmt17hdf0cb1
+  0x00010e50 63303662 31346439 30354500 5f5a4e34 c06b14d905E._ZN4
+  0x00010e60 636f7265 336f7073 3866756e 6374696f core3ops8functio
+  0x00010e70 6e36466e 4f6e6365 34306361 6c6c5f6f n6FnOnce40call_o
+  0x00010e80 6e636524 75376224 24753762 24767461 nce$u7b$$u7b$vta
+  0x00010e90 626c652e 7368696d 24753764 24247537 ble.shim$u7d$$u7
+  0x00010ea0 64243137 68636465 30623030 33356536 d$17hcde0b0035e6
+  0x00010eb0 63386265 65452e6c 6c766d2e 31333233 c8beeE.llvm.1323
+  0x00010ec0 38383933 34333232 30303639 32323236 8893432200692226
+  0x00010ed0 005f5a4e 34636f72 65397061 6e69636b ._ZN4core9panick
+  0x00010ee0 696e6731 33617373 6572745f 6661696c ing13assert_fail
+  0x00010ef0 65643137 68663961 37343734 66663431 ed17hf9a7474ff41
+  0x00010f00 66333833 6545005f 5a4e3731 5f244c54 f383eE._ZN71_$LT
+  0x00010f10 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x00010f20 732e2e50 79556e69 636f6465 5761726e s..PyUnicodeWarn
+  0x00010f30 696e6724 75323024 61732475 32302463 ing$u20$as$u20$c
+  0x00010f40 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x00010f50 47542433 666d7431 37683831 39306536 GT$3fmt17h8190e6
+  0x00010f60 36306137 38623161 30324500 5f5a4e39 60a78b1a02E._ZN9
+  0x00010f70 61646472 326c696e 65397061 74685f70 addr2line9path_p
+  0x00010f80 75736831 37683262 64636238 35386430 ush17h2bdcb858d0
+  0x00010f90 66316465 64394500 5f5a4e34 636f7265 f1ded9E._ZN4core
+  0x00010fa0 33666d74 39466f72 6d617474 65723130 3fmt9Formatter10
+  0x00010fb0 64656275 675f6c69 73743137 68396632 debug_list17h9f2
+  0x00010fc0 66323861 39373332 66663337 3845005f f28a9732ff378E._
+  0x00010fd0 5a4e3463 6f726533 666d7439 466f726d ZN4core3fmt9Form
+  0x00010fe0 61747465 72323564 65627567 5f747570 atter25debug_tup
+  0x00010ff0 6c655f66 69656c64 325f6669 6e697368 le_field2_finish
+  0x00011000 31376835 39633861 35336462 64656332 17h59c8a53dbdec2
+  0x00011010 63323745 00616e6f 6e2e3638 32663035 c27E.anon.682f05
+  0x00011020 33626133 64366431 34616635 62323763 3ba3d6d14af5b27c
+  0x00011030 66636262 64313633 36332e34 302e6c6c fcbbd16363.40.ll
+  0x00011040 766d2e35 36393739 32393736 39313333 vm.5697929769133
+  0x00011050 30353734 3736005f 5a4e3463 6f726533 057476._ZN4core3
+  0x00011060 70747233 3764726f 705f696e 5f706c61 ptr37drop_in_pla
+  0x00011070 6365244c 5424636f 72652e2e 666d742e ce$LT$core..fmt.
+  0x00011080 2e457272 6f722447 54243137 68653230 .Error$GT$17he20
+  0x00011090 63633361 36386336 31626231 39452e6c cc3a68c61bb19E.l
+  0x000110a0 6c766d2e 35363937 39323937 36393133 lvm.569792976913
+  0x000110b0 33303537 34373600 5f5a4e34 636f7265 3057476._ZN4core
+  0x000110c0 33707472 31303864 726f705f 696e5f70 3ptr108drop_in_p
+  0x000110d0 6c616365 244c5424 70796f33 2e2e6572 lace$LT$pyo3..er
+  0x000110e0 722e2e65 72725f73 74617465 2e2e626f r..err_state..bo
+  0x000110f0 7865645f 61726773 244c5424 244c5024 xed_args$LT$$LP$
+  0x00011100 24524624 73747224 43242452 50242447 $RF$str$C$$RP$$G
+  0x00011110 54242e2e 24753762 24247537 6224636c T$..$u7b$$u7b$cl
+  0x00011120 6f737572 65247537 64242475 37642424 osure$u7d$$u7d$$
+  0x00011130 47542431 37686161 35393266 61356636 GT$17haa592fa5f6
+  0x00011140 36393738 3064452e 6c6c766d 2e333136 69780dE.llvm.316
+  0x00011150 30393037 32383138 38303738 31313233 0907281880781123
+  0x00011160 005f5a4e 37325f24 4c542470 796f332e ._ZN72_$LT$pyo3.
+  0x00011170 2e657863 65707469 6f6e732e 2e507953 .exceptions..PyS
+  0x00011180 796e7461 78576172 6e696e67 24753230 yntaxWarning$u20
+  0x00011190 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x000111a0 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x000111b0 6d743137 68333831 61646536 31313161 mt17h381ade6111a
+  0x000111c0 36613939 3645005f 5a4e3731 5f244c54 6a996E._ZN71_$LT
+  0x000111d0 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x000111e0 732e2e50 79417474 72696275 74654572 s..PyAttributeEr
+  0x000111f0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x00011200 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x00011210 47542433 666d7431 37683635 63636661 GT$3fmt17h65ccfa
+  0x00011220 34636437 63396661 62634500 5f5a4e36 4cd7c9fabcE._ZN6
+  0x00011230 345f244c 54247374 642e2e73 79732e2e 4_$LT$std..sys..
+  0x00011240 756e6978 2e2e7374 64696f2e 2e537464 unix..stdio..Std
+  0x00011250 65727224 75323024 61732475 32302473 err$u20$as$u20$s
+  0x00011260 74642e2e 696f2e2e 57726974 65244754 td..io..Write$GT
+  0x00011270 24313477 72697465 5f766563 746f7265 $14write_vectore
+  0x00011280 64313768 32373931 35373463 30303536 d17h2791574c0056
+  0x00011290 36316666 45005f5a 4e36385f 244c5424 61ffE._ZN68_$LT$
+  0x000112a0 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x000112b0 2e2e5079 4c6f6f6b 75704572 726f7224 ..PyLookupError$
+  0x000112c0 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x000112d0 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x000112e0 666d7431 37683831 63333762 66336236 fmt17h81c37bf3b6
+  0x000112f0 64373130 35314500 5f5a4e33 73746434 d71051E._ZN3std4
+  0x00011300 70617468 34506174 68376973 5f66696c path4Path7is_fil
+  0x00011310 65313768 61306630 32376236 66323737 e17ha0f027b6f277
+  0x00011320 36363865 45005f5a 4e36315f 244c5424 668eE._ZN61_$LT$
+  0x00011330 24524624 7374642e 2e696f2e 2e737464 $RF$std..io..std
+  0x00011340 696f2e2e 53746465 72722475 32302461 io..Stderr$u20$a
+  0x00011350 73247532 30247374 642e2e69 6f2e2e57 s$u20$std..io..W
+  0x00011360 72697465 24475424 39777269 74655f66 rite$GT$9write_f
+  0x00011370 6d743137 68353366 31376236 34613132 mt17h53f17b64a12
+  0x00011380 66613964 6245005f 5a4e3373 74643970 fa9dbE._ZN3std9p
+  0x00011390 616e6963 6b696e67 32307275 73745f70 anicking20rust_p
+  0x000113a0 616e6963 5f776974 685f686f 6f6b3137 anic_with_hook17
+  0x000113b0 68353063 30396430 30306463 35363164 h50c09d000dc561d
+  0x000113c0 3245005f 5a4e3463 6f726533 666d7433 2E._ZN4core3fmt3
+  0x000113d0 6e756d33 696d7035 325f244c 5424696d num3imp52_$LT$im
+  0x000113e0 706c2475 32302463 6f72652e 2e666d74 pl$u20$core..fmt
+  0x000113f0 2e2e4469 73706c61 79247532 3024666f ..Display$u20$fo
+  0x00011400 72247532 30247536 34244754 2433666d r$u20$u64$GT$3fm
+  0x00011410 74313768 61623733 38626537 33633762 t17hab738be73c7b
+  0x00011420 37633836 45005f5a 4e34636f 72653366 7c86E._ZN4core3f
+  0x00011430 6d743130 41726775 6d656e74 56313130 mt10ArgumentV110
+  0x00011440 66726f6d 5f757369 7a653137 68616561 from_usize17haea
+  0x00011450 65383365 36383330 31363161 3145005f e83e6830161a1E._
+  0x00011460 5a4e3463 6f726533 70747232 30356472 ZN4core3ptr205dr
+  0x00011470 6f705f69 6e5f706c 61636524 4c542424 op_in_place$LT$$
+  0x00011480 4c542461 6c6c6f63 2e2e626f 7865642e LT$alloc..boxed.
+  0x00011490 2e426f78 244c5424 64796e24 75323024 .Box$LT$dyn$u20$
+  0x000114a0 636f7265 2e2e6572 726f722e 2e457272 core..error..Err
+  0x000114b0 6f722475 32622463 6f72652e 2e6d6172 or$u2b$core..mar
+  0x000114c0 6b65722e 2e53656e 64247532 6224636f ker..Send$u2b$co
+  0x000114d0 72652e2e 6d61726b 65722e2e 53796e63 re..marker..Sync
+  0x000114e0 24475424 24753230 24617324 75323024 $GT$$u20$as$u20$
+  0x000114f0 636f7265 2e2e636f 6e766572 742e2e46 core..convert..F
+  0x00011500 726f6d24 4c542461 6c6c6f63 2e2e7374 rom$LT$alloc..st
+  0x00011510 72696e67 2e2e5374 72696e67 24475424 ring..String$GT$
+  0x00011520 24475424 2e2e6672 6f6d2e2e 53747269 $GT$..from..Stri
+  0x00011530 6e674572 726f7224 47542431 37683434 ngError$GT$17h44
+  0x00011540 66336138 31343833 35316431 3338452e f3a8148351d138E.
+  0x00011550 6c6c766d 2e333034 31333933 39353835 llvm.30413939585
+  0x00011560 36393937 34333439 005f5a4e 37355f24 69974349._ZN75_$
+  0x00011570 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
+  0x00011580 6f6e732e 2e507955 6e69636f 6465456e ons..PyUnicodeEn
+  0x00011590 636f6465 4572726f 72247532 30246173 codeError$u20$as
+  0x000115a0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x000115b0 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x000115c0 61313330 64663938 35623562 34636466 a130df985b5b4cdf
+  0x000115d0 45005f5a 4e37325f 244c5424 70796f33 E._ZN72_$LT$pyo3
+  0x000115e0 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x000115f0 5265736f 75726365 5761726e 696e6724 ResourceWarning$
+  0x00011600 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x00011610 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x00011620 666d7431 37686634 32663332 31393262 fmt17hf42f32192b
+  0x00011630 36626434 62394500 5f5a4e35 616c6c6f 6bd4b9E._ZN5allo
+  0x00011640 63377261 775f7665 63313952 61775665 c7raw_vec19RawVe
+  0x00011650 63244c54 24542443 24412447 54243136 c$LT$T$C$A$GT$16
+  0x00011660 72657365 7276655f 666f725f 70757368 reserve_for_push
+  0x00011670 31376839 36383433 61383065 37313530 17h96843a80e7150
+  0x00011680 63653945 005f5a4e 35616c6c 6f633772 ce9E._ZN5alloc7r
+  0x00011690 61775f76 65633139 52617756 6563244c aw_vec19RawVec$L
+  0x000116a0 54245424 43244124 47542431 36726573 T$T$C$A$GT$16res
+  0x000116b0 65727665 5f666f72 5f707573 68313768 erve_for_push17h
+  0x000116c0 38633962 31663134 65623739 38613061 8c9b1f14eb798a0a
+  0x000116d0 45005f5a 4e37355f 244c5424 70796f33 E._ZN75_$LT$pyo3
+  0x000116e0 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x000116f0 556e6963 6f646544 65636f64 65457272 UnicodeDecodeErr
+  0x00011700 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x00011710 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x00011720 54243366 6d743137 68643432 62386432 T$3fmt17hd42b8d2
+  0x00011730 32653864 39313730 3645005f 5a4e3463 2e8d91706E._ZN4c
+  0x00011740 6f726533 666d7439 466f726d 61747465 ore3fmt9Formatte
+  0x00011750 72397772 6974655f 666d7431 37686134 r9write_fmt17ha4
+  0x00011760 61383834 64623235 34613631 66394500 a884db254a61f9E.
+  0x00011770 616e6f6e 2e653965 62323337 63663530 anon.e9eb237cf50
+  0x00011780 61343362 36356436 33366230 66343737 a43b65d636b0f477
+  0x00011790 30623034 652e3333 2e6c6c76 6d2e3133 0b04e.33.llvm.13
+  0x000117a0 38363138 35323731 31333930 32373437 8618527113902747
+  0x000117b0 36005f5a 4e34636f 7265336e 756d3630 6._ZN4core3num60
+  0x000117c0 5f244c54 24696d70 6c247532 3024636f _$LT$impl$u20$co
+  0x000117d0 72652e2e 7374722e 2e747261 6974732e re..str..traits.
+  0x000117e0 2e46726f 6d537472 24753230 24666f72 .FromStr$u20$for
+  0x000117f0 24753230 24753634 24475424 3866726f $u20$u64$GT$8fro
+  0x00011800 6d5f7374 72313768 37616161 37316436 m_str17h7aaa71d6
+  0x00011810 31376565 37303839 45005f5a 4e34636f 17ee7089E._ZN4co
+  0x00011820 72653370 74723132 3664726f 705f696e re3ptr126drop_in
+  0x00011830 5f706c61 6365244c 54247079 6f332e2e _place$LT$pyo3..
+  0x00011840 6572722e 2e657272 5f737461 74652e2e err..err_state..
+  0x00011850 626f7865 645f6172 6773244c 5424636f boxed_args$LT$co
+  0x00011860 72652e2e 63686172 2e2e6465 636f6465 re..char..decode
+  0x00011870 2e2e4465 636f6465 55746631 36457272 ..DecodeUtf16Err
+  0x00011880 6f722447 54242e2e 24753762 24247537 or$GT$..$u7b$$u7
+  0x00011890 6224636c 6f737572 65247537 64242475 b$closure$u7d$$u
+  0x000118a0 37642424 47542431 37683462 31643731 7d$$GT$17h4b1d71
+  0x000118b0 37353930 63623366 3266452e 6c6c766d 7590cb3f2fE.llvm
+  0x000118c0 2e333136 30393037 32383138 38303738 .316090728188078
+  0x000118d0 31313233 005f5a4e 34636f72 6533666d 1123._ZN4core3fm
+  0x000118e0 74336e75 6d35325f 244c5424 696d706c t3num52_$LT$impl
+  0x000118f0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00011900 55707065 72486578 24753230 24666f72 UpperHex$u20$for
+  0x00011910 24753230 24753824 47542433 666d7431 $u20$u8$GT$3fmt1
+  0x00011920 37683862 62616166 65333338 34633261 7h8bbaafe3384c2a
+  0x00011930 61374500 5f5a4e34 636f7265 33707472 a7E._ZN4core3ptr
+  0x00011940 33376472 6f705f69 6e5f706c 61636524 37drop_in_place$
+  0x00011950 4c542463 6f72652e 2e666d74 2e2e4572 LT$core..fmt..Er
+  0x00011960 726f7224 47542431 37686532 30636333 ror$GT$17he20cc3
+  0x00011970 61363863 36316262 3139452e 6c6c766d a68c61bb19E.llvm
+  0x00011980 2e333034 31333933 39353835 36393937 .304139395856997
+  0x00011990 34333439 00616e6f 6e2e6239 61303438 4349.anon.b9a048
+  0x000119a0 36633030 61343137 32623762 31616335 6c00a4172b7b1ac5
+  0x000119b0 32623331 35616134 61332e31 342e6c6c 2b315aa4a3.14.ll
+  0x000119c0 766d2e31 33323338 38393334 33323230 vm.1323889343220
+  0x000119d0 30363932 32323600 5f5a4e34 70796f33 0692226._ZN4pyo3
+  0x000119e0 35696d70 6c5f3870 796d6f64 756c6539 5impl_8pymodule9
+  0x000119f0 4d6f6475 6c654465 6631316d 616b655f ModuleDef11make_
+  0x00011a00 6d6f6475 6c653137 68373966 32346664 module17h79f24fd
+  0x00011a10 37356136 65326337 6345005f 5a4e3634 75a6e2c7cE._ZN64
+  0x00011a20 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x00011a30 74696f6e 732e2e50 79494f45 72726f72 tions..PyIOError
+  0x00011a40 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00011a50 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
+  0x00011a60 33666d74 31376861 39393962 65313639 3fmt17ha999be169
+  0x00011a70 65303939 35373545 005f5a4e 34636f72 e099575E._ZN4cor
+  0x00011a80 6533666d 7439466f 726d6174 74657239 e3fmt9Formatter9
+  0x00011a90 77726974 655f7374 72313768 38313638 write_str17h8168
+  0x00011aa0 36613833 33663638 66633533 45005f5a 6a833f68fc53E._Z
+  0x00011ab0 4e37375f 244c5424 70796f33 2e2e6578 N77_$LT$pyo3..ex
+  0x00011ac0 63657074 696f6e73 2e2e5079 50726f63 ceptions..PyProc
+  0x00011ad0 6573734c 6f6f6b75 70457272 6f722475 essLookupError$u
+  0x00011ae0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x00011af0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x00011b00 33666d74 31376839 66366238 31666633 3fmt17h9f6b81ff3
+  0x00011b10 38386434 34663745 00616e6f 6e2e3638 88d44f7E.anon.68
+  0x00011b20 32663035 33626133 64366431 34616635 2f053ba3d6d14af5
+  0x00011b30 62323763 66636262 64313633 36332e30 b27cfcbbd16363.0
+  0x00011b40 2e6c6c76 6d2e3536 39373932 39373639 .llvm.5697929769
+  0x00011b50 31333330 35373437 36005f5a 4e347079 133057476._ZN4py
+  0x00011b60 6f333574 79706573 35747570 6c653132 o35types5tuple12
+  0x00011b70 355f244c 5424696d 706c2475 32302470 5_$LT$impl$u20$p
+  0x00011b80 796f332e 2e636f6e 76657273 696f6e2e yo3..conversion.
+  0x00011b90 2e496e74 6f507924 4c542470 796f332e .IntoPy$LT$pyo3.
+  0x00011ba0 2e696e73 74616e63 652e2e50 79244c54 .instance..Py$LT
+  0x00011bb0 2470796f 332e2e74 79706573 2e2e616e $pyo3..types..an
+  0x00011bc0 792e2e50 79416e79 24475424 24475424 y..PyAny$GT$$GT$
+  0x00011bd0 24753230 24666f72 24753230 24244c50 $u20$for$u20$$LP
+  0x00011be0 24543024 43242452 50242447 54243769 $T0$C$$RP$$GT$7i
+  0x00011bf0 6e746f5f 70793137 68643665 64366563 nto_py17hd6ed6ec
+  0x00011c00 30333136 66383831 3445005f 5a4e3561 0316f8814E._ZN5a
+  0x00011c10 6c6c6f63 37726177 5f766563 31395261 lloc7raw_vec19Ra
+  0x00011c20 77566563 244c5424 54244324 41244754 wVec$LT$T$C$A$GT
+  0x00011c30 24313672 65736572 76655f66 6f725f70 $16reserve_for_p
+  0x00011c40 75736831 37683566 63623064 32306662 ush17h5fcb0d20fb
+  0x00011c50 33316634 37384500 5f5a4e33 73746439 31f478E._ZN3std9
+  0x00011c60 70616e69 636b696e 67313170 616e6963 panicking11panic
+  0x00011c70 5f636f75 6e743138 474c4f42 414c5f50 _count18GLOBAL_P
+  0x00011c80 414e4943 5f434f55 4e543137 68343931 ANIC_COUNT17h491
+  0x00011c90 64383230 65643833 31386563 3545005f d820ed8318ec5E._
+  0x00011ca0 5a4e3636 5f244c54 2470796f 332e2e65 ZN66_$LT$pyo3..e
+  0x00011cb0 78636570 74696f6e 732e2e50 794e616d xceptions..PyNam
+  0x00011cc0 65457272 6f722475 32302461 73247532 eError$u20$as$u2
+  0x00011cd0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x00011ce0 75672447 54243366 6d743137 68666461 ug$GT$3fmt17hfda
+  0x00011cf0 31656631 31373734 37396236 3145005f 1ef1177479b61E._
+  0x00011d00 5a4e3463 6f726533 666d7433 6e756d35 ZN4core3fmt3num5
+  0x00011d10 355f244c 5424696d 706c2475 32302463 5_$LT$impl$u20$c
+  0x00011d20 6f72652e 2e666d74 2e2e4c6f 77657248 ore..fmt..LowerH
+  0x00011d30 65782475 32302466 6f722475 32302475 ex$u20$for$u20$u
+  0x00011d40 73697a65 24475424 33666d74 31376862 size$GT$3fmt17hb
+  0x00011d50 37333432 64643137 35306463 38383745 7342dd1750dc887E
+  0x00011d60 005f5a4e 3470796f 33357479 70657335 ._ZN4pyo35types5
+  0x00011d70 7475706c 65375079 5475706c 65336c65 tuple7PyTuple3le
+  0x00011d80 6e313768 63653737 61643463 34643865 n17hce77ad4c4d8e
+  0x00011d90 63343763 4500616e 6f6e2e36 38326630 c47cE.anon.682f0
+  0x00011da0 35336261 33643664 31346166 35623237 53ba3d6d14af5b27
+  0x00011db0 63666362 62643136 3336332e 332e6c6c cfcbbd16363.3.ll
+  0x00011dc0 766d2e35 36393739 32393736 39313333 vm.5697929769133
+  0x00011dd0 30353734 3736005f 5a4e3463 6f726533 057476._ZN4core3
+  0x00011de0 70747235 3064726f 705f696e 5f706c61 ptr50drop_in_pla
+  0x00011df0 6365244c 5424616c 6c6f632e 2e626f72 ce$LT$alloc..bor
+  0x00011e00 726f772e 2e436f77 244c5424 73747224 row..Cow$LT$str$
+  0x00011e10 47542424 47542431 37686232 31633831 GT$$GT$17hb21c81
+  0x00011e20 35346535 38663066 6336452e 6c6c766d 54e58f0fc6E.llvm
+  0x00011e30 2e333136 30393037 32383138 38303738 .316090728188078
+  0x00011e40 31313233 005f5a4e 33737464 32696f35 1123._ZN3std2io5
+  0x00011e50 6572726f 7238335f 244c5424 696d706c error83_$LT$impl
+  0x00011e60 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00011e70 44656275 67247532 3024666f 72247532 Debug$u20$for$u2
+  0x00011e80 30247374 642e2e69 6f2e2e65 72726f72 0$std..io..error
+  0x00011e90 2e2e7265 70725f62 69747061 636b6564 ..repr_bitpacked
+  0x00011ea0 2e2e5265 70722447 54243366 6d743137 ..Repr$GT$3fmt17
+  0x00011eb0 68646562 32386630 30623436 38353866 hdeb28f00b46858f
+  0x00011ec0 3945005f 5f727573 745f666f 72656967 9E.__rust_foreig
+  0x00011ed0 6e5f6578 63657074 696f6e00 5f5a4e31 n_exception._ZN1
+  0x00011ee0 36706172 6b696e67 5f6c6f74 5f636f72 6parking_lot_cor
+  0x00011ef0 65313170 61726b69 6e675f6c 6f743136 e11parking_lot16
+  0x00011f00 63726561 74655f68 61736874 61626c65 create_hashtable
+  0x00011f10 31376832 63316161 37396633 35303038 17h2c1aa79f35008
+  0x00011f20 34326145 005f5a4e 37365f24 4c542470 42aE._ZN76_$LT$p
+  0x00011f30 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00011f40 2e507943 68696c64 50726f63 65737345 .PyChildProcessE
+  0x00011f50 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x00011f60 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
+  0x00011f70 61792447 54243366 6d743137 68333764 ay$GT$3fmt17h37d
+  0x00011f80 36393138 64616362 32376566 3545005f 6918dacb27ef5E._
+  0x00011f90 5a4e3373 74643130 7379735f 636f6d6d ZN3std10sys_comm
+  0x00011fa0 6f6e3962 61636b74 72616365 32365f5f on9backtrace26__
+  0x00011fb0 72757374 5f656e64 5f73686f 72745f62 rust_end_short_b
+  0x00011fc0 61636b74 72616365 31376839 39313366 acktrace17h9913f
+  0x00011fd0 38643038 62393235 61336545 005f5a4e 8d08b925a3eE._ZN
+  0x00011fe0 36375f24 4c542470 796f332e 2e657863 67_$LT$pyo3..exc
+  0x00011ff0 65707469 6f6e732e 2e50794b 65794572 eptions..PyKeyEr
+  0x00012000 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x00012010 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x00012020 79244754 2433666d 74313768 32303031 y$GT$3fmt17h2001
+  0x00012030 39393162 62666139 32323333 45005f5a 991bbfa92233E._Z
+  0x00012040 4e37365f 244c5424 70796f33 2e2e6578 N76_$LT$pyo3..ex
+  0x00012050 63657074 696f6e73 2e2e5079 4b657962 ceptions..PyKeyb
+  0x00012060 6f617264 496e7465 72727570 74247532 oardInterrupt$u2
+  0x00012070 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00012080 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
+  0x00012090 666d7431 37686631 63633335 37653637 fmt17hf1cc357e67
+  0x000120a0 62363562 38634500 616e6f6e 2e613830 b65b8cE.anon.a80
+  0x000120b0 39303264 36626230 38373733 62663637 902d6bb08773bf67
+  0x000120c0 34336430 32336337 64663733 652e3133 43d023c7df73e.13
+  0x000120d0 2e6c6c76 6d2e3131 39343036 32313336 .llvm.1194062136
+  0x000120e0 37353630 36363238 3035005f 5a4e3530 7560662805._ZN50
+  0x000120f0 5f244c54 24245246 246d7574 24753230 _$LT$$RF$mut$u20
+  0x00012100 24572475 32302461 73247532 3024636f $W$u20$as$u20$co
+  0x00012110 72652e2e 666d742e 2e577269 74652447 re..fmt..Write$G
+  0x00012120 54243977 72697465 5f666d74 31376835 T$9write_fmt17h5
+  0x00012130 34366437 61303433 66623835 65303345 46d7a043fb85e03E
+  0x00012140 2e6c6c76 6d2e3330 34313339 33393538 .llvm.3041393958
+  0x00012150 35363939 37343334 39005f5a 4e37375f 569974349._ZN77_
+  0x00012160 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x00012170 696f6e73 2e2e5079 436f6e6e 65637469 ions..PyConnecti
+  0x00012180 6f6e5265 73657445 72726f72 24753230 onResetError$u20
+  0x00012190 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x000121a0 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x000121b0 31376838 34316462 64633133 62303238 17h841dbdc13b028
+  0x000121c0 30373345 005f5a4e 37335f24 4c542463 073E._ZN73_$LT$c
+  0x000121d0 6f72652e 2e70616e 69632e2e 70616e69 ore..panic..pani
+  0x000121e0 635f696e 666f2e2e 50616e69 63496e66 c_info..PanicInf
+  0x000121f0 6f247532 30246173 24753230 24636f72 o$u20$as$u20$cor
+  0x00012200 652e2e66 6d742e2e 44697370 6c617924 e..fmt..Display$
+  0x00012210 47542433 666d7431 37683865 31313238 GT$3fmt17h8e1128
+  0x00012220 62383339 31343935 34354500 5f5a4e34 b839149545E._ZN4
+  0x00012230 325f244c 54247374 72247532 30246173 2_$LT$str$u20$as
+  0x00012240 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00012250 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x00012260 37686362 30346163 63353234 34643335 7hcb04acc5244d35
+  0x00012270 65334500 5f5a4e34 70796f33 35747970 e3E._ZN4pyo35typ
+  0x00012280 65733130 74797065 6f626a65 63743650 es10typeobject6P
+  0x00012290 79547970 65346e61 6d653849 4e544552 yType4name8INTER
+  0x000122a0 4e454431 37686465 33323330 62396535 NED17hde3230b9e5
+  0x000122b0 66653333 3763452e 6c6c766d 2e313436 fe337cE.llvm.146
+  0x000122c0 33313433 31343233 31303736 38373832 3143142310768782
+  0x000122d0 3300616e 6f6e2e37 62393436 61653164 3.anon.7b946ae1d
+  0x000122e0 33613636 36373937 65326462 31663336 3a666797e2db1f36
+  0x000122f0 65346364 3665372e 32302e6c 6c766d2e e4cd6e7.20.llvm.
+  0x00012300 31383335 36373530 34383536 31343531 1835675048561451
+  0x00012310 33313239 005f5a4e 3567696d 6c693472 3129._ZN5gimli4r
+  0x00012320 65616436 61626272 65763133 41626272 ead6abbrev13Abbr
+  0x00012330 65766961 74696f6e 7335656d 70747931 eviations5empty1
+  0x00012340 37683833 35313234 32326433 63343034 7h83512422d3c404
+  0x00012350 33344500 5f5a4e37 335f244c 54247079 34E._ZN73_$LT$py
+  0x00012360 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x00012370 50795265 66657265 6e636545 72726f72 PyReferenceError
+  0x00012380 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00012390 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
+  0x000123a0 54243366 6d743137 68366233 62643764 T$3fmt17h6b3bd7d
+  0x000123b0 35663663 61373831 3045005f 5a4e3463 5f6ca7810E._ZN4c
+  0x000123c0 6f726533 73747238 636f6e76 65727473 ore3str8converts
+  0x000123d0 3966726f 6d5f7574 66383137 68393666 9from_utf817h96f
+  0x000123e0 65303466 34633664 33663165 6145005f e04f4c6d3f1eaE._
+  0x000123f0 5a4e3530 5f244c54 24245246 246d7574 ZN50_$LT$$RF$mut
+  0x00012400 24753230 24572475 32302461 73247532 $u20$W$u20$as$u2
+  0x00012410 3024636f 72652e2e 666d742e 2e577269 0$core..fmt..Wri
+  0x00012420 74652447 54243977 72697465 5f737472 te$GT$9write_str
+  0x00012430 31376863 31376437 65393632 35623764 17hc17d7e9625b7d
+  0x00012440 66666145 2e6c6c76 6d2e3330 34313339 ffaE.llvm.304139
+  0x00012450 33393538 35363939 37343334 39005f5a 3958569974349._Z
+  0x00012460 4e34636f 72653366 6d74336e 756d3532 N4core3fmt3num52
+  0x00012470 5f244c54 24696d70 6c247532 3024636f _$LT$impl$u20$co
+  0x00012480 72652e2e 666d742e 2e557070 65724865 re..fmt..UpperHe
+  0x00012490 78247532 3024666f 72247532 30246938 x$u20$for$u20$i8
+  0x000124a0 24475424 33666d74 31376839 35313034 $GT$3fmt17h95104
+  0x000124b0 39326461 35613766 35663645 005f5a4e 92da5a7f5f6E._ZN
+  0x000124c0 37355f24 4c542470 796f332e 2e657863 75_$LT$pyo3..exc
+  0x000124d0 65707469 6f6e732e 2e50794e 6f744144 eptions..PyNotAD
+  0x000124e0 69726563 746f7279 4572726f 72247532 irectoryError$u2
+  0x000124f0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00012500 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x00012510 74313768 31313332 30623430 62323032 t17h11320b40b202
+  0x00012520 32373161 45005f5a 4e37355f 244c5424 271aE._ZN75_$LT$
+  0x00012530 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x00012540 2e2e5079 50726f63 6573734c 6f6f6b75 ..PyProcessLooku
+  0x00012550 70457272 6f722475 32302461 73247532 pError$u20$as$u2
+  0x00012560 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x00012570 75672447 54243366 6d743137 68383930 ug$GT$3fmt17h890
+  0x00012580 36613436 65663762 31343363 3145005f 6a46ef7b143c1E._
+  0x00012590 5a4e3463 6f726533 70747234 3764726f ZN4core3ptr47dro
+  0x000125a0 705f696e 5f706c61 6365244c 5424636f p_in_place$LT$co
+  0x000125b0 72652e2e 63656c6c 2e2e426f 72726f77 re..cell..Borrow
+  0x000125c0 4d757445 72726f72 24475424 31376862 MutError$GT$17hb
+  0x000125d0 64653830 65616663 62376563 30326245 de80eafcb7ec02bE
+  0x000125e0 2e6c6c76 6d2e3138 33353637 35303438 .llvm.1835675048
+  0x000125f0 35363134 35313331 3239005f 5a4e3636 5614513129._ZN66
+  0x00012600 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x00012610 74696f6e 732e2e50 79547970 65457272 tions..PyTypeErr
+  0x00012620 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x00012630 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x00012640 54243366 6d743137 68303235 61656531 T$3fmt17h025aee1
+  0x00012650 34626438 31356634 31450061 6e6f6e2e 4bd815f41E.anon.
+  0x00012660 37623934 36616531 64336136 36363739 7b946ae1d3a66679
+  0x00012670 37653264 62316633 36653463 64366537 7e2db1f36e4cd6e7
+  0x00012680 2e33322e 6c6c766d 2e313833 35363735 .32.llvm.1835675
+  0x00012690 30343835 36313435 31333132 39005f5a 0485614513129._Z
+  0x000126a0 4e35616c 6c6f6335 616c6c6f 6338626f N5alloc5alloc8bo
+  0x000126b0 785f6672 65653137 68366436 30646532 x_free17h6d60de2
+  0x000126c0 65386537 30376264 64452e6c 6c766d2e e8e707bddE.llvm.
+  0x000126d0 31333233 38383933 34333232 30303639 1323889343220069
+  0x000126e0 32323236 005f5a4e 38345f24 4c542470 2226._ZN84_$LT$p
+  0x000126f0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00012700 2e507950 656e6469 6e674465 70726563 .PyPendingDeprec
+  0x00012710 6174696f 6e576172 6e696e67 24753230 ationWarning$u20
+  0x00012720 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00012730 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x00012740 6d743137 68343366 36646530 64666266 mt17h43f6de0dfbf
+  0x00012750 61386435 3945005f 5a4e3735 5f244c54 a8d59E._ZN75_$LT
+  0x00012760 2467696d 6c692e2e 72656164 2e2e6162 $gimli..read..ab
+  0x00012770 62726576 2e2e4174 74726962 75746573 brev..Attributes
+  0x00012780 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00012790 2e2e6f70 732e2e64 65726566 2e2e4465 ..ops..deref..De
+  0x000127a0 72656624 47542435 64657265 66313768 ref$GT$5deref17h
+  0x000127b0 30653937 37383037 36336435 30313662 0e97780763d5016b
+  0x000127c0 45005f5a 4e38315f 244c5424 24524624 E._ZN81_$LT$$RF$
+  0x000127d0 24753562 24753824 75356424 24753230 $u5b$u8$u5d$$u20
+  0x000127e0 24617324 75323024 616c6c6f 632e2e66 $as$u20$alloc..f
+  0x000127f0 66692e2e 635f7374 722e2e43 53747269 fi..c_str..CStri
+  0x00012800 6e672e2e 6e65772e 2e537065 634e6577 ng..new..SpecNew
+  0x00012810 496d706c 24475424 31337370 65635f6e Impl$GT$13spec_n
+  0x00012820 65775f69 6d706c31 37686363 62313137 ew_impl17hccb117
+  0x00012830 64616531 37656134 30654500 5f5a4e31 dae17ea40eE._ZN1
+  0x00012840 316d696e 697a5f6f 78696465 37696e66 1miniz_oxide7inf
+  0x00012850 6c617465 34636f72 65313744 65636f6d late4core17Decom
+  0x00012860 70726573 736f724f 78696465 336e6577 pressorOxide3new
+  0x00012870 31376864 36326136 32653633 65343932 17hd62a62e63e492
+  0x00012880 30346545 005f5a4e 36365f24 4c542470 04eE._ZN66_$LT$p
+  0x00012890 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x000128a0 2e507949 4f457272 6f722475 32302461 .PyIOError$u20$a
+  0x000128b0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x000128c0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x000128d0 31376834 36383462 38363363 37343035 17h4684b863c7405
+  0x000128e0 63323445 005f5a4e 36365f24 4c542470 c24E._ZN66_$LT$p
+  0x000128f0 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00012900 2e507957 61726e69 6e672475 32302461 .PyWarning$u20$a
+  0x00012910 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00012920 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x00012930 31376863 35616162 38303233 36396135 17hc5aab802369a5
+  0x00012940 62653845 005f5a4e 3470796f 33357479 be8E._ZN4pyo35ty
+  0x00012950 70657333 616e7935 5079416e 79376765 pes3any5PyAny7ge
+  0x00012960 74617474 72313768 63643835 31646234 tattr17hcd851db4
+  0x00012970 33653536 38353133 45005f5a 4e34636f 3e568513E._ZN4co
+  0x00012980 72653370 74723937 64726f70 5f696e5f re3ptr97drop_in_
+  0x00012990 706c6163 65244c54 2470796f 332e2e65 place$LT$pyo3..e
+  0x000129a0 72722e2e 6572725f 73746174 652e2e62 rr..err_state..b
+  0x000129b0 6f786564 5f617267 73244c54 24245246 oxed_args$LT$$RF
+  0x000129c0 24737472 24475424 2e2e2475 37622424 $str$GT$..$u7b$$
+  0x000129d0 75376224 636c6f73 75726524 75376424 u7b$closure$u7d$
+  0x000129e0 24753764 24244754 24313768 32663863 $u7d$$GT$17h2f8c
+  0x000129f0 31616531 33636161 62623130 452e6c6c 1ae13caabb10E.ll
+  0x00012a00 766d2e33 31363039 30373238 31383830 vm.3160907281880
+  0x00012a10 37383131 3233005f 5a4e3463 6f726533 781123._ZN4core3
+  0x00012a20 70747231 32326472 6f705f69 6e5f706c ptr122drop_in_pl
+  0x00012a30 61636524 4c542461 6c6c6f63 2e2e7665 ace$LT$alloc..ve
+  0x00012a40 632e2e69 6e746f5f 69746572 2e2e496e c..into_iter..In
+  0x00012a50 746f4974 6572244c 5424636f 72652e2e toIter$LT$core..
+  0x00012a60 7074722e 2e6e6f6e 5f6e756c 6c2e2e4e ptr..non_null..N
+  0x00012a70 6f6e4e75 6c6c244c 54247079 6f335f66 onNull$LT$pyo3_f
+  0x00012a80 66692e2e 6f626a65 63742e2e 50794f62 fi..object..PyOb
+  0x00012a90 6a656374 24475424 24475424 24475424 ject$GT$$GT$$GT$
+  0x00012aa0 31376833 35346536 35623263 33343632 17h354e65b2c3462
+  0x00012ab0 32313145 2e6c6c76 6d2e3133 32333838 211E.llvm.132388
+  0x00012ac0 39333433 32323030 36393232 32360072 93432200692226.r
+  0x00012ad0 7573745f 62656769 6e5f756e 77696e64 ust_begin_unwind
+  0x00012ae0 00616e6f 6e2e3531 30356264 64373966 .anon.5105bdd79f
+  0x00012af0 32336231 31373166 33383734 32666561 23b1171f38742fea
+  0x00012b00 61633564 31372e32 352e6c6c 766d2e33 ac5d17.25.llvm.3
+  0x00012b10 31363039 30373238 31383830 37383131 1609072818807811
+  0x00012b20 3233005f 5a4e3463 6f726533 70747233 23._ZN4core3ptr3
+  0x00012b30 3764726f 705f696e 5f706c61 6365244c 7drop_in_place$L
+  0x00012b40 54247079 6f332e2e 6572722e 2e507945 T$pyo3..err..PyE
+  0x00012b50 72722447 54243137 68626437 34353762 rr$GT$17hbd7457b
+  0x00012b60 30323035 37336431 62452e6c 6c766d2e 020573d1bE.llvm.
+  0x00012b70 31333233 38383933 34333232 30303639 1323889343220069
+  0x00012b80 32323236 005f5a4e 37335f24 4c542470 2226._ZN73_$LT$p
+  0x00012b90 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00012ba0 2e507949 6e746572 72757074 65644572 .PyInterruptedEr
+  0x00012bb0 726f7224 75323024 61732475 32302463 ror$u20$as$u20$c
+  0x00012bc0 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x00012bd0 47542433 666d7431 37686237 32613032 GT$3fmt17hb72a02
+  0x00012be0 32613761 36626432 61394500 5f5a4e37 2a7a6bd2a9E._ZN7
+  0x00012bf0 345f244c 54247079 6f332e2e 65786365 4_$LT$pyo3..exce
+  0x00012c00 7074696f 6e732e2e 50794272 6f6b656e ptions..PyBroken
+  0x00012c10 50697065 4572726f 72247532 30246173 PipeError$u20$as
+  0x00012c20 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00012c30 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x00012c40 37683532 65333464 36356262 34393734 7h52e34d65bb4974
+  0x00012c50 33614500 5f5a4e36 385f244c 54247374 3aE._ZN68_$LT$st
+  0x00012c60 642e2e73 79732e2e 756e6978 2e2e6f73 d..sys..unix..os
+  0x00012c70 5f737472 2e2e536c 69636524 75323024 _str..Slice$u20$
+  0x00012c80 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00012c90 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
+  0x00012ca0 74313768 37653666 64663933 32613763 t17h7e6fdf932a7c
+  0x00012cb0 30643635 45005f5a 4e34636f 72653370 0d65E._ZN4core3p
+  0x00012cc0 74723133 3264726f 705f696e 5f706c61 tr132drop_in_pla
+  0x00012cd0 6365244c 5424636f 72652e2e 63656c6c ce$LT$core..cell
+  0x00012ce0 2e2e5265 664d7574 244c5424 616c6c6f ..RefMut$LT$allo
+  0x00012cf0 632e2e76 65632e2e 56656324 4c542463 c..vec..Vec$LT$c
+  0x00012d00 6f72652e 2e707472 2e2e6e6f 6e5f6e75 ore..ptr..non_nu
+  0x00012d10 6c6c2e2e 4e6f6e4e 756c6c24 4c542470 ll..NonNull$LT$p
+  0x00012d20 796f335f 6666692e 2e6f626a 6563742e yo3_ffi..object.
+  0x00012d30 2e50794f 626a6563 74244754 24244754 .PyObject$GT$$GT
+  0x00012d40 24244754 24244754 24313768 37336630 $$GT$$GT$17h73f0
+  0x00012d50 65656335 62636135 39616233 452e6c6c eec5bca59ab3E.ll
+  0x00012d60 766d2e31 38333536 37353034 38353631 vm.1835675048561
+  0x00012d70 34353133 31323900 5f5a4e35 616c6c6f 4513129._ZN5allo
+  0x00012d80 63377261 775f7665 63313763 61706163 c7raw_vec17capac
+  0x00012d90 6974795f 6f766572 666c6f77 31376835 ity_overflow17h5
+  0x00012da0 36343437 35643433 61633065 33376345 64475d43ac0e37cE
+  0x00012db0 005f5a4e 36365f24 4c542470 796f332e ._ZN66_$LT$pyo3.
+  0x00012dc0 2e657863 65707469 6f6e732e 2e50794f .exceptions..PyO
+  0x00012dd0 53457272 6f722475 32302461 73247532 SError$u20$as$u2
+  0x00012de0 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00012df0 706c6179 24475424 33666d74 31376865 play$GT$3fmt17he
+  0x00012e00 64616137 31356363 35336333 30613345 daa715cc53c30a3E
+  0x00012e10 005f5a4e 33737464 33737973 34756e69 ._ZN3std3sys4uni
+  0x00012e20 78356c6f 636b7331 32667574 65785f72 x5locks12futex_r
+  0x00012e30 776c6f63 6b365277 4c6f636b 31347265 wlock6RwLock14re
+  0x00012e40 61645f63 6f6e7465 6e646564 31376838 ad_contended17h8
+  0x00012e50 64326434 66323566 61376532 63666645 d2d4f25fa7e2cffE
+  0x00012e60 005f5a4e 34636f72 6533666d 74336e75 ._ZN4core3fmt3nu
+  0x00012e70 6d33696d 7035315f 244c5424 696d706c m3imp51_$LT$impl
+  0x00012e80 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00012e90 44697370 6c617924 75323024 666f7224 Display$u20$for$
+  0x00012ea0 75323024 75382447 54243366 6d743137 u20$u8$GT$3fmt17
+  0x00012eb0 68653439 31386337 38323136 62383939 he4918c78216b899
+  0x00012ec0 3545005f 5a4e3832 5f244c54 24636f72 5E._ZN82_$LT$cor
+  0x00012ed0 652e2e63 6861722e 2e457363 61706544 e..char..EscapeD
+  0x00012ee0 65627567 24753230 24617324 75323024 ebug$u20$as$u20$
+  0x00012ef0 636f7265 2e2e6974 65722e2e 74726169 core..iter..trai
+  0x00012f00 74732e2e 69746572 61746f72 2e2e4974 ts..iterator..It
+  0x00012f10 65726174 6f722447 5424346e 65787431 erator$GT$4next1
+  0x00012f20 37683063 65346335 62633536 64343334 7h0ce4c5bc56d434
+  0x00012f30 39664500 5f5a4e34 335f244c 54246368 9fE._ZN43_$LT$ch
+  0x00012f40 61722475 32302461 73247532 3024636f ar$u20$as$u20$co
+  0x00012f50 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
+  0x00012f60 24475424 33666d74 31376833 31633463 $GT$3fmt17h31c4c
+  0x00012f70 32346262 64303861 61323445 005f5a4e 24bbd08aa24E._ZN
+  0x00012f80 34636f72 65337374 72377061 74746572 4core3str7patter
+  0x00012f90 6e313153 74725365 61726368 6572336e n11StrSearcher3n
+  0x00012fa0 65773137 68363333 36373130 33313361 ew17h6336710313a
+  0x00012fb0 33626635 62450061 6e6f6e2e 65396562 3bf5bE.anon.e9eb
+  0x00012fc0 32333763 66353061 34336236 35643633 237cf50a43b65d63
+  0x00012fd0 36623066 34373730 62303465 2e33342e 6b0f4770b04e.34.
+  0x00012fe0 6c6c766d 2e313338 36313835 32373131 llvm.13861852711
+  0x00012ff0 33393032 37343736 005f5a4e 37315f24 39027476._ZN71_$
+  0x00013000 4c542472 75737463 5f64656d 616e676c LT$rustc_demangl
+  0x00013010 652e2e53 697a654c 696d6974 45786861 e..SizeLimitExha
+  0x00013020 75737465 64247532 30246173 24753230 usted$u20$as$u20
+  0x00013030 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
+  0x00013040 67244754 2433666d 74313768 31346139 g$GT$3fmt17h14a9
+  0x00013050 35313533 38383838 63633734 45005f5a 51538888cc74E._Z
+  0x00013060 4e37365f 244c5424 70796f33 2e2e6578 N76_$LT$pyo3..ex
+  0x00013070 63657074 696f6e73 2e2e5079 4d6f6475 ceptions..PyModu
+  0x00013080 6c654e6f 74466f75 6e644572 726f7224 leNotFoundError$
+  0x00013090 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x000130a0 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x000130b0 666d7431 37686239 30666132 65343538 fmt17hb90fa2e458
+  0x000130c0 64353463 64354500 5f5a4e34 70796f33 d54cd5E._ZN4pyo3
+  0x000130d0 35696d70 6c5f3970 796d6574 686f6473 5impl_9pymethods
+  0x000130e0 31315079 4d657468 6f644465 66313361 11PyMethodDef13a
+  0x000130f0 735f6d65 74686f64 5f646566 31376836 s_method_def17h6
+  0x00013100 32346462 64326263 33613561 62336145 24dbd2bc3a5ab3aE
+  0x00013110 005f5f54 4d435f45 4e445f5f 005f5a4e .__TMC_END__._ZN
+  0x00013120 37305f24 4c542470 796f332e 2e657863 70_$LT$pyo3..exc
+  0x00013130 65707469 6f6e732e 2e507953 796e7461 eptions..PySynta
+  0x00013140 78576172 6e696e67 24753230 24617324 xWarning$u20$as$
+  0x00013150 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x00013160 65627567 24475424 33666d74 31376862 ebug$GT$3fmt17hb
+  0x00013170 61656561 37386662 37366362 33666145 aeea78fb76cb3faE
+  0x00013180 005f5a4e 35385f24 4c542461 6c6c6f63 ._ZN58_$LT$alloc
+  0x00013190 2e2e7374 72696e67 2e2e5374 72696e67 ..string..String
+  0x000131a0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x000131b0 2e2e666d 742e2e57 72697465 24475424 ..fmt..Write$GT$
+  0x000131c0 39777269 74655f73 74723137 68636162 9write_str17hcab
+  0x000131d0 64336663 39663734 39616533 30452e6c d3fc9f749ae30E.l
+  0x000131e0 6c766d2e 35363937 39323937 36393133 lvm.569792976913
+  0x000131f0 33303537 34373600 5f5a4e36 325f244c 3057476._ZN62_$L
+  0x00013200 54247079 6f332e2e 74797065 732e2e61 T$pyo3..types..a
+  0x00013210 6e792e2e 5079416e 79247532 30246173 ny..PyAny$u20$as
+  0x00013220 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00013230 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x00013240 37683031 62666437 66616635 61646432 7h01bfd7faf5add2
+  0x00013250 65614500 616e6f6e 2e623961 30343836 eaE.anon.b9a0486
+  0x00013260 63303061 34313732 62376231 61633532 c00a4172b7b1ac52
+  0x00013270 62333135 61613461 332e3338 2e6c6c76 b315aa4a3.38.llv
+  0x00013280 6d2e3133 32333838 39333433 32323030 m.13238893432200
+  0x00013290 36393232 3236005f 5a4e3470 796f3331 692226._ZN4pyo31
+  0x000132a0 31636f6e 76657273 696f6e73 33737464 1conversions3std
+  0x000132b0 36737472 696e6738 325f244c 5424696d 6string82_$LT$im
+  0x000132c0 706c2475 32302470 796f332e 2e636f6e pl$u20$pyo3..con
+  0x000132d0 76657273 696f6e2e 2e46726f 6d50794f version..FromPyO
+  0x000132e0 626a6563 74247532 3024666f 72247532 bject$u20$for$u2
+  0x000132f0 3024616c 6c6f632e 2e737472 696e672e 0$alloc..string.
+  0x00013300 2e537472 696e6724 47542437 65787472 .String$GT$7extr
+  0x00013310 61637431 37683038 61303733 39356135 act17h08a07395a5
+  0x00013320 33656430 39384500 5f5a4e31 36706172 3ed098E._ZN16par
+  0x00013330 6b696e67 5f6c6f74 5f636f72 65313170 king_lot_core11p
+  0x00013340 61726b69 6e675f6c 6f743948 41534854 arking_lot9HASHT
+  0x00013350 41424c45 31376839 66636436 62353036 ABLE17h9fcd6b506
+  0x00013360 35386437 37393045 005f5a4e 37325f24 58d7790E._ZN72_$
+  0x00013370 4c542470 796f332e 2e657863 65707469 LT$pyo3..excepti
+  0x00013380 6f6e732e 2e507941 72697468 6d657469 ons..PyArithmeti
+  0x00013390 63457272 6f722475 32302461 73247532 cError$u20$as$u2
+  0x000133a0 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x000133b0 75672447 54243366 6d743137 68386435 ug$GT$3fmt17h8d5
+  0x000133c0 38333033 32393332 64333235 3845005f 83032932d3258E._
+  0x000133d0 5a4e3431 5f244c54 24636861 72247532 ZN41_$LT$char$u2
+  0x000133e0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x000133f0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x00013400 74313768 61636361 31653038 35343835 t17hacca1e085485
+  0x00013410 33326631 45005f5a 4e337374 64397061 32f1E._ZN3std9pa
+  0x00013420 6e69636b 696e6731 31626567 696e5f70 nicking11begin_p
+  0x00013430 616e6963 31376837 61336365 66376339 anic17h7a3cef7c9
+  0x00013440 34653337 35623845 005f5a4e 34636f72 4e375b8E._ZN4cor
+  0x00013450 6533666d 74386275 696c6465 72733131 e3fmt8builders11
+  0x00013460 44656275 67537472 75637435 6669656c DebugStruct5fiel
+  0x00013470 64313768 33346163 31626263 38386137 d17h34ac1bbc88a7
+  0x00013480 39616333 45005f5a 4e39315f 244c5424 9ac3E._ZN91_$LT$
+  0x00013490 7374642e 2e70616e 69636b69 6e672e2e std..panicking..
+  0x000134a0 72757374 5f70616e 69635f77 6974686f rust_panic_witho
+  0x000134b0 75745f68 6f6f6b2e 2e526577 72617042 ut_hook..RewrapB
+  0x000134c0 6f782475 32302461 73247532 3024636f ox$u20$as$u20$co
+  0x000134d0 72652e2e 70616e69 632e2e42 6f784d65 re..panic..BoxMe
+  0x000134e0 55702447 54243367 65743137 68643935 Up$GT$3get17hd95
+  0x000134f0 38373863 34346265 36393239 3845005f 878c44be69298E._
+  0x00013500 5a4e3373 74643130 7379735f 636f6d6d ZN3std10sys_comm
+  0x00013510 6f6e3962 61636b74 72616365 32365f5f on9backtrace26__
+  0x00013520 72757374 5f656e64 5f73686f 72745f62 rust_end_short_b
+  0x00013530 61636b74 72616365 31376835 31353265 acktrace17h5152e
+  0x00013540 35333833 39353666 36353245 005f5a4e 5383956f652E._ZN
+  0x00013550 34636f72 65337074 72373064 726f705f 4core3ptr70drop_
+  0x00013560 696e5f70 6c616365 244c5424 70796f33 in_place$LT$pyo3
+  0x00013570 2e2e696e 7374616e 63652e2e 5079244c ..instance..Py$L
+  0x00013580 54247079 6f332e2e 74797065 732e2e61 T$pyo3..types..a
+  0x00013590 6e792e2e 5079416e 79244754 24244754 ny..PyAny$GT$$GT
+  0x000135a0 24313768 37363264 31636337 63336437 $17h762d1cc7c3d7
+  0x000135b0 39373239 452e6c6c 766d2e31 31393031 9729E.llvm.11901
+  0x000135c0 34383233 34333535 35353631 33323700 482343555561327.
+  0x000135d0 5f5a4e34 636f7265 33666d74 336e756d _ZN4core3fmt3num
+  0x000135e0 35325f24 4c542469 6d706c24 75323024 52_$LT$impl$u20$
+  0x000135f0 636f7265 2e2e666d 742e2e4c 6f776572 core..fmt..Lower
+  0x00013600 48657824 75323024 666f7224 75323024 Hex$u20$for$u20$
+  0x00013610 75382447 54243366 6d743137 68363164 u8$GT$3fmt17h61d
+  0x00013620 65336464 38303836 34613264 6245005f e3dd80864a2dbE._
+  0x00013630 5a4e3134 72757374 635f6465 6d616e67 ZN14rustc_demang
+  0x00013640 6c653864 656d616e 676c6531 37683138 le8demangle17h18
+  0x00013650 33323964 38666633 36393565 33334500 329d8ff3695e33E.
+  0x00013660 5f5a4e35 616c6c6f 63377261 775f7665 _ZN5alloc7raw_ve
+  0x00013670 63313952 61775665 63244c54 24542443 c19RawVec$LT$T$C
+  0x00013680 24412447 54243136 72657365 7276655f $A$GT$16reserve_
+  0x00013690 666f725f 70757368 31376833 65386362 for_push17h3e8cb
+  0x000136a0 39663431 33336637 37363645 005f5a4e 9f4133f7766E._ZN
+  0x000136b0 34636f72 65337074 72363964 726f705f 4core3ptr69drop_
+  0x000136c0 696e5f70 6c616365 244c5424 616c6c6f in_place$LT$allo
+  0x000136d0 632e2e62 6f72726f 772e2e43 6f77244c c..borrow..Cow$L
+  0x000136e0 5424636f 72652e2e 6666692e 2e635f73 T$core..ffi..c_s
+  0x000136f0 74722e2e 43537472 24475424 24475424 tr..CStr$GT$$GT$
+  0x00013700 31376833 34373333 61653339 65303666 17h34733ae39e06f
+  0x00013710 64333245 2e6c6c76 6d2e3536 39373932 d32E.llvm.569792
+  0x00013720 39373639 31333330 35373437 36005f5a 9769133057476._Z
+  0x00013730 4e34636f 72653366 6d74336e 756d3533 N4core3fmt3num53
+  0x00013740 5f244c54 24696d70 6c247532 3024636f _$LT$impl$u20$co
+  0x00013750 72652e2e 666d742e 2e4c6f77 65724865 re..fmt..LowerHe
+  0x00013760 78247532 3024666f 72247532 30246933 x$u20$for$u20$i3
+  0x00013770 32244754 2433666d 74313768 37333438 2$GT$3fmt17h7348
+  0x00013780 31386338 66633632 65633662 45005f5a 18c8fc62ec6bE._Z
+  0x00013790 4e37305f 244c5424 70796f33 2e2e6578 N70_$LT$pyo3..ex
+  0x000137a0 63657074 696f6e73 2e2e5079 42756666 ceptions..PyBuff
+  0x000137b0 65724572 726f7224 75323024 61732475 erError$u20$as$u
+  0x000137c0 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
+  0x000137d0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
+  0x000137e0 66386330 65343166 64343734 39303331 f8c0e41fd4749031
+  0x000137f0 45005f5a 4e34636f 72653366 6d743862 E._ZN4core3fmt8b
+  0x00013800 75696c64 65727339 44656275 674c6973 uilders9DebugLis
+  0x00013810 74366669 6e697368 31376838 64663464 t6finish17h8df4d
+  0x00013820 64333264 36373734 63313645 005f5a4e d32d6774c16E._ZN
+  0x00013830 34636f72 65336f70 73386675 6e637469 4core3ops8functi
+  0x00013840 6f6e3646 6e4f6e63 65343063 616c6c5f on6FnOnce40call_
+  0x00013850 6f6e6365 24753762 24247537 62247674 once$u7b$$u7b$vt
+  0x00013860 61626c65 2e736869 6d247537 64242475 able.shim$u7d$$u
+  0x00013870 37642431 37683134 39653736 30323538 7d$17h149e760258
+  0x00013880 62326330 3334452e 6c6c766d 2e333136 b2c034E.llvm.316
+  0x00013890 30393037 32383138 38303738 31313233 0907281880781123
+  0x000138a0 005f5a4e 3470796f 33313174 7970655f ._ZN4pyo311type_
+  0x000138b0 6f626a65 63743130 50795479 7065496e object10PyTypeIn
+  0x000138c0 666f3131 74797065 5f6f626a 65637431 fo11type_object1
+  0x000138d0 37683934 38316130 36333162 36316466 7h9481a0631b61df
+  0x000138e0 31374500 5f5a4e36 385f244c 54247079 17E._ZN68_$LT$py
+  0x000138f0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x00013900 5079496d 706f7274 4572726f 72247532 PyImportError$u2
+  0x00013910 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00013920 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x00013930 74313768 62363666 35393163 36643132 t17hb66f591c6d12
+  0x00013940 34616230 45005f5a 4e39335f 244c5424 4ab0E._ZN93_$LT$
+  0x00013950 7374642e 2e70616e 69636b69 6e672e2e std..panicking..
+  0x00013960 62656769 6e5f7061 6e69635f 68616e64 begin_panic_hand
+  0x00013970 6c65722e 2e537472 50616e69 63506179 ler..StrPanicPay
+  0x00013980 6c6f6164 24753230 24617324 75323024 load$u20$as$u20$
+  0x00013990 636f7265 2e2e7061 6e69632e 2e426f78 core..panic..Box
+  0x000139a0 4d655570 24475424 33676574 31376863 MeUp$GT$3get17hc
+  0x000139b0 35396264 63663538 36666566 37366345 59bdcf586fef76cE
+  0x000139c0 005f5a4e 34636f72 6533666d 74336e75 ._ZN4core3fmt3nu
+  0x000139d0 6d33696d 7035325f 244c5424 696d706c m3imp52_$LT$impl
+  0x000139e0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x000139f0 44697370 6c617924 75323024 666f7224 Display$u20$for$
+  0x00013a00 75323024 75333224 47542433 666d7431 u20$u32$GT$3fmt1
+  0x00013a10 37686534 32326238 31393939 31306434 7he422b8199910d4
+  0x00013a20 34384500 5f5a4e35 67696d6c 6936636f 48E._ZN5gimli6co
+  0x00013a30 6d6d6f6e 39536563 74696f6e 4964346e mmon9SectionId4n
+  0x00013a40 616d6531 37686231 39656361 63663436 ame17hb19ecacf46
+  0x00013a50 35373538 66314500 5f5a4e33 73746435 5758f1E._ZN3std5
+  0x00013a60 616c6c6f 63387275 73745f6f 6f6d3137 alloc8rust_oom17
+  0x00013a70 68626232 63663438 37353637 34323366 hbb2cf487567423f
+  0x00013a80 3945005f 5f72675f 6f6f6d00 5f5a4e38 9E.__rg_oom._ZN8
+  0x00013a90 736d616c 6c766563 3137536d 616c6c56 smallvec17SmallV
+  0x00013aa0 6563244c 54244124 47542431 31747279 ec$LT$A$GT$11try
+  0x00013ab0 5f726573 65727665 31376835 31373933 _reserve17h51793
+  0x00013ac0 30373863 66623565 36643845 005f5a4e 078cfb5e6d8E._ZN
+  0x00013ad0 36305f24 4c542473 74642e2e 74696d65 60_$LT$std..time
+  0x00013ae0 2e2e496e 7374616e 74247532 30246173 ..Instant$u20$as
+  0x00013af0 24753230 24636f72 652e2e6f 70732e2e $u20$core..ops..
+  0x00013b00 61726974 682e2e53 75622447 54243373 arith..Sub$GT$3s
+  0x00013b10 75623137 68616464 30636463 64383033 ub17hadd0cdcd803
+  0x00013b20 32613264 61450061 6e6f6e2e 30646261 2a2daE.anon.0dba
+  0x00013b30 33643263 61616366 34353866 63343433 3d2caacf458fc443
+  0x00013b40 31313735 37333631 62633361 2e302e6c 11757361bc3a.0.l
+  0x00013b50 6c766d2e 31313231 33383839 37363336 lvm.112138897636
+  0x00013b60 30353633 33343933 005f5a4e 3470796f 05633493._ZN4pyo
+  0x00013b70 33357479 70657335 7475706c 65375079 35types5tuple7Py
+  0x00013b80 5475706c 65313867 65745f69 74656d5f Tuple18get_item_
+  0x00013b90 756e6368 65636b65 64313768 63363766 unchecked17hc67f
+  0x00013ba0 34386336 65393032 32656265 45005f5a 48c6e9022ebeE._Z
+  0x00013bb0 4e37325f 244c5424 70796f33 2e2e6578 N72_$LT$pyo3..ex
+  0x00013bc0 63657074 696f6e73 2e2e5079 426c6f63 ceptions..PyBloc
+  0x00013bd0 6b696e67 494f4572 726f7224 75323024 kingIOError$u20$
+  0x00013be0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00013bf0 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
+  0x00013c00 37686534 64643834 32616534 61666365 7he4dd842ae4afce
+  0x00013c10 32334500 5f5a4e37 305f244c 54247079 23E._ZN70_$LT$py
+  0x00013c20 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x00013c30 50794261 73654578 63657074 696f6e24 PyBaseException$
+  0x00013c40 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x00013c50 2e666d74 2e2e4465 62756724 47542433 .fmt..Debug$GT$3
+  0x00013c60 666d7431 37686664 31653730 63396233 fmt17hfd1e70c9b3
+  0x00013c70 38376436 32394500 5f5a4e34 70796f33 87d629E._ZN4pyo3
+  0x00013c80 3367696c 3847494c 47756172 64313761 3gil8GILGuard17a
+  0x00013c90 63717569 72655f75 6e636865 636b6564 cquire_unchecked
+  0x00013ca0 31376830 38653461 65323738 35613131 17h08e4ae2785a11
+  0x00013cb0 31623245 2e6c6c76 6d2e3133 32333838 1b2E.llvm.132388
+  0x00013cc0 39333433 32323030 36393232 3236005f 93432200692226._
+  0x00013cd0 5a4e3463 6f726533 6f707338 66756e63 ZN4core3ops8func
+  0x00013ce0 74696f6e 36466e4f 6e636534 3063616c tion6FnOnce40cal
+  0x00013cf0 6c5f6f6e 63652475 37622424 75376224 l_once$u7b$$u7b$
+  0x00013d00 76746162 6c652e73 68696d24 75376424 vtable.shim$u7d$
+  0x00013d10 24753764 24313768 37643565 66623161 $u7d$17h7d5efb1a
+  0x00013d20 37626366 31333962 452e6c6c 766d2e33 7bcf139bE.llvm.3
+  0x00013d30 31363039 30373238 31383830 37383131 1609072818807811
+  0x00013d40 3233005f 5a4e3463 6f726533 70747231 23._ZN4core3ptr1
+  0x00013d50 32336472 6f705f69 6e5f706c 61636524 23drop_in_place$
+  0x00013d60 4c542470 796f332e 2e657272 2e2e6572 LT$pyo3..err..er
+  0x00013d70 725f7374 6174652e 2e626f78 65645f61 r_state..boxed_a
+  0x00013d80 72677324 4c542463 6f72652e 2e6e756d rgs$LT$core..num
+  0x00013d90 2e2e6572 726f722e 2e547279 46726f6d ..error..TryFrom
+  0x00013da0 496e7445 72726f72 24475424 2e2e2475 IntError$GT$..$u
+  0x00013db0 37622424 75376224 636c6f73 75726524 7b$$u7b$closure$
+  0x00013dc0 75376424 24753764 24244754 24313768 u7d$$u7d$$GT$17h
+  0x00013dd0 37326664 32376366 61636535 38643163 72fd27cface58d1c
+  0x00013de0 452e6c6c 766d2e33 31363039 30373238 E.llvm.316090728
+  0x00013df0 31383830 37383131 3233005f 5a4e3931 1880781123._ZN91
+  0x00013e00 5f244c54 24737464 2e2e7061 6e69636b _$LT$std..panick
+  0x00013e10 696e672e 2e626567 696e5f70 616e6963 ing..begin_panic
+  0x00013e20 2e2e5061 6e696350 61796c6f 6164244c ..PanicPayload$L
+  0x00013e30 54244124 47542424 75323024 61732475 T$A$GT$$u20$as$u
+  0x00013e40 32302463 6f72652e 2e70616e 69632e2e 20$core..panic..
+  0x00013e50 426f784d 65557024 47542433 67657431 BoxMeUp$GT$3get1
+  0x00013e60 37686438 37633039 32643937 39326565 7hd87c092d9792ee
+  0x00013e70 65304500 5f5a4e34 636f7265 33666d74 e0E._ZN4core3fmt
+  0x00013e80 38627569 6c646572 73384465 62756753 8builders8DebugS
+  0x00013e90 65743565 6e747279 31376837 39363131 et5entry17h79611
+  0x00013ea0 34346564 31626131 66313645 005f5f72 44ed1ba1f16E.__r
+  0x00013eb0 7573745f 616c6c6f 635f6572 726f725f ust_alloc_error_
+  0x00013ec0 68616e64 6c65725f 73686f75 6c645f70 handler_should_p
+  0x00013ed0 616e6963 005f5a4e 33737464 3570616e anic._ZN3std5pan
+  0x00013ee0 69633133 72657375 6d655f75 6e77696e ic13resume_unwin
+  0x00013ef0 64313768 62306432 61313863 37376132 d17hb0d2a18c77a2
+  0x00013f00 33646536 45005f5a 4e347079 6f333869 3de6E._ZN4pyo38i
+  0x00013f10 6e737461 6e636531 3250794e 61746976 nstance12PyNativ
+  0x00013f20 65547970 65313875 6e636865 636b6564 eType18unchecked
+  0x00013f30 5f646f77 6e636173 74313768 65333835 _downcast17he385
+  0x00013f40 34396632 31363633 33346134 45005f5a 49f2166334a4E._Z
+  0x00013f50 4e337374 64337379 7334756e 69783137 N3std3sys4unix17
+  0x00013f60 74687265 61645f6c 6f63616c 5f64746f thread_local_dto
+  0x00013f70 72313372 65676973 7465725f 64746f72 r13register_dtor
+  0x00013f80 31376831 33653639 33383166 63313063 17h13e69381fc10c
+  0x00013f90 34666445 005f5a4e 3130375f 244c5424 4fdE._ZN107_$LT$
+  0x00013fa0 7374642e 2e73796e 632e2e6d 7073632e std..sync..mpsc.
+  0x00013fb0 2e526563 7654696d 656f7574 4572726f .RecvTimeoutErro
+  0x00013fc0 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
+  0x00013fd0 652e2e63 6f6e7665 72742e2e 46726f6d e..convert..From
+  0x00013fe0 244c5424 7374642e 2e73796e 632e2e6d $LT$std..sync..m
+  0x00013ff0 7073632e 2e526563 76457272 6f722447 psc..RecvError$G
+  0x00014000 54242447 54243466 726f6d31 37683830 T$$GT$4from17h80
+  0x00014010 39666561 65383363 32356161 38614500 9feae83c25aa8aE.
+  0x00014020 5f5a4e34 636f7265 3970616e 69636b69 _ZN4core9panicki
+  0x00014030 6e673138 70616e69 635f6e6f 756e7769 ng18panic_nounwi
+  0x00014040 6e645f66 6d743137 68353230 38333364 nd_fmt17h520833d
+  0x00014050 31343437 66343865 3945005f 5a4e3373 1447f48e9E._ZN3s
+  0x00014060 74643373 79733475 6e697835 73746469 td3sys4unix5stdi
+  0x00014070 6f313270 616e6963 5f6f7574 70757431 o12panic_output1
+  0x00014080 37683139 61323534 30333861 31666465 7h19a254038a1fde
+  0x00014090 31384500 616e6f6e 2e376239 34366165 18E.anon.7b946ae
+  0x000140a0 31643361 36363637 39376532 64623166 1d3a666797e2db1f
+  0x000140b0 33366534 63643665 372e3135 2e6c6c76 36e4cd6e7.15.llv
+  0x000140c0 6d2e3138 33353637 35303438 35363134 m.18356750485614
+  0x000140d0 35313331 32390061 6e6f6e2e 36383266 513129.anon.682f
+  0x000140e0 30353362 61336436 64313461 66356232 053ba3d6d14af5b2
+  0x000140f0 37636663 62626431 36333633 2e322e6c 7cfcbbd16363.2.l
+  0x00014100 6c766d2e 35363937 39323937 36393133 lvm.569792976913
+  0x00014110 33303537 34373600 5f5a4e33 73746436 3057476._ZN3std6
+  0x00014120 74687265 61643979 69656c64 5f6e6f77 thread9yield_now
+  0x00014130 31376831 39383830 33616363 38306434 17h198803acc80d4
+  0x00014140 32323945 005f5a4e 34636f72 6533666d 229E._ZN4core3fm
+  0x00014150 7439466f 726d6174 74657232 36646562 t9Formatter26deb
+  0x00014160 75675f73 74727563 745f6669 656c6432 ug_struct_field2
+  0x00014170 5f66696e 69736831 37683639 30363138 _finish17h690618
+  0x00014180 31336632 62386432 34334500 5f5a4e34 13f2b8d243E._ZN4
+  0x00014190 70796f33 35747970 65733866 756e6374 pyo35types8funct
+  0x000141a0 696f6e31 31507943 46756e63 74696f6e ion11PyCFunction
+  0x000141b0 3132696e 7465726e 616c5f6e 65773137 12internal_new17
+  0x000141c0 68353335 61353336 66633031 37653163 h535a536fc017e1c
+  0x000141d0 3845005f 5a4e3638 5f244c54 2470796f 8E._ZN68_$LT$pyo
+  0x000141e0 332e2e74 79706573 2e2e6d61 7070696e 3..types..mappin
+  0x000141f0 672e2e50 794d6170 70696e67 24753230 g..PyMapping$u20
+  0x00014200 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00014210 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x00014220 31376863 63383163 34643966 34333633 17hcc81c4d9f4363
+  0x00014230 31386445 005f5a4e 33737464 36746872 18dE._ZN3std6thr
+  0x00014240 65616435 6c6f6361 6c346661 73743132 ead5local4fast12
+  0x00014250 4b657924 4c542454 24475424 31347472 Key$LT$T$GT$14tr
+  0x00014260 795f696e 69746961 6c697a65 31376838 y_initialize17h8
+  0x00014270 63343836 61393337 62623733 33666345 c486a937bb733fcE
+  0x00014280 2e6c6c76 6d2e3331 36303930 37323831 .llvm.3160907281
+  0x00014290 38383037 38313132 33005f5a 4e34636f 880781123._ZN4co
+  0x000142a0 72653970 616e6963 6b696e67 31387061 re9panicking18pa
+  0x000142b0 6e69635f 626f756e 64735f63 6865636b nic_bounds_check
+  0x000142c0 31376861 66303666 65666232 33656261 17haf06fefb23eba
+  0x000142d0 38326445 005f5a4e 35616c6c 6f633772 82dE._ZN5alloc7r
+  0x000142e0 61775f76 65633139 52617756 6563244c aw_vec19RawVec$L
+  0x000142f0 54245424 43244124 47542437 72657365 T$T$C$A$GT$7rese
+  0x00014300 72766532 31646f5f 72657365 7276655f rve21do_reserve_
+  0x00014310 616e645f 68616e64 6c653137 68613235 and_handle17ha25
+  0x00014320 64306238 33336331 66346263 3445005f d0b833c1f4bc4E._
+  0x00014330 5a4e3732 5f244c54 2470796f 332e2e65 ZN72_$LT$pyo3..e
+  0x00014340 78636570 74696f6e 732e2e50 7942726f xceptions..PyBro
+  0x00014350 6b656e50 69706545 72726f72 24753230 kenPipeError$u20
+  0x00014360 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00014370 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x00014380 31376863 37306236 63643736 37633234 17hc70b6cd767c24
+  0x00014390 36396445 005f5a4e 34636f72 6533666d 69dE._ZN4core3fm
+  0x000143a0 74336e75 6d35355f 244c5424 696d706c t3num55_$LT$impl
+  0x000143b0 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x000143c0 55707065 72486578 24753230 24666f72 UpperHex$u20$for
+  0x000143d0 24753230 24757369 7a652447 54243366 $u20$usize$GT$3f
+  0x000143e0 6d743137 68336238 64663766 37373433 mt17h3b8df7f7743
+  0x000143f0 61306263 3145005f 5a4e3733 5f244c54 a0bc1E._ZN73_$LT
+  0x00014400 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x00014410 732e2e61 73796e63 696f2e2e 51756575 s..asyncio..Queu
+  0x00014420 6546756c 6c247532 30246173 24753230 eFull$u20$as$u20
+  0x00014430 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
+  0x00014440 67244754 2433666d 74313768 61653136 g$GT$3fmt17hae16
+  0x00014450 62656139 33326136 63643363 45005f5a bea932a6cd3cE._Z
+  0x00014460 4e37365f 244c5424 70796f33 2e2e6578 N76_$LT$pyo3..ex
+  0x00014470 63657074 696f6e73 2e2e5079 46696c65 ceptions..PyFile
+  0x00014480 4e6f7446 6f756e64 4572726f 72247532 NotFoundError$u2
+  0x00014490 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x000144a0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
+  0x000144b0 666d7431 37683538 33393962 64326463 fmt17h58399bd2dc
+  0x000144c0 62323262 37664500 5f5a4e33 73746433 b22b7fE._ZN3std3
+  0x000144d0 656e7637 5f766172 5f6f7331 37686361 env7_var_os17hca
+  0x000144e0 36303439 37323462 64353037 30374500 6049724bd50707E.
+  0x000144f0 5f5a4e35 616c6c6f 6335736c 69636536 _ZN5alloc5slice6
+  0x00014500 345f244c 5424696d 706c2475 32302461 4_$LT$impl$u20$a
+  0x00014510 6c6c6f63 2e2e626f 72726f77 2e2e546f lloc..borrow..To
+  0x00014520 4f776e65 64247532 3024666f 72247532 Owned$u20$for$u2
+  0x00014530 30242475 35622454 24753564 24244754 0$$u5b$T$u5d$$GT
+  0x00014540 2438746f 5f6f776e 65643137 68623063 $8to_owned17hb0c
+  0x00014550 64376239 31646531 32323233 3545005f d7b91de122235E._
+  0x00014560 5f727573 745f616c 6c6f6300 5f5a4e35 _rust_alloc._ZN5
+  0x00014570 335f244c 54247079 6f332e2e 6572722e 3_$LT$pyo3..err.
+  0x00014580 2e507945 72722475 32302461 73247532 .PyErr$u20$as$u2
+  0x00014590 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x000145a0 75672447 54243366 6d743137 68396131 ug$GT$3fmt17h9a1
+  0x000145b0 61383565 64663339 61623761 6245005f a85edf39ab7abE._
+  0x000145c0 5a4e3738 5f244c54 2470796f 332e2e65 ZN78_$LT$pyo3..e
+  0x000145d0 78636570 74696f6e 732e2e50 79556e69 xceptions..PyUni
+  0x000145e0 636f6465 5472616e 736c6174 65457272 codeTranslateErr
+  0x000145f0 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x00014600 72652e2e 666d742e 2e446562 75672447 re..fmt..Debug$G
+  0x00014610 54243366 6d743137 68363964 61366437 T$3fmt17h69da6d7
+  0x00014620 63333737 63306632 3545005f 5a4e3732 c377c0f25E._ZN72
+  0x00014630 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x00014640 74696f6e 732e2e50 79426173 65457863 tions..PyBaseExc
+  0x00014650 65707469 6f6e2475 32302461 73247532 eption$u20$as$u2
+  0x00014660 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00014670 706c6179 24475424 33666d74 31376839 play$GT$3fmt17h9
+  0x00014680 66386131 66303435 30613832 30373745 f8a1f0450a82077E
+  0x00014690 005f5a4e 34636f72 6533666d 74386275 ._ZN4core3fmt8bu
+  0x000146a0 696c6465 72733130 44656275 67547570 ilders10DebugTup
+  0x000146b0 6c653666 696e6973 68313768 65613361 le6finish17hea3a
+  0x000146c0 39303564 62343638 61663537 45005f5a 905db468af57E._Z
+  0x000146d0 4e34636f 72653366 6d743946 6f726d61 N4core3fmt9Forma
+  0x000146e0 74746572 31327061 645f696e 74656772 tter12pad_integr
+  0x000146f0 616c3137 68363733 63613764 32396231 al17h673ca7d29b1
+  0x00014700 34333164 6245005f 5a4e3730 5f244c54 431dbE._ZN70_$LT
+  0x00014710 2470796f 332e2e65 78636570 74696f6e $pyo3..exception
+  0x00014720 732e2e50 79557365 72576172 6e696e67 s..PyUserWarning
+  0x00014730 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00014740 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
+  0x00014750 54243366 6d743137 68373039 64303466 T$3fmt17h709d04f
+  0x00014760 33323536 37633266 3145005f 5a4e3930 32567c2f1E._ZN90
+  0x00014770 5f244c54 24737464 2e2e7061 6e69636b _$LT$std..panick
+  0x00014780 696e672e 2e626567 696e5f70 616e6963 ing..begin_panic
+  0x00014790 5f68616e 646c6572 2e2e5061 6e696350 _handler..PanicP
+  0x000147a0 61796c6f 61642475 32302461 73247532 ayload$u20$as$u2
+  0x000147b0 3024636f 72652e2e 70616e69 632e2e42 0$core..panic..B
+  0x000147c0 6f784d65 55702447 54243874 616b655f oxMeUp$GT$8take_
+  0x000147d0 626f7831 37683333 32363866 38346634 box17h33268f84f4
+  0x000147e0 63366537 66364500 5f5a4e34 70796f33 c6e7f6E._ZN4pyo3
+  0x000147f0 3367696c 3947494c 5f434f55 4e54375f 3gil9GIL_COUNT7_
+  0x00014800 5f676574 6974355f 5f4b4559 31376862 _getit5__KEY17hb
+  0x00014810 64623538 35343265 64643037 32373445 db58542edd07274E
+  0x00014820 005f5a4e 37305f24 4c542470 796f332e ._ZN70_$LT$pyo3.
+  0x00014830 2e657863 65707469 6f6e732e 2e507953 .exceptions..PyS
+  0x00014840 796e7461 78457272 6f722475 32302461 yntaxError$u20$a
+  0x00014850 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00014860 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x00014870 31376862 65306431 31373134 31353661 17hbe0d11714156a
+  0x00014880 37656545 005f5a4e 34636f72 65337074 7eeE._ZN4core3pt
+  0x00014890 72353464 726f705f 696e5f70 6c616365 r54drop_in_place
+  0x000148a0 244c5424 24524624 6d757424 75323024 $LT$$RF$mut$u20$
+  0x000148b0 616c6c6f 632e2e73 7472696e 672e2e53 alloc..string..S
+  0x000148c0 7472696e 67244754 24313768 39623732 tring$GT$17h9b72
+  0x000148d0 35373836 32393737 33363433 452e6c6c 578629773643E.ll
+  0x000148e0 766d2e33 30343133 39333935 38353639 vm.3041393958569
+  0x000148f0 39373433 3439005f 5a4e3470 796f3331 974349._ZN4pyo31
+  0x00014900 31636f6e 76657273 696f6e73 33737464 1conversions3std
+  0x00014910 36737472 696e6736 385f244c 5424696d 6string68_$LT$im
+  0x00014920 706c2475 32302470 796f332e 2e636f6e pl$u20$pyo3..con
+  0x00014930 76657273 696f6e2e 2e46726f 6d50794f version..FromPyO
+  0x00014940 626a6563 74247532 3024666f 72247532 bject$u20$for$u2
+  0x00014950 30242452 46247374 72244754 24376578 0$$RF$str$GT$7ex
+  0x00014960 74726163 74313768 65346666 30316638 tract17he4ff01f8
+  0x00014970 66626166 62636239 45005f5a 4e35616c fbafbcb9E._ZN5al
+  0x00014980 6c6f6335 616c6c6f 63313868 616e646c loc5alloc18handl
+  0x00014990 655f616c 6c6f635f 6572726f 72313768 e_alloc_error17h
+  0x000149a0 30376564 62383761 61616232 34633334 07edb87aaab24c34
+  0x000149b0 45005f5a 4e34636f 72653370 74723730 E._ZN4core3ptr70
+  0x000149c0 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
+  0x000149d0 2470796f 332e2e69 6e737461 6e63652e $pyo3..instance.
+  0x000149e0 2e507924 4c542470 796f332e 2e747970 .Py$LT$pyo3..typ
+  0x000149f0 65732e2e 616e792e 2e507941 6e792447 es..any..PyAny$G
+  0x00014a00 54242447 54243137 68386365 62613632 T$$GT$17h8ceba62
+  0x00014a10 64626230 38346538 61452e6c 6c766d2e dbb084e8aE.llvm.
+  0x00014a20 33303431 33393339 35383536 39393734 3041393958569974
+  0x00014a30 33343900 5f5a4e34 636f7265 33707472 349._ZN4core3ptr
+  0x00014a40 38316472 6f705f69 6e5f706c 61636524 81drop_in_place$
+  0x00014a50 4c542463 6f72652e 2e6f7074 696f6e2e LT$core..option.
+  0x00014a60 2e4f7074 696f6e24 4c542470 796f332e .Option$LT$pyo3.
+  0x00014a70 2e657272 2e2e6572 725f7374 6174652e .err..err_state.
+  0x00014a80 2e507945 72725374 61746524 47542424 .PyErrState$GT$$
+  0x00014a90 47542431 37686338 30373966 36346633 GT$17hc8079f64f3
+  0x00014aa0 31623166 3130452e 6c6c766d 2e313338 1b1f10E.llvm.138
+  0x00014ab0 36313835 32373131 33393032 37343736 6185271139027476
+  0x00014ac0 00616e6f 6e2e6234 62633165 36646439 .anon.b4bc1e6dd9
+  0x00014ad0 30383334 32663362 62353465 36333633 08342f3bb54e6363
+  0x00014ae0 65663764 61382e32 302e6c6c 766d2e36 ef7da8.20.llvm.6
+  0x00014af0 35373230 36383037 31323833 38353839 5720680712838589
+  0x00014b00 3239005f 5a4e3732 5f244c54 2470796f 29._ZN72_$LT$pyo
+  0x00014b10 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00014b20 79436f6e 6e656374 696f6e45 72726f72 yConnectionError
+  0x00014b30 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00014b40 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
+  0x00014b50 33666d74 31376864 61613463 39376433 3fmt17hdaa4c97d3
+  0x00014b60 37623937 61383845 005f5a4e 34636f72 7b97a88E._ZN4cor
+  0x00014b70 65336f70 73386675 6e637469 6f6e3646 e3ops8function6F
+  0x00014b80 6e4f6e63 65343063 616c6c5f 6f6e6365 nOnce40call_once
+  0x00014b90 24753762 24247537 62247674 61626c65 $u7b$$u7b$vtable
+  0x00014ba0 2e736869 6d247537 64242475 37642431 .shim$u7d$$u7d$1
+  0x00014bb0 37686265 62303937 34636636 35353031 7hbeb0974cf65501
+  0x00014bc0 6665452e 6c6c766d 2e363838 34373639 feE.llvm.6884769
+  0x00014bd0 30333534 35303335 36363730 005f5a4e 035450356670._ZN
+  0x00014be0 3470796f 33313174 7970655f 6f626a65 4pyo311type_obje
+  0x00014bf0 63743130 50795479 7065496e 666f3131 ct10PyTypeInfo11
+  0x00014c00 74797065 5f6f626a 65637431 37683337 type_object17h37
+  0x00014c10 38393764 32313739 34346134 33614500 897d217944a43aE.
+  0x00014c20 5f5a4e36 395f244c 54247079 6f332e2e _ZN69_$LT$pyo3..
+  0x00014c30 65786365 7074696f 6e732e2e 5079556e exceptions..PyUn
+  0x00014c40 69636f64 65457272 6f722475 32302461 icodeError$u20$a
+  0x00014c50 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00014c60 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x00014c70 68393762 65653737 61326632 38373362 h97bee77a2f2873b
+  0x00014c80 3845005f 5a4e3638 5f244c54 2470796f 8E._ZN68_$LT$pyo
+  0x00014c90 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00014ca0 79457863 65707469 6f6e2475 32302461 yException$u20$a
+  0x00014cb0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00014cc0 2e446973 706c6179 24475424 33666d74 .Display$GT$3fmt
+  0x00014cd0 31376833 36366262 36373133 61316431 17h366bb6713a1d1
+  0x00014ce0 30643045 005f5a4e 35385f24 4c542473 0d0E._ZN58_$LT$s
+  0x00014cf0 74642e2e 696f2e2e 6572726f 722e2e45 td..io..error..E
+  0x00014d00 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x00014d10 636f7265 2e2e666d 742e2e44 65627567 core..fmt..Debug
+  0x00014d20 24475424 33666d74 31376836 38646332 $GT$3fmt17h68dc2
+  0x00014d30 37306165 33653963 36386245 005f5a4e 70ae3e9c68bE._ZN
+  0x00014d40 35385f24 4c542461 6c6c6f63 2e2e7374 58_$LT$alloc..st
+  0x00014d50 72696e67 2e2e5374 72696e67 24753230 ring..String$u20
+  0x00014d60 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00014d70 742e2e57 72697465 24475424 31307772 t..Write$GT$10wr
+  0x00014d80 6974655f 63686172 31376831 62366436 ite_char17h1b6d6
+  0x00014d90 30366431 63623164 35623745 2e6c6c76 06d1cb1d5b7E.llv
+  0x00014da0 6d2e3536 39373932 39373639 31333330 m.56979297691330
+  0x00014db0 35373437 36005f5a 4e33365f 244c5424 57476._ZN36_$LT$
+  0x00014dc0 54247532 30246173 24753230 24636f72 T$u20$as$u20$cor
+  0x00014dd0 652e2e61 6e792e2e 416e7924 47542437 e..any..Any$GT$7
+  0x00014de0 74797065 5f696431 37683162 66666266 type_id17h1bffbf
+  0x00014df0 34323531 31636562 37324500 5f5a4e37 42511ceb72E._ZN7
+  0x00014e00 365f244c 54247079 6f332e2e 65786365 6_$LT$pyo3..exce
+  0x00014e10 7074696f 6e732e2e 50795a65 726f4469 ptions..PyZeroDi
+  0x00014e20 76697369 6f6e4572 726f7224 75323024 visionError$u20$
+  0x00014e30 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00014e40 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
+  0x00014e50 74313768 39663538 30626636 39643565 t17h9f580bf69d5e
+  0x00014e60 35643433 45005f5a 4e34636f 72653373 5d43E._ZN4core3s
+  0x00014e70 7472356c 6f737379 39557466 38436875 tr5lossy9Utf8Chu
+  0x00014e80 6e6b3769 6e76616c 69643137 68386164 nk7invalid17h8ad
+  0x00014e90 66626630 39316632 30396365 3845005f fbf091f209ce8E._
+  0x00014ea0 5a4e3373 74643674 68726561 64356c6f ZN3std6thread5lo
+  0x00014eb0 63616c34 66617374 31324b65 79244c54 cal4fast12Key$LT
+  0x00014ec0 24542447 54243134 7472795f 696e6974 $T$GT$14try_init
+  0x00014ed0 69616c69 7a653137 68353165 33323039 ialize17h51e3209
+  0x00014ee0 63623639 36343836 63452e6c 6c766d2e cb696486cE.llvm.
+  0x00014ef0 33313630 39303732 38313838 30373831 3160907281880781
+  0x00014f00 31323300 5f5a4e36 385f244c 54247079 123._ZN68_$LT$py
+  0x00014f10 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x00014f20 50795379 6e746178 4572726f 72247532 PySyntaxError$u2
+  0x00014f30 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00014f40 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x00014f50 74313768 38316339 38333435 65386536 t17h81c98345e8e6
+  0x00014f60 37643061 45005f5a 4e37375f 244c5424 7d0aE._ZN77_$LT$
+  0x00014f70 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x00014f80 2e2e5079 556e6963 6f646544 65636f64 ..PyUnicodeDecod
+  0x00014f90 65457272 6f722475 32302461 73247532 eError$u20$as$u2
+  0x00014fa0 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00014fb0 706c6179 24475424 33666d74 31376832 play$GT$3fmt17h2
+  0x00014fc0 31636236 63316531 37326232 66333945 1cb6c1e172b2f39E
+  0x00014fd0 005f5a4e 34325f24 4c542424 52462454 ._ZN42_$LT$$RF$T
+  0x00014fe0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00014ff0 2e2e666d 742e2e44 65627567 24475424 ..fmt..Debug$GT$
+  0x00015000 33666d74 31376838 30363861 30356463 3fmt17h8068a05dc
+  0x00015010 34353135 31373345 005f5a4e 34636f72 4515173E._ZN4cor
+  0x00015020 6533666d 74336e75 6d35335f 244c5424 e3fmt3num53_$LT$
+  0x00015030 696d706c 24753230 24636f72 652e2e66 impl$u20$core..f
+  0x00015040 6d742e2e 55707065 72486578 24753230 mt..UpperHex$u20
+  0x00015050 24666f72 24753230 24753332 24475424 $for$u20$u32$GT$
+  0x00015060 33666d74 31376866 34613163 35336665 3fmt17hf4a1c53fe
+  0x00015070 63346464 61653045 005f5a4e 34636f72 c4ddae0E._ZN4cor
+  0x00015080 65337074 72393264 726f705f 696e5f70 e3ptr92drop_in_p
+  0x00015090 6c616365 244c5424 7374642e 2e696f2e lace$LT$std..io.
+  0x000150a0 2e577269 74652e2e 77726974 655f666d .Write..write_fm
+  0x000150b0 742e2e41 64617074 6572244c 54247374 t..Adapter$LT$st
+  0x000150c0 642e2e73 79732e2e 756e6978 2e2e7374 d..sys..unix..st
+  0x000150d0 64696f2e 2e537464 65727224 47542424 dio..Stderr$GT$$
+  0x000150e0 47542431 37686334 61313330 63663065 GT$17hc4a130cf0e
+  0x000150f0 64366231 3833452e 6c6c766d 2e383336 d6b183E.llvm.836
+  0x00015100 34373335 31373237 30333437 36333534 4735172703476354
+  0x00015110 005f5a4e 34636f72 65337074 72343464 ._ZN4core3ptr44d
+  0x00015120 726f705f 696e5f70 6c616365 244c5424 rop_in_place$LT$
+  0x00015130 636f7265 2e2e6365 6c6c2e2e 426f7272 core..cell..Borr
+  0x00015140 6f774572 726f7224 47542431 37683261 owError$GT$17h2a
+  0x00015150 33663964 34323430 33663831 6135452e 3f9d42403f81a5E.
+  0x00015160 6c6c766d 2e313332 33383839 33343332 llvm.13238893432
+  0x00015170 32303036 39323232 36005f5a 4e34636f 200692226._ZN4co
+  0x00015180 72653970 616e6963 6b696e67 3970616e re9panicking9pan
+  0x00015190 69635f66 6d743137 68663333 61313437 ic_fmt17hf33a147
+  0x000151a0 35623464 63356333 6545005f 5a4e3735 5b4dc5c3eE._ZN75
+  0x000151b0 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x000151c0 74696f6e 732e2e50 79446570 72656361 tions..PyDepreca
+  0x000151d0 74696f6e 5761726e 696e6724 75323024 tionWarning$u20$
+  0x000151e0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x000151f0 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
+  0x00015200 37686465 39656634 66386461 35313466 7hde9ef4f8da514f
+  0x00015210 61324500 5f5a4e34 636f7265 3570616e a2E._ZN4core5pan
+  0x00015220 69633130 70616e69 635f696e 666f3950 ic10panic_info9P
+  0x00015230 616e6963 496e666f 386c6f63 6174696f anicInfo8locatio
+  0x00015240 6e313768 62663566 64616235 33636534 n17hbf5fdab53ce4
+  0x00015250 65653235 45005f5a 4e38335f 244c5424 ee25E._ZN83_$LT$
+  0x00015260 7061726b 696e675f 6c6f745f 636f7265 parking_lot_core
+  0x00015270 2e2e7061 726b696e 675f6c6f 742e2e54 ..parking_lot..T
+  0x00015280 68726561 64446174 61247532 30246173 hreadData$u20$as
+  0x00015290 24753230 24636f72 652e2e6f 70732e2e $u20$core..ops..
+  0x000152a0 64726f70 2e2e4472 6f702447 54243464 drop..Drop$GT$4d
+  0x000152b0 726f7031 37683239 32323837 39623261 rop17h2922879b2a
+  0x000152c0 37643230 61304500 5f5a4e37 395f244c 7d20a0E._ZN79_$L
+  0x000152d0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x000152e0 6e732e2e 5079436f 6e6e6563 74696f6e ns..PyConnection
+  0x000152f0 41626f72 74656445 72726f72 24753230 AbortedError$u20
+  0x00015300 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00015310 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x00015320 31376835 35396339 31366463 36663133 17h559c916dc6f13
+  0x00015330 64633245 00616e6f 6e2e3933 62663464 dc2E.anon.93bf4d
+  0x00015340 37316633 31323138 33313132 38353630 71f3121831128560
+  0x00015350 32336462 38376333 63382e30 2e6c6c76 23db87c3c8.0.llv
+  0x00015360 6d2e3638 38343736 39303335 34353033 m.68847690354503
+  0x00015370 35363637 3000616e 6f6e2e62 39613034 56670.anon.b9a04
+  0x00015380 38366330 30613431 37326237 62316163 86c00a4172b7b1ac
+  0x00015390 35326233 31356161 3461332e 302e6c6c 52b315aa4a3.0.ll
+  0x000153a0 766d2e31 33323338 38393334 33323230 vm.1323889343220
+  0x000153b0 30363932 32323600 5f5a4e33 73746439 0692226._ZN3std9
+  0x000153c0 70616e69 636b696e 67313264 65666175 panicking12defau
+  0x000153d0 6c745f68 6f6f6b31 37686133 35303064 lt_hook17ha3500d
+  0x000153e0 61353761 61346163 34664500 5f5a4e33 a57aa4ac4fE._ZN3
+  0x000153f0 73746434 70617468 34506174 68366973 std4path4Path6is
+  0x00015400 5f646972 31376836 66313166 35326265 _dir17h6f11f52be
+  0x00015410 66313330 62333945 005f5a4e 33737464 f130b39E._ZN3std
+  0x00015420 3970616e 69636b69 6e673448 4f4f4b31 9panicking4HOOK1
+  0x00015430 37683762 62363361 36346164 35303130 7h7bb63a64ad5010
+  0x00015440 38374500 5f5a4e34 636f7265 33707472 87E._ZN4core3ptr
+  0x00015450 31323164 726f705f 696e5f70 6c616365 121drop_in_place
+  0x00015460 244c5424 70796f33 2e2e6572 722e2e65 $LT$pyo3..err..e
+  0x00015470 72725f73 74617465 2e2e626f 7865645f rr_state..boxed_
+  0x00015480 61726773 244c5424 636f7265 2e2e6e75 args$LT$core..nu
+  0x00015490 6d2e2e65 72726f72 2e2e5061 72736549 m..error..ParseI
+  0x000154a0 6e744572 726f7224 4754242e 2e247537 ntError$GT$..$u7
+  0x000154b0 62242475 37622463 6c6f7375 72652475 b$$u7b$closure$u
+  0x000154c0 37642424 75376424 24475424 31376862 7d$$u7d$$GT$17hb
+  0x000154d0 62336531 65616638 31623839 31383045 b3e1eaf81b89180E
+  0x000154e0 2e6c6c76 6d2e3331 36303930 37323831 .llvm.3160907281
+  0x000154f0 38383037 38313132 33005f5a 4e38325f 880781123._ZN82_
+  0x00015500 244c5424 70796f33 2e2e6578 63657074 $LT$pyo3..except
+  0x00015510 696f6e73 2e2e5079 50656e64 696e6744 ions..PyPendingD
+  0x00015520 65707265 63617469 6f6e5761 726e696e eprecationWarnin
+  0x00015530 67247532 30246173 24753230 24636f72 g$u20$as$u20$cor
+  0x00015540 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
+  0x00015550 2433666d 74313768 63346264 36646335 $3fmt17hc4bd6dc5
+  0x00015560 35366362 65643438 4500616e 6f6e2e62 56cbed48E.anon.b
+  0x00015570 39613034 38366330 30613431 37326237 9a0486c00a4172b7
+  0x00015580 62316163 35326233 31356161 3461332e b1ac52b315aa4a3.
+  0x00015590 34302e6c 6c766d2e 31333233 38383933 40.llvm.13238893
+  0x000155a0 34333232 30303639 32323236 005f5a4e 432200692226._ZN
+  0x000155b0 34636f72 65337074 72343864 726f705f 4core3ptr48drop_
+  0x000155c0 696e5f70 6c616365 244c5424 636f7265 in_place$LT$core
+  0x000155d0 2e2e7374 722e2e65 72726f72 2e2e5574 ..str..error..Ut
+  0x000155e0 66384572 726f7224 47542431 37683263 f8Error$GT$17h2c
+  0x000155f0 65333464 33643064 39326633 3064452e e34d3d0d92f30dE.
+  0x00015600 6c6c766d 2e313736 39353736 32333431 llvm.17695762341
+  0x00015610 37383134 35333031 32005f5a 4e337374 781453012._ZN3st
+  0x00015620 64367468 72656164 356c6f63 616c3466 d6thread5local4f
+  0x00015630 61737431 324b6579 244c5424 54244754 ast12Key$LT$T$GT
+  0x00015640 24313474 72795f69 6e697469 616c697a $14try_initializ
+  0x00015650 65313768 39373761 64363839 66643363 e17h977ad689fd3c
+  0x00015660 35323833 452e6c6c 766d2e31 31323030 5283E.llvm.11200
+  0x00015670 37313335 34313431 32383731 35383900 713541412871589.
+  0x00015680 5f5a4e34 70796f33 31317479 70655f6f _ZN4pyo311type_o
+  0x00015690 626a6563 74313050 79547970 65496e66 bject10PyTypeInf
+  0x000156a0 6f313174 7970655f 6f626a65 63743137 o11type_object17
+  0x000156b0 68623034 66613436 62666561 35353231 hb04fa46bfea5521
+  0x000156c0 3645005f 5a4e366d 656d6368 72366d65 6E._ZN6memchr6me
+  0x000156d0 6d636872 33783836 34737365 32366d65 mchr3x864sse26me
+  0x000156e0 6d636872 31376864 31383261 61666264 mchr17hd182aafbd
+  0x000156f0 36353033 36393345 005f5a4e 33737464 6503693E._ZN3std
+  0x00015700 3570616e 69633139 6765745f 6261636b 5panic19get_back
+  0x00015710 74726163 655f7374 796c6531 37686161 trace_style17haa
+  0x00015720 38316132 34373134 64616565 33334500 81a24714daee33E.
+  0x00015730 5f5a4e34 636f7265 33707472 34376472 _ZN4core3ptr47dr
+  0x00015740 6f705f69 6e5f706c 61636524 4c542463 op_in_place$LT$c
+  0x00015750 6f72652e 2e63656c 6c2e2e42 6f72726f ore..cell..Borro
+  0x00015760 774d7574 4572726f 72244754 24313768 wMutError$GT$17h
+  0x00015770 62646538 30656166 63623765 63303262 bde80eafcb7ec02b
+  0x00015780 452e6c6c 766d2e31 33323338 38393334 E.llvm.132388934
+  0x00015790 33323230 30363932 32323600 5f5a4e39 32200692226._ZN9
+  0x000157a0 385f244c 5424616c 6c6f632e 2e766563 8_$LT$alloc..vec
+  0x000157b0 2e2e5665 63244c54 24542447 54242475 ..Vec$LT$T$GT$$u
+  0x000157c0 32302461 73247532 3024616c 6c6f632e 20$as$u20$alloc.
+  0x000157d0 2e766563 2e2e7370 65635f66 726f6d5f .vec..spec_from_
+  0x000157e0 69746572 2e2e5370 65634672 6f6d4974 iter..SpecFromIt
+  0x000157f0 6572244c 54245424 43244924 47542424 er$LT$T$C$I$GT$$
+  0x00015800 47542439 66726f6d 5f697465 72313768 GT$9from_iter17h
+  0x00015810 31663861 63626366 33323464 64643433 1f8acbcf324ddd43
+  0x00015820 45005f5a 4e347079 6f333367 696c3133 E._ZN4pyo33gil13
+  0x00015830 4f574e45 445f4f42 4a454354 53375f5f OWNED_OBJECTS7__
+  0x00015840 67657469 74355f5f 4b455931 37686265 getit5__KEY17hbe
+  0x00015850 65643033 35386262 35653939 38364500 ed0358bb5e9986E.
+  0x00015860 5f5a4e38 385f244c 54247374 642e2e74 _ZN88_$LT$std..t
+  0x00015870 696d652e 2e496e73 74616e74 24753230 ime..Instant$u20
+  0x00015880 24617324 75323024 636f7265 2e2e6f70 $as$u20$core..op
+  0x00015890 732e2e61 72697468 2e2e4164 64244c54 s..arith..Add$LT
+  0x000158a0 24636f72 652e2e74 696d652e 2e447572 $core..time..Dur
+  0x000158b0 6174696f 6e244754 24244754 24336164 ation$GT$$GT$3ad
+  0x000158c0 64313768 30363536 36633361 39343834 d17h06566c3a9484
+  0x000158d0 31613530 45005f5a 4e37375f 244c5424 1a50E._ZN77_$LT$
+  0x000158e0 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x000158f0 2e2e5079 44657072 65636174 696f6e57 ..PyDeprecationW
+  0x00015900 61726e69 6e672475 32302461 73247532 arning$u20$as$u2
+  0x00015910 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00015920 706c6179 24475424 33666d74 31376836 play$GT$3fmt17h6
+  0x00015930 33366236 62336633 32313033 39616445 36b6b3f321039adE
+  0x00015940 00616e6f 6e2e3762 39343661 65316433 .anon.7b946ae1d3
+  0x00015950 61363636 37393765 32646231 66333665 a666797e2db1f36e
+  0x00015960 34636436 65372e39 2e6c6c76 6d2e3138 4cd6e7.9.llvm.18
+  0x00015970 33353637 35303438 35363134 35313331 3567504856145131
+  0x00015980 3239005f 5a4e3730 5f244c54 2470796f 29._ZN70_$LT$pyo
+  0x00015990 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x000159a0 794c6f6f 6b757045 72726f72 24753230 yLookupError$u20
+  0x000159b0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x000159c0 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x000159d0 6d743137 68623535 66623537 64323564 mt17hb55fb57d25d
+  0x000159e0 63366439 3745005f 5a4e3434 5f244c54 c6d97E._ZN44_$LT
+  0x000159f0 24245246 24542475 32302461 73247532 $$RF$T$u20$as$u2
+  0x00015a00 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00015a10 706c6179 24475424 33666d74 31376833 play$GT$3fmt17h3
+  0x00015a20 38373232 39383435 63333431 33666245 87229845c3413fbE
+  0x00015a30 005f5a4e 36375f24 4c542470 796f332e ._ZN67_$LT$pyo3.
+  0x00015a40 2e657863 65707469 6f6e732e 2e507956 .exceptions..PyV
+  0x00015a50 616c7565 4572726f 72247532 30246173 alueError$u20$as
+  0x00015a60 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00015a70 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x00015a80 34633931 64393230 30373330 34353938 4c91d92007304598
+  0x00015a90 4500616e 6f6e2e62 39613034 38366330 E.anon.b9a0486c0
+  0x00015aa0 30613431 37326237 62316163 35326233 0a4172b7b1ac52b3
+  0x00015ab0 31356161 3461332e 33392e6c 6c766d2e 15aa4a3.39.llvm.
+  0x00015ac0 31333233 38383933 34333232 30303639 1323889343220069
+  0x00015ad0 32323236 005f5a4e 33737464 34706174 2226._ZN3std4pat
+  0x00015ae0 68345061 74683133 5f737472 69705f70 h4Path13_strip_p
+  0x00015af0 72656669 78313768 39613265 61383537 refix17h9a2ea857
+  0x00015b00 39333134 61383361 45005f5a 4e34636f 9314a83aE._ZN4co
+  0x00015b10 72653370 74723135 3564726f 705f696e re3ptr155drop_in
+  0x00015b20 5f706c61 6365244c 54247061 726b696e _place$LT$parkin
+  0x00015b30 675f6c6f 742e2e6f 6e63652e 2e4f6e63 g_lot..once..Onc
+  0x00015b40 652e2e63 616c6c5f 6f6e6365 5f666f72 e..call_once_for
+  0x00015b50 6365244c 54247079 6f332e2e 67696c2e ce$LT$pyo3..gil.
+  0x00015b60 2e47494c 47756172 642e2e61 63717569 .GILGuard..acqui
+  0x00015b70 72652e2e 24753762 24247537 6224636c re..$u7b$$u7b$cl
+  0x00015b80 6f737572 65247537 64242475 37642424 osure$u7d$$u7d$$
+  0x00015b90 4754242e 2e247537 62242475 37622463 GT$..$u7b$$u7b$c
+  0x00015ba0 6c6f7375 72652475 37642424 75376424 losure$u7d$$u7d$
+  0x00015bb0 24475424 31376830 37376630 30326534 $GT$17h077f002e4
+  0x00015bc0 32653237 32633745 2e6c6c76 6d2e3133 2e272c7E.llvm.13
+  0x00015bd0 32333838 39333433 32323030 36393232 2388934322006922
+  0x00015be0 3236005f 5a4e3938 5f244c54 24616c6c 26._ZN98_$LT$all
+  0x00015bf0 6f632e2e 73747269 6e672e2e 53747269 oc..string..Stri
+  0x00015c00 6e672475 32302461 73247532 3024636f ng$u20$as$u20$co
+  0x00015c10 72652e2e 636f6e76 6572742e 2e46726f re..convert..Fro
+  0x00015c20 6d244c54 24616c6c 6f632e2e 626f7272 m$LT$alloc..borr
+  0x00015c30 6f772e2e 436f7724 4c542473 74722447 ow..Cow$LT$str$G
+  0x00015c40 54242447 54242447 54243466 726f6d31 T$$GT$$GT$4from1
+  0x00015c50 37683132 66386531 63313037 65346438 7h12f8e1c107e4d8
+  0x00015c60 31654500 616e6f6e 2e653965 62323337 1eE.anon.e9eb237
+  0x00015c70 63663530 61343362 36356436 33366230 cf50a43b65d636b0
+  0x00015c80 66343737 30623034 652e3238 2e6c6c76 f4770b04e.28.llv
+  0x00015c90 6d2e3133 38363138 35323731 31333930 m.13861852711390
+  0x00015ca0 32373437 36005f5a 4e35616c 6c6f6336 27476._ZN5alloc6
+  0x00015cb0 73747269 6e673653 7472696e 67313566 string6String15f
+  0x00015cc0 726f6d5f 75746638 5f6c6f73 73793137 rom_utf8_lossy17
+  0x00015cd0 68663363 30313339 64626365 64616666 hf3c0139dbcedaff
+  0x00015ce0 3045005f 5a4e3463 6f726533 70747237 0E._ZN4core3ptr7
+  0x00015cf0 3164726f 705f696e 5f706c61 6365244c 1drop_in_place$L
+  0x00015d00 5424636f 72652e2e 72657375 6c742e2e T$core..result..
+  0x00015d10 52657375 6c74244c 54246936 34244324 Result$LT$i64$C$
+  0x00015d20 70796f33 2e2e6572 722e2e50 79457272 pyo3..err..PyErr
+  0x00015d30 24475424 24475424 31376833 64333236 $GT$$GT$17h3d326
+  0x00015d40 62353337 33303161 32333145 2e6c6c76 b537301a231E.llv
+  0x00015d50 6d2e3138 33353637 35303438 35363134 m.18356750485614
+  0x00015d60 35313331 3239005f 5a4e3463 6f726533 513129._ZN4core3
+  0x00015d70 70747239 3764726f 705f696e 5f706c61 ptr97drop_in_pla
+  0x00015d80 6365244c 54247079 6f332e2e 6572722e ce$LT$pyo3..err.
+  0x00015d90 2e657272 5f737461 74652e2e 626f7865 .err_state..boxe
+  0x00015da0 645f6172 6773244c 54242452 46247374 d_args$LT$$RF$st
+  0x00015db0 72244754 242e2e24 75376224 24753762 r$GT$..$u7b$$u7b
+  0x00015dc0 24636c6f 73757265 24753764 24247537 $closure$u7d$$u7
+  0x00015dd0 64242447 54243137 68613561 39316530 d$$GT$17ha5a91e0
+  0x00015de0 38316462 62336361 36452e6c 6c766d2e 81dbb3ca6E.llvm.
+  0x00015df0 36383834 37363930 33353435 30333536 6884769035450356
+  0x00015e00 36373000 5f5a4e34 636f7265 37756e69 670._ZN4core7uni
+  0x00015e10 636f6465 3132756e 69636f64 655f6461 code12unicode_da
+  0x00015e20 74613263 63366c6f 6f6b7570 31376865 ta2cc6lookup17he
+  0x00015e30 65396430 61663736 38646134 62393345 e9d0af768da4b93E
+  0x00015e40 005f5a4e 37355f24 4c542470 796f332e ._ZN75_$LT$pyo3.
+  0x00015e50 2e657863 65707469 6f6e732e 2e507946 .exceptions..PyF
+  0x00015e60 6c6f6174 696e6750 6f696e74 4572726f loatingPointErro
+  0x00015e70 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
+  0x00015e80 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
+  0x00015e90 2433666d 74313768 61656433 38363831 $3fmt17haed38681
+  0x00015ea0 30336561 61326666 45005f5a 4e36315f 03eaa2ffE._ZN61_
+  0x00015eb0 244c5424 70796f33 2e2e6769 6c2e2e47 $LT$pyo3..gil..G
+  0x00015ec0 494c4775 61726424 75323024 61732475 ILGuard$u20$as$u
+  0x00015ed0 32302463 6f72652e 2e6f7073 2e2e6472 20$core..ops..dr
+  0x00015ee0 6f702e2e 44726f70 24475424 3464726f op..Drop$GT$4dro
+  0x00015ef0 70313768 37373135 61666566 63653237 p17h7715afefce27
+  0x00015f00 62386564 45005f5a 4e37345f 244c5424 b8edE._ZN74_$LT$
+  0x00015f10 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x00015f20 2e2e5079 5a65726f 44697669 73696f6e ..PyZeroDivision
+  0x00015f30 4572726f 72247532 30246173 24753230 Error$u20$as$u20
+  0x00015f40 24636f72 652e2e66 6d742e2e 44656275 $core..fmt..Debu
+  0x00015f50 67244754 2433666d 74313768 32386538 g$GT$3fmt17h28e8
+  0x00015f60 34653836 61346234 36363139 45005f5a 4e86a4b46619E._Z
+  0x00015f70 4e347079 6f333131 74797065 5f6f626a N4pyo311type_obj
+  0x00015f80 65637431 30507954 79706549 6e666f31 ect10PyTypeInfo1
+  0x00015f90 31747970 655f6f62 6a656374 31376863 1type_object17hc
+  0x00015fa0 35333731 39613337 62663235 32313045 53719a37bf25210E
+  0x00015fb0 005f5a4e 34636f72 65337374 7235636f ._ZN4core3str5co
+  0x00015fc0 756e7432 33636861 725f636f 756e745f unt23char_count_
+  0x00015fd0 67656e65 72616c5f 63617365 31376865 general_case17he
+  0x00015fe0 61333562 62323438 62643064 36623745 a35bb248bd0d6b7E
+  0x00015ff0 00616e6f 6e2e3937 61643933 31633534 .anon.97ad931c54
+  0x00016000 63383835 63613936 64666437 32656631 c885ca96dfd72ef1
+  0x00016010 30616230 33382e31 332e6c6c 766d2e33 0ab038.13.llvm.3
+  0x00016020 30343133 39333935 38353639 39373433 0413939585699743
+  0x00016030 3439005f 5a4e3736 5f244c54 2470796f 49._ZN76_$LT$pyo
+  0x00016040 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00016050 79556e62 6f756e64 4c6f6361 6c457272 yUnboundLocalErr
+  0x00016060 6f722475 32302461 73247532 3024636f or$u20$as$u20$co
+  0x00016070 72652e2e 666d742e 2e446973 706c6179 re..fmt..Display
+  0x00016080 24475424 33666d74 31376839 61376464 $GT$3fmt17h9a7dd
+  0x00016090 66663534 36346439 37666445 005f5a4e ff5464d97fdE._ZN
+  0x000160a0 37325f24 4c542470 796f332e 2e657863 72_$LT$pyo3..exc
+  0x000160b0 65707469 6f6e732e 2e507950 65726d69 eptions..PyPermi
+  0x000160c0 7373696f 6e457272 6f722475 32302461 ssionError$u20$a
+  0x000160d0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x000160e0 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x000160f0 68616634 65303437 65316466 39356638 haf4e047e1df95f8
+  0x00016100 3045005f 5a4e3638 5f244c54 24636f72 0E._ZN68_$LT$cor
+  0x00016110 652e2e6e 756d2e2e 6572726f 722e2e50 e..num..error..P
+  0x00016120 61727365 496e7445 72726f72 24753230 arseIntError$u20
+  0x00016130 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00016140 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x00016150 31376864 65616134 33373163 33343465 17hdeaa4371c344e
+  0x00016160 38663045 00616e6f 6e2e6539 65623233 8f0E.anon.e9eb23
+  0x00016170 37636635 30613433 62363564 36333662 7cf50a43b65d636b
+  0x00016180 30663437 37306230 34652e35 312e6c6c 0f4770b04e.51.ll
+  0x00016190 766d2e31 33383631 38353237 31313339 vm.1386185271139
+  0x000161a0 30323734 3736005f 5a4e3463 6f726533 027476._ZN4core3
+  0x000161b0 70747235 3064726f 705f696e 5f706c61 ptr50drop_in_pla
+  0x000161c0 6365244c 5424616c 6c6f632e 2e626f72 ce$LT$alloc..bor
+  0x000161d0 726f772e 2e436f77 244c5424 73747224 row..Cow$LT$str$
+  0x000161e0 47542424 47542431 37686232 31633831 GT$$GT$17hb21c81
+  0x000161f0 35346535 38663066 6336452e 6c6c766d 54e58f0fc6E.llvm
+  0x00016200 2e313338 36313835 32373131 33393032 .138618527113902
+  0x00016210 37343736 005f5a4e 34636f72 65397061 7476._ZN4core9pa
+  0x00016220 6e69636b 696e6731 39617373 6572745f nicking19assert_
+  0x00016230 6661696c 65645f69 6e6e6572 31376861 failed_inner17ha
+  0x00016240 66393831 36323237 62323062 36663245 f9816227b20b6f2E
+  0x00016250 005f5a4e 39315f24 4c542473 74642e2e ._ZN91_$LT$std..
+  0x00016260 70616e69 636b696e 672e2e62 6567696e panicking..begin
+  0x00016270 5f70616e 69632e2e 50616e69 63506179 _panic..PanicPay
+  0x00016280 6c6f6164 244c5424 41244754 24247532 load$LT$A$GT$$u2
+  0x00016290 30246173 24753230 24636f72 652e2e70 0$as$u20$core..p
+  0x000162a0 616e6963 2e2e426f 784d6555 70244754 anic..BoxMeUp$GT
+  0x000162b0 24387461 6b655f62 6f783137 68393666 $8take_box17h96f
+  0x000162c0 31653733 33373735 63366637 3145005f 1e733775c6f71E._
+  0x000162d0 5a4e3373 74643970 616e6963 6b696e67 ZN3std9panicking
+  0x000162e0 31317061 6e69635f 636f756e 74313769 11panic_count17i
+  0x000162f0 735f7a65 726f5f73 6c6f775f 70617468 s_zero_slow_path
+  0x00016300 31376831 63313931 36393664 34356234 17h1c191696d45b4
+  0x00016310 38336245 005f5a4e 34636f72 6533666d 83bE._ZN4core3fm
+  0x00016320 74336e75 6d33696d 7035325f 244c5424 t3num3imp52_$LT$
+  0x00016330 696d706c 24753230 24636f72 652e2e66 impl$u20$core..f
+  0x00016340 6d742e2e 44697370 6c617924 75323024 mt..Display$u20$
+  0x00016350 666f7224 75323024 69333224 47542433 for$u20$i32$GT$3
+  0x00016360 666d7431 37686264 37393461 33336666 fmt17hbd794a33ff
+  0x00016370 65623761 62634500 5f5a4e37 345f244c eb7abcE._ZN74_$L
+  0x00016380 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x00016390 6e732e2e 50794b65 79626f61 7264496e ns..PyKeyboardIn
+  0x000163a0 74657272 75707424 75323024 61732475 terrupt$u20$as$u
+  0x000163b0 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x000163c0 62756724 47542433 666d7431 37683363 bug$GT$3fmt17h3c
+  0x000163d0 64363063 32343534 35356366 36664500 d60c245455cf6fE.
+  0x000163e0 5f5a4e39 315f244c 54247374 642e2e73 _ZN91_$LT$std..s
+  0x000163f0 79735f63 6f6d6d6f 6e2e2e62 61636b74 ys_common..backt
+  0x00016400 72616365 2e2e5f70 72696e74 2e2e4469 race.._print..Di
+  0x00016410 73706c61 79426163 6b747261 63652475 splayBacktrace$u
+  0x00016420 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x00016430 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x00016440 33666d74 31376835 37373964 37626637 3fmt17h5779d7bf7
+  0x00016450 66373063 62306345 005f5f72 7573745f f70cb0cE.__rust_
+  0x00016460 70616e69 635f636c 65616e75 7000616e panic_cleanup.an
+  0x00016470 6f6e2e33 34376432 36346533 34656233 on.347d264e34eb3
+  0x00016480 61306337 34626535 61383966 38393561 a0c74be5a89f895a
+  0x00016490 6337652e 36332e6c 6c766d2e 31373639 c7e.63.llvm.1769
+  0x000164a0 35373632 33343137 38313435 33303132 5762341781453012
+  0x000164b0 005f5a4e 36345f24 4c542473 74642e2e ._ZN64_$LT$std..
+  0x000164c0 7379732e 2e756e69 782e2e73 7464696f sys..unix..stdio
+  0x000164d0 2e2e5374 646f7574 24753230 24617324 ..Stdout$u20$as$
+  0x000164e0 75323024 7374642e 2e696f2e 2e577269 u20$std..io..Wri
+  0x000164f0 74652447 54243566 6c757368 31376835 te$GT$5flush17h5
+  0x00016500 34323733 38656637 62376331 31353745 42738ef7b7c1157E
+  0x00016510 005f5a4e 3470796f 33336572 72355079 ._ZN4pyo33err5Py
+  0x00016520 45727231 3066726f 6d5f7661 6c756531 Err10from_value1
+  0x00016530 37683763 65643665 37393965 64623862 7h7ced6e799edb8b
+  0x00016540 38364500 5f5a4e34 636f7265 33666d74 86E._ZN4core3fmt
+  0x00016550 39466f72 6d617474 65723235 64656275 9Formatter25debu
+  0x00016560 675f7475 706c655f 6669656c 64315f66 g_tuple_field1_f
+  0x00016570 696e6973 68313768 36376134 36363963 inish17h67a4669c
+  0x00016580 33303234 35333434 45005f5a 4e347079 30245344E._ZN4py
+  0x00016590 6f333131 636f6e76 65727369 6f6e7333 o311conversions3
+  0x000165a0 73746436 73747269 6e673133 335f244c std6string133_$L
+  0x000165b0 5424696d 706c2475 32302470 796f332e T$impl$u20$pyo3.
+  0x000165c0 2e636f6e 76657273 696f6e2e 2e496e74 .conversion..Int
+  0x000165d0 6f507924 4c542470 796f332e 2e696e73 oPy$LT$pyo3..ins
+  0x000165e0 74616e63 652e2e50 79244c54 2470796f tance..Py$LT$pyo
+  0x000165f0 332e2e74 79706573 2e2e616e 792e2e50 3..types..any..P
+  0x00016600 79416e79 24475424 24475424 24753230 yAny$GT$$GT$$u20
+  0x00016610 24666f72 24753230 24616c6c 6f632e2e $for$u20$alloc..
+  0x00016620 73747269 6e672e2e 53747269 6e672447 string..String$G
+  0x00016630 54243769 6e746f5f 70793137 68343161 T$7into_py17h41a
+  0x00016640 62383739 63393639 38663230 6545005f b879c9698f20eE._
+  0x00016650 5a4e3732 5f244c54 2470796f 332e2e65 ZN72_$LT$pyo3..e
+  0x00016660 78636570 74696f6e 732e2e50 7946696c xceptions..PyFil
+  0x00016670 65457869 73747345 72726f72 24753230 eExistsError$u20
+  0x00016680 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00016690 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x000166a0 31376865 32613530 33646131 65396533 17he2a503da1e9e3
+  0x000166b0 39653145 00616e6f 6e2e6239 61303438 9e1E.anon.b9a048
+  0x000166c0 36633030 61343137 32623762 31616335 6c00a4172b7b1ac5
+  0x000166d0 32623331 35616134 61332e35 312e6c6c 2b315aa4a3.51.ll
+  0x000166e0 766d2e31 33323338 38393334 33323230 vm.1323889343220
+  0x000166f0 30363932 32323600 5f5a4e36 385f244c 0692226._ZN68_$L
+  0x00016700 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x00016710 6e732e2e 50795479 70654572 726f7224 ns..PyTypeError$
+  0x00016720 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x00016730 2e666d74 2e2e4469 73706c61 79244754 .fmt..Display$GT
+  0x00016740 2433666d 74313768 62306161 61653038 $3fmt17hb0aaae08
+  0x00016750 31666336 32636264 4500616e 6f6e2e39 1fc62cbdE.anon.9
+  0x00016760 65313134 65643530 31306436 32353362 e114ed5010d6253b
+  0x00016770 64323631 31323934 37336364 3138382e d261129473cd188.
+  0x00016780 352e6c6c 766d2e38 33363437 33353137 5.llvm.836473517
+  0x00016790 32373033 34373633 3534005f 5a4e3463 2703476354._ZN4c
+  0x000167a0 6f726533 66666935 635f7374 72344353 ore3ffi5c_str4CS
+  0x000167b0 74723674 6f5f7374 72313768 37356237 tr6to_str17h75b7
+  0x000167c0 62613766 64636534 32363630 45005f5a ba7fdce42660E._Z
+  0x000167d0 4e34636f 72653370 74723132 3264726f N4core3ptr122dro
+  0x000167e0 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
+  0x000167f0 6f332e2e 6572722e 2e657272 5f737461 o3..err..err_sta
+  0x00016800 74652e2e 626f7865 645f6172 6773244c te..boxed_args$L
+  0x00016810 5424244c 5024616c 6c6f632e 2e737472 T$$LP$alloc..str
+  0x00016820 696e672e 2e537472 696e6724 43242452 ing..String$C$$R
+  0x00016830 50242447 54242e2e 24753762 24247537 P$$GT$..$u7b$$u7
+  0x00016840 6224636c 6f737572 65247537 64242475 b$closure$u7d$$u
+  0x00016850 37642424 47542431 37683533 34386461 7d$$GT$17h5348da
+  0x00016860 32353363 35643364 3932452e 6c6c766d 253c5d3d92E.llvm
+  0x00016870 2e333136 30393037 32383138 38303738 .316090728188078
+  0x00016880 31313233 00616e6f 6e2e6239 61303438 1123.anon.b9a048
+  0x00016890 36633030 61343137 32623762 31616335 6c00a4172b7b1ac5
+  0x000168a0 32623331 35616134 61332e31 332e6c6c 2b315aa4a3.13.ll
+  0x000168b0 766d2e31 33323338 38393334 33323230 vm.1323889343220
+  0x000168c0 30363932 32323600 5f5a4e37 305f244c 0692226._ZN70_$L
+  0x000168d0 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x000168e0 6e732e2e 50794675 74757265 5761726e ns..PyFutureWarn
+  0x000168f0 696e6724 75323024 61732475 32302463 ing$u20$as$u20$c
+  0x00016900 6f72652e 2e666d74 2e2e4465 62756724 ore..fmt..Debug$
+  0x00016910 47542433 666d7431 37686239 35303363 GT$3fmt17hb9503c
+  0x00016920 61356364 31636264 37394500 5f5a4e37 a5cd1cbd79E._ZN7
+  0x00016930 315f244c 54247079 6f332e2e 65786365 1_$LT$pyo3..exce
+  0x00016940 7074696f 6e732e2e 50794173 73657274 ptions..PyAssert
+  0x00016950 696f6e45 72726f72 24753230 24617324 ionError$u20$as$
+  0x00016960 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x00016970 65627567 24475424 33666d74 31376839 ebug$GT$3fmt17h9
+  0x00016980 39356266 38626136 32323265 30376245 95bf8ba6222e07bE
+  0x00016990 005f5a4e 37335f24 4c542470 796f332e ._ZN73_$LT$pyo3.
+  0x000169a0 2e657863 65707469 6f6e732e 2e507941 .exceptions..PyA
+  0x000169b0 74747269 62757465 4572726f 72247532 ttributeError$u2
+  0x000169c0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x000169d0 6d742e2e 44697370 6c617924 47542433 mt..Display$GT$3
+  0x000169e0 666d7431 37683231 66363834 31386430 fmt17h21f68418d0
+  0x000169f0 64653463 31374500 5f5a4e34 636f7265 de4c17E._ZN4core
+  0x00016a00 33737472 356c6f73 73793130 55746638 3str5lossy10Utf8
+  0x00016a10 4368756e 6b73336e 65773137 68623334 Chunks3new17hb34
+  0x00016a20 39306162 34663166 35636139 3645005f 90ab4f1f5ca96E._
+  0x00016a30 5a4e3463 6f726533 73747231 39736c69 ZN4core3str19sli
+  0x00016a40 63655f65 72726f72 5f666169 6c5f7274 ce_error_fail_rt
+  0x00016a50 31376864 64613439 62656434 64373136 17hdda49bed4d716
+  0x00016a60 31623845 005f5a4e 3470796f 33357479 1b8E._ZN4pyo35ty
+  0x00016a70 70657337 666c6f61 746f6231 31355f24 pes7floatob115_$
+  0x00016a80 4c542469 6d706c24 75323024 70796f33 LT$impl$u20$pyo3
+  0x00016a90 2e2e636f 6e766572 73696f6e 2e2e496e ..conversion..In
+  0x00016aa0 746f5079 244c5424 70796f33 2e2e696e toPy$LT$pyo3..in
+  0x00016ab0 7374616e 63652e2e 5079244c 54247079 stance..Py$LT$py
+  0x00016ac0 6f332e2e 74797065 732e2e61 6e792e2e o3..types..any..
+  0x00016ad0 5079416e 79244754 24244754 24247532 PyAny$GT$$GT$$u2
+  0x00016ae0 3024666f 72247532 30246633 32244754 0$for$u20$f32$GT
+  0x00016af0 2437696e 746f5f70 79313768 30653962 $7into_py17h0e9b
+  0x00016b00 30303963 61633336 30646466 45005f5a 009cac360ddfE._Z
+  0x00016b10 4e37395f 244c5424 70796f33 2e2e7479 N79_$LT$pyo3..ty
+  0x00016b20 7065732e 2e737472 696e672e 2e507953 pes..string..PyS
+  0x00016b30 7472696e 67247532 30246173 24753230 tring$u20$as$u20
+  0x00016b40 2470796f 332e2e74 7970655f 6f626a65 $pyo3..type_obje
+  0x00016b50 63742e2e 50795479 7065496e 666f2447 ct..PyTypeInfo$G
+  0x00016b60 54243130 69735f74 7970655f 6f663137 T$10is_type_of17
+  0x00016b70 68316336 65346431 35613134 61326532 h1c6e4d15a14a2e2
+  0x00016b80 3445005f 5a4e3470 796f3335 74797065 4E._ZN4pyo35type
+  0x00016b90 73357475 706c6537 50795475 706c6534 s5tuple7PyTuple4
+  0x00016ba0 69746572 31376863 66353363 36333534 iter17hcf53c6354
+  0x00016bb0 33633332 64636345 00616e6f 6e2e3965 3c32dccE.anon.9e
+  0x00016bc0 31313465 64353031 30643632 35336264 114ed5010d6253bd
+  0x00016bd0 32363131 32393437 33636431 38382e30 261129473cd188.0
+  0x00016be0 2e6c6c76 6d2e3833 36343733 35313732 .llvm.8364735172
+  0x00016bf0 37303334 37363335 34005f5a 4e356769 703476354._ZN5gi
+  0x00016c00 6d6c6934 72656164 346c696e 65374c69 mli4read4line7Li
+  0x00016c10 6e65526f 77313861 70706c79 5f6c696e neRow18apply_lin
+  0x00016c20 655f6164 76616e63 65313768 66323138 e_advance17hf218
+  0x00016c30 32336466 63613739 61633836 45005f5a 23dfca79ac86E._Z
+  0x00016c40 4e34636f 72653366 6d743946 6f726d61 N4core3fmt9Forma
+  0x00016c50 74746572 32366465 6275675f 73747275 tter26debug_stru
+  0x00016c60 63745f66 69656c64 315f6669 6e697368 ct_field1_finish
+  0x00016c70 31376865 37393364 63613436 39383165 17he793dca46981e
+  0x00016c80 35316145 005f5a4e 3470796f 33336572 51aE._ZN4pyo33er
+  0x00016c90 72355079 45727231 356d616b 655f6e6f r5PyErr15make_no
+  0x00016ca0 726d616c 697a6564 31376839 36656464 rmalized17h96edd
+  0x00016cb0 61626237 32326233 65633545 005f5a4e abb722b3ec5E._ZN
+  0x00016cc0 3567696d 6c693472 65616434 756e6974 5gimli4read4unit
+  0x00016cd0 3230616c 6c6f775f 73656374 696f6e5f 20allow_section_
+  0x00016ce0 6f666673 65743137 68633262 62656664 offset17hc2bbefd
+  0x00016cf0 39353439 39666665 3945005f 5a4e3470 95499ffe9E._ZN4p
+  0x00016d00 796f3333 67696c31 334f574e 45445f4f yo33gil13OWNED_O
+  0x00016d10 424a4543 5453375f 5f676574 69743137 BJECTS7__getit17
+  0x00016d20 68396461 36353339 63316130 66373066 h9da6539c1a0f70f
+  0x00016d30 63452e6c 6c766d2e 31333233 38383933 cE.llvm.13238893
+  0x00016d40 34333232 30303639 32323236 005f5a4e 432200692226._ZN
+  0x00016d50 34636f72 6533666d 74357772 69746531 4core3fmt5write1
+  0x00016d60 37683561 34626161 66663162 63643365 7h5a4baaff1bcd3e
+  0x00016d70 62354500 616e6f6e 2e353130 35626464 b5E.anon.5105bdd
+  0x00016d80 37396632 33623131 37316633 38373432 79f23b1171f38742
+  0x00016d90 66656161 63356431 372e3333 2e6c6c76 feaac5d17.33.llv
+  0x00016da0 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x00016db0 38313132 33005f5a 4e39315f 244c5424 81123._ZN91_$LT$
+  0x00016dc0 7374642e 2e70616e 69636b69 6e672e2e std..panicking..
+  0x00016dd0 62656769 6e5f7061 6e69632e 2e50616e begin_panic..Pan
+  0x00016de0 69635061 796c6f61 64244c54 24412447 icPayload$LT$A$G
+  0x00016df0 54242475 32302461 73247532 3024636f T$$u20$as$u20$co
+  0x00016e00 72652e2e 70616e69 632e2e42 6f784d65 re..panic..BoxMe
+  0x00016e10 55702447 54243874 616b655f 626f7831 Up$GT$8take_box1
+  0x00016e20 37686430 63393935 38353736 39336633 7hd0c995857693f3
+  0x00016e30 37614500 5f5a4e37 315f244c 54247079 7aE._ZN71_$LT$py
+  0x00016e40 6f332e2e 696d706c 5f2e2e70 616e6963 o3..impl_..panic
+  0x00016e50 2e2e5061 6e696354 72617024 75323024 ..PanicTrap$u20$
+  0x00016e60 61732475 32302463 6f72652e 2e6f7073 as$u20$core..ops
+  0x00016e70 2e2e6472 6f702e2e 44726f70 24475424 ..drop..Drop$GT$
+  0x00016e80 3464726f 70313768 34356133 64363432 4drop17h45a3d642
+  0x00016e90 35313836 36363131 45005f5a 4e37325f 51866611E._ZN72_
+  0x00016ea0 244c5424 70796f33 2e2e7479 7065732e $LT$pyo3..types.
+  0x00016eb0 2e747261 63656261 636b2e2e 50795472 .traceback..PyTr
+  0x00016ec0 61636562 61636b24 75323024 61732475 aceback$u20$as$u
+  0x00016ed0 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x00016ee0 62756724 47542433 666d7431 37683130 bug$GT$3fmt17h10
+  0x00016ef0 66653036 36336636 66363537 34394500 fe0663f6f65749E.
+  0x00016f00 5f5a4e31 316d696e 697a5f6f 78696465 _ZN11miniz_oxide
+  0x00016f10 37696e66 6c617465 34636f72 65313064 7inflate4core10d
+  0x00016f20 65636f6d 70726573 73313768 37393535 ecompress17h7955
+  0x00016f30 34643231 66323565 37393132 45005f5a 4d21f25e7912E._Z
+  0x00016f40 4e37305f 244c5424 70796f33 2e2e6578 N70_$LT$pyo3..ex
+  0x00016f50 63657074 696f6e73 2e2e5079 47656e65 ceptions..PyGene
+  0x00016f60 7261746f 72457869 74247532 30246173 ratorExit$u20$as
+  0x00016f70 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00016f80 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x00016f90 31333364 32363634 36633565 39303835 133d26646c5e9085
+  0x00016fa0 45005f5a 4e36345f 244c5424 72757374 E._ZN64_$LT$rust
+  0x00016fb0 635f6465 6d616e67 6c652e2e 76302e2e c_demangle..v0..
+  0x00016fc0 4964656e 74247532 30246173 24753230 Ident$u20$as$u20
+  0x00016fd0 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
+  0x00016fe0 6c617924 47542433 666d7431 37683865 lay$GT$3fmt17h8e
+  0x00016ff0 38333236 66613733 39656463 35344500 8326fa739edc54E.
+  0x00017000 5f5a4e34 636f7265 33666d74 35577269 _ZN4core3fmt5Wri
+  0x00017010 74653977 72697465 5f666d74 31376832 te9write_fmt17h2
+  0x00017020 63636535 31313161 37316136 65626145 cce5111a71a6ebaE
+  0x00017030 005f5a4e 39325f24 4c542470 796f332e ._ZN92_$LT$pyo3.
+  0x00017040 2e657272 2e2e5079 446f776e 63617374 .err..PyDowncast
+  0x00017050 4572726f 72417267 756d656e 74732475 ErrorArguments$u
+  0x00017060 32302461 73247532 30247079 6f332e2e 20$as$u20$pyo3..
+  0x00017070 6572722e 2e657272 5f737461 74652e2e err..err_state..
+  0x00017080 50794572 72417267 756d656e 74732447 PyErrArguments$G
+  0x00017090 54243961 7267756d 656e7473 31376864 T$9arguments17hd
+  0x000170a0 34333262 62663636 61323532 31633145 432bbf66a2521c1E
+  0x000170b0 00616e6f 6e2e3531 30356264 64373966 .anon.5105bdd79f
+  0x000170c0 32336231 31373166 33383734 32666561 23b1171f38742fea
+  0x000170d0 61633564 31372e31 392e6c6c 766d2e33 ac5d17.19.llvm.3
+  0x000170e0 31363039 30373238 31383830 37383131 1609072818807811
+  0x000170f0 3233005f 5a4e3561 6c6c6f63 35616c6c 23._ZN5alloc5all
+  0x00017100 6f633862 6f785f66 72656531 37683664 oc8box_free17h6d
+  0x00017110 36306465 32653865 37303762 6464452e 60de2e8e707bddE.
+  0x00017120 6c6c766d 2e313833 35363735 30343835 llvm.18356750485
+  0x00017130 36313435 31333132 39005f5a 4e313170 614513129._ZN11p
+  0x00017140 61726b69 6e675f6c 6f74346f 6e636534 arking_lot4once4
+  0x00017150 4f6e6365 31346361 6c6c5f6f 6e63655f Once14call_once_
+  0x00017160 736c6f77 31376835 39393035 62653633 slow17h59905be63
+  0x00017170 66333838 36316345 00616e6f 6e2e3334 f38861cE.anon.34
+  0x00017180 37643236 34653334 65623361 30633734 7d264e34eb3a0c74
+  0x00017190 62653561 38396638 39356163 37652e31 be5a89f895ac7e.1
+  0x000171a0 332e6c6c 766d2e31 37363935 37363233 3.llvm.176957623
+  0x000171b0 34313738 31343533 30313200 616e6f6e 41781453012.anon
+  0x000171c0 2e393761 64393331 63353463 38383563 .97ad931c54c885c
+  0x000171d0 61393664 66643732 65663130 61623033 a96dfd72ef10ab03
+  0x000171e0 382e362e 6c6c766d 2e333034 31333933 8.6.llvm.3041393
+  0x000171f0 39353835 36393937 34333439 005f5a4e 958569974349._ZN
+  0x00017200 34636f72 6533666d 74336e75 6d35335f 4core3fmt3num53_
+  0x00017210 244c5424 696d706c 24753230 24636f72 $LT$impl$u20$cor
+  0x00017220 652e2e66 6d742e2e 4c6f7765 72486578 e..fmt..LowerHex
+  0x00017230 24753230 24666f72 24753230 24753634 $u20$for$u20$u64
+  0x00017240 24475424 33666d74 31376863 64613764 $GT$3fmt17hcda7d
+  0x00017250 39623131 34383031 35376345 005f5a4e 9b11480157cE._ZN
+  0x00017260 37345f24 4c542470 796f332e 2e657863 74_$LT$pyo3..exc
+  0x00017270 65707469 6f6e732e 2e617379 6e63696f eptions..asyncio
+  0x00017280 2e2e5175 65756545 6d707479 24753230 ..QueueEmpty$u20
+  0x00017290 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x000172a0 742e2e44 65627567 24475424 33666d74 t..Debug$GT$3fmt
+  0x000172b0 31376837 35323732 36643865 66323261 17h752726d8ef22a
+  0x000172c0 30333245 005f5a4e 33737464 33737973 032E._ZN3std3sys
+  0x000172d0 34756e69 78356c6f 636b7331 31667574 4unix5locks11fut
+  0x000172e0 65785f6d 75746578 354d7574 65783134 ex_mutex5Mutex14
+  0x000172f0 6c6f636b 5f636f6e 74656e64 65643137 lock_contended17
+  0x00017300 68303433 34616464 66633633 62613830 h0434addfc63ba80
+  0x00017310 6245005f 5a4e3635 5f244c54 2470796f bE._ZN65_$LT$pyo
+  0x00017320 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00017330 79454f46 4572726f 72247532 30246173 yEOFError$u20$as
+  0x00017340 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00017350 44656275 67244754 2433666d 74313768 Debug$GT$3fmt17h
+  0x00017360 38353238 61393937 64363939 33663265 8528a997d6993f2e
+  0x00017370 45005f5a 4e34636f 72653366 66693563 E._ZN4core3ffi5c
+  0x00017380 5f737472 34435374 72386672 6f6d5f70 _str4CStr8from_p
+  0x00017390 74723973 74726c65 6e5f7274 31376862 tr9strlen_rt17hb
+  0x000173a0 61353530 65356163 36366133 61613845 a550e5ac66a3aa8E
+  0x000173b0 005f5a4e 39315f24 4c542473 74642e2e ._ZN91_$LT$std..
+  0x000173c0 70616e69 636b696e 672e2e72 7573745f panicking..rust_
+  0x000173d0 70616e69 635f7769 74686f75 745f686f panic_without_ho
+  0x000173e0 6f6b2e2e 52657772 6170426f 78247532 ok..RewrapBox$u2
+  0x000173f0 30246173 24753230 24636f72 652e2e70 0$as$u20$core..p
+  0x00017400 616e6963 2e2e426f 784d6555 70244754 anic..BoxMeUp$GT
+  0x00017410 24387461 6b655f62 6f783137 68376533 $8take_box17h7e3
+  0x00017420 39656439 30613662 38653139 6445005f 9ed90a6b8e19dE._
+  0x00017430 5a4e3561 6c6c6f63 35616c6c 6f633862 ZN5alloc5alloc8b
+  0x00017440 6f785f66 72656531 37683664 36306465 ox_free17h6d60de
+  0x00017450 32653865 37303762 6464452e 6c6c766d 2e8e707bddE.llvm
+  0x00017460 2e333136 30393037 32383138 38303738 .316090728188078
+  0x00017470 31313233 005f5a4e 36345f24 4c542470 1123._ZN64_$LT$p
+  0x00017480 796f332e 2e657863 65707469 6f6e732e yo3..exceptions.
+  0x00017490 2e507957 61726e69 6e672475 32302461 .PyWarning$u20$a
+  0x000174a0 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x000174b0 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x000174c0 68343730 33353731 65386437 63656335 h4703571e8d7cec5
+  0x000174d0 6645005f 5a4e3373 74643365 6e763131 fE._ZN3std3env11
+  0x000174e0 63757272 656e745f 64697231 37683566 current_dir17h5f
+  0x000174f0 62326565 37663930 65366236 36394500 b2ee7f90e6b669E.
+  0x00017500 5f5a4e37 325f244c 54247079 6f332e2e _ZN72_$LT$pyo3..
+  0x00017510 65786365 7074696f 6e732e2e 5079496d exceptions..PyIm
+  0x00017520 706f7274 5761726e 696e6724 75323024 portWarning$u20$
+  0x00017530 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00017540 2e2e4469 73706c61 79244754 2433666d ..Display$GT$3fm
+  0x00017550 74313768 31396563 33613662 34626361 t17h19ec3a6b4bca
+  0x00017560 38646238 45005f5a 4e337374 64397061 8db8E._ZN3std9pa
+  0x00017570 6e69636b 696e6733 74727937 636c6561 nicking3try7clea
+  0x00017580 6e757031 37683061 36343564 35343939 nup17h0a645d5499
+  0x00017590 34326364 33314500 5f5a4e35 616c6c6f 42cd31E._ZN5allo
+  0x000175a0 63377261 775f7665 63313166 696e6973 c7raw_vec11finis
+  0x000175b0 685f6772 6f773137 68376432 39663838 h_grow17h7d29f88
+  0x000175c0 34623162 30663831 32452e6c 6c766d2e 4b1b0f812E.llvm.
+  0x000175d0 35373637 37393037 36343736 38303731 5767790764768071
+  0x000175e0 30333400 5f5a4e33 73746433 656e7631 034._ZN3std3env1
+  0x000175f0 31637572 72656e74 5f657865 31376866 1current_exe17hf
+  0x00017600 35666136 34373363 39653839 31666545 5fa6473c9e891feE
+  0x00017610 005f5a4e 34636f72 6533666d 74336e75 ._ZN4core3fmt3nu
+  0x00017620 6d35355f 244c5424 696d706c 24753230 m55_$LT$impl$u20
+  0x00017630 24636f72 652e2e66 6d742e2e 4c6f7765 $core..fmt..Lowe
+  0x00017640 72486578 24753230 24666f72 24753230 rHex$u20$for$u20
+  0x00017650 24697369 7a652447 54243366 6d743137 $isize$GT$3fmt17
+  0x00017660 68386264 34636331 33633532 31656339 h8bd4cc13c521ec9
+  0x00017670 3445005f 5a4e3734 5f244c54 2470796f 4E._ZN74_$LT$pyo
+  0x00017680 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00017690 79526573 6f757263 65576172 6e696e67 yResourceWarning
+  0x000176a0 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x000176b0 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
+  0x000176c0 54243366 6d743137 68613038 61303863 T$3fmt17ha08a08c
+  0x000176d0 34653864 33383832 3545005f 5a4e3734 4e8d38825E._ZN74
+  0x000176e0 5f244c54 2470796f 332e2e65 78636570 _$LT$pyo3..excep
+  0x000176f0 74696f6e 732e2e50 79436869 6c645072 tions..PyChildPr
+  0x00017700 6f636573 73457272 6f722475 32302461 ocessError$u20$a
+  0x00017710 73247532 3024636f 72652e2e 666d742e s$u20$core..fmt.
+  0x00017720 2e446562 75672447 54243366 6d743137 .Debug$GT$3fmt17
+  0x00017730 68313561 36306137 61306530 37636366 h15a60a7a0e07ccf
+  0x00017740 3545005f 5a4e3732 5f244c54 2470796f 5E._ZN72_$LT$pyo
+  0x00017750 332e2e65 78636570 74696f6e 732e2e50 3..exceptions..P
+  0x00017760 794f7665 72666c6f 77457272 6f722475 yOverflowError$u
+  0x00017770 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x00017780 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x00017790 33666d74 31376831 34633065 38353361 3fmt17h14c0e853a
+  0x000177a0 30353562 61356345 00616e6f 6e2e3762 055ba5cE.anon.7b
+  0x000177b0 39343661 65316433 61363636 37393765 946ae1d3a666797e
+  0x000177c0 32646231 66333665 34636436 65372e37 2db1f36e4cd6e7.7
+  0x000177d0 2e6c6c76 6d2e3138 33353637 35303438 .llvm.1835675048
+  0x000177e0 35363134 35313331 32390061 6e6f6e2e 5614513129.anon.
+  0x000177f0 65393133 36643463 63326632 62663733 e9136d4cc2f2bf73
+  0x00017800 33643539 32623564 66383839 35323037 3d592b5df8895207
+  0x00017810 2e342e6c 6c766d2e 31373336 38373534 .4.llvm.17368754
+  0x00017820 32343034 36383033 33353630 005f5a4e 240468033560._ZN
+  0x00017830 3567696d 6c693472 65616436 61626272 5gimli4read6abbr
+  0x00017840 65763130 41747472 69627574 65733470 ev10Attributes4p
+  0x00017850 75736831 37683831 62353438 61326532 ush17h81b548a2e2
+  0x00017860 61656238 36644500 5f5a4e37 325f244c aeb86dE._ZN72_$L
+  0x00017870 54247079 6f332e2e 65786365 7074696f T$pyo3..exceptio
+  0x00017880 6e732e2e 50794765 6e657261 746f7245 ns..PyGeneratorE
+  0x00017890 78697424 75323024 61732475 32302463 xit$u20$as$u20$c
+  0x000178a0 6f72652e 2e666d74 2e2e4469 73706c61 ore..fmt..Displa
+  0x000178b0 79244754 2433666d 74313768 37346133 y$GT$3fmt17h74a3
+  0x000178c0 33306136 65663239 30313236 4500616e 30a6ef290126E.an
+  0x000178d0 6f6e2e65 39656232 33376366 35306134 on.e9eb237cf50a4
+  0x000178e0 33623635 64363336 62306634 37373062 3b65d636b0f4770b
+  0x000178f0 3034652e 32332e6c 6c766d2e 31333836 04e.23.llvm.1386
+  0x00017900 31383532 37313133 39303237 34373600 185271139027476.
+  0x00017910 5f5a4e36 365f244c 5424636f 72652e2e _ZN66_$LT$core..
+  0x00017920 6f707469 6f6e2e2e 4f707469 6f6e244c option..Option$L
+  0x00017930 54245424 47542424 75323024 61732475 T$T$GT$$u20$as$u
+  0x00017940 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x00017950 62756724 47542433 666d7431 37683039 bug$GT$3fmt17h09
+  0x00017960 62663231 31306264 62613861 34344500 bf2110bdba8a44E.
+  0x00017970 5f5a4e36 385f244c 54242452 46242475 _ZN68_$LT$$RF$$u
+  0x00017980 35622475 38247535 64242475 32302461 5b$u8$u5d$$u20$a
+  0x00017990 73247532 30246f62 6a656374 2e2e7265 s$u20$object..re
+  0x000179a0 61642e2e 72656164 5f726566 2e2e5265 ad..read_ref..Re
+  0x000179b0 61645265 66244754 24313372 6561645f adRef$GT$13read_
+  0x000179c0 62797465 735f6174 31376866 33613562 bytes_at17hf3a5b
+  0x000179d0 63313665 34376132 36653645 005f5a4e c16e47a26e6E._ZN
+  0x000179e0 3470796f 33357479 70657337 666c6f61 4pyo35types7floa
+  0x000179f0 746f6236 345f244c 5424696d 706c2475 tob64_$LT$impl$u
+  0x00017a00 32302470 796f332e 2e636f6e 76657273 20$pyo3..convers
+  0x00017a10 696f6e2e 2e46726f 6d50794f 626a6563 ion..FromPyObjec
+  0x00017a20 74247532 3024666f 72247532 30246633 t$u20$for$u20$f3
+  0x00017a30 32244754 24376578 74726163 74313768 2$GT$7extract17h
+  0x00017a40 66383733 66336639 30343637 32623130 f873f3f904672b10
+  0x00017a50 45005f5a 4e36385f 244c5424 70796f33 E._ZN68_$LT$pyo3
+  0x00017a60 2e2e6578 63657074 696f6e73 2e2e5079 ..exceptions..Py
+  0x00017a70 4e616d65 4572726f 72247532 30246173 NameError$u20$as
+  0x00017a80 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00017a90 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x00017aa0 37683832 66396236 34353363 33636434 7h82f9b6453c3cd4
+  0x00017ab0 62374500 5f5a4e36 385f244c 54247079 b7E._ZN68_$LT$py
+  0x00017ac0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x00017ad0 50794d65 6d6f7279 4572726f 72247532 PyMemoryError$u2
+  0x00017ae0 30246173 24753230 24636f72 652e2e66 0$as$u20$core..f
+  0x00017af0 6d742e2e 44656275 67244754 2433666d mt..Debug$GT$3fm
+  0x00017b00 74313768 35396334 36336233 37663463 t17h59c463b37f4c
+  0x00017b10 66343861 45005f5a 4e36335f 244c5424 f48aE._ZN63_$LT$
+  0x00017b20 72757374 635f6465 6d616e67 6c652e2e rustc_demangle..
+  0x00017b30 44656d61 6e676c65 24753230 24617324 Demangle$u20$as$
+  0x00017b40 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x00017b50 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
+  0x00017b60 68393739 39643335 31386336 32316365 h9799d3518c621ce
+  0x00017b70 3945005f 5a4e3463 6f726533 73747236 9E._ZN4core3str6
+  0x00017b80 74726169 74733233 7374725f 696e6465 traits23str_inde
+  0x00017b90 785f6f76 6572666c 6f775f66 61696c31 x_overflow_fail1
+  0x00017ba0 37683736 32333363 39393235 38643639 7h76233c99258d69
+  0x00017bb0 35374500 5f5a4e34 70796f33 33657272 57E._ZN4pyo33err
+  0x00017bc0 35507945 72723973 65745f63 61757365 5PyErr9set_cause
+  0x00017bd0 31376833 30353830 65663761 64646465 17h30580ef7addde
+  0x00017be0 66306445 005f5a4e 33737464 34706174 f0dE._ZN3std4pat
+  0x00017bf0 68313043 6f6d706f 6e656e74 73376173 h10Components7as
+  0x00017c00 5f706174 68313768 33636333 65363838 _path17h3cc3e688
+  0x00017c10 65333130 37373034 45005f5a 4e36335f e3107704E._ZN63_
+  0x00017c20 244c5424 636f7265 2e2e6365 6c6c2e2e $LT$core..cell..
+  0x00017c30 426f7272 6f774d75 74457272 6f722475 BorrowMutError$u
+  0x00017c40 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x00017c50 666d742e 2e446562 75672447 54243366 fmt..Debug$GT$3f
+  0x00017c60 6d743137 68383834 38626261 37623839 mt17h8848bba7b89
+  0x00017c70 64336638 6145005f 5a4e3463 6f726533 d3f8aE._ZN4core3
+  0x00017c80 666d7433 6e756d35 335f244c 5424696d fmt3num53_$LT$im
+  0x00017c90 706c2475 32302463 6f72652e 2e666d74 pl$u20$core..fmt
+  0x00017ca0 2e2e5570 70657248 65782475 32302466 ..UpperHex$u20$f
+  0x00017cb0 6f722475 32302469 33322447 54243366 or$u20$i32$GT$3f
+  0x00017cc0 6d743137 68666138 31643164 35613237 mt17hfa81d1d5a27
+  0x00017cd0 39346237 6445005f 5a4e3463 6f726533 94b7dE._ZN4core3
+  0x00017ce0 70747231 32356472 6f705f69 6e5f706c ptr125drop_in_pl
+  0x00017cf0 61636524 4c542470 796f332e 2e657272 ace$LT$pyo3..err
+  0x00017d00 2e2e6572 725f7374 6174652e 2e626f78 ..err_state..box
+  0x00017d10 65645f61 72677324 4c542470 796f332e ed_args$LT$pyo3.
+  0x00017d20 2e657272 2e2e5079 446f776e 63617374 .err..PyDowncast
+  0x00017d30 4572726f 72417267 756d656e 74732447 ErrorArguments$G
+  0x00017d40 54242e2e 24753762 24247537 6224636c T$..$u7b$$u7b$cl
+  0x00017d50 6f737572 65247537 64242475 37642424 osure$u7d$$u7d$$
+  0x00017d60 47542431 37683837 36643539 66653362 GT$17h876d59fe3b
+  0x00017d70 31333062 3037452e 6c6c766d 2e333136 130b07E.llvm.316
+  0x00017d80 30393037 32383138 38303738 31313233 0907281880781123
+  0x00017d90 005f5a4e 3130335f 244c5424 7374642e ._ZN103_$LT$std.
+  0x00017da0 2e73796e 632e2e6d 7073632e 2e547279 .sync..mpsc..Try
+  0x00017db0 52656376 4572726f 72247532 30246173 RecvError$u20$as
+  0x00017dc0 24753230 24636f72 652e2e63 6f6e7665 $u20$core..conve
+  0x00017dd0 72742e2e 46726f6d 244c5424 7374642e rt..From$LT$std.
+  0x00017de0 2e73796e 632e2e6d 7073632e 2e526563 .sync..mpsc..Rec
+  0x00017df0 76457272 6f722447 54242447 54243466 vError$GT$$GT$4f
+  0x00017e00 726f6d31 37686232 63663830 33663336 rom17hb2cf803f36
+  0x00017e10 31623632 65314500 616e6f6e 2e653965 1b62e1E.anon.e9e
+  0x00017e20 62323337 63663530 61343362 36356436 b237cf50a43b65d6
+  0x00017e30 33366230 66343737 30623034 652e3239 36b0f4770b04e.29
+  0x00017e40 2e6c6c76 6d2e3133 38363138 35323731 .llvm.1386185271
+  0x00017e50 31333930 32373437 3600616e 6f6e2e61 139027476.anon.a
+  0x00017e60 61343333 39636132 64626232 39366661 a4339ca2dbb296fa
+  0x00017e70 36336261 35376435 38643535 6538392e 63ba57d58d55e89.
+  0x00017e80 302e6c6c 766d2e31 35323830 30393430 0.llvm.152800940
+  0x00017e90 31383838 39343131 30363200 5f5a4e37 18889411062._ZN7
+  0x00017ea0 375f244c 54247079 6f332e2e 65786365 7_$LT$pyo3..exce
+  0x00017eb0 7074696f 6e732e2e 50794e6f 74414469 ptions..PyNotADi
+  0x00017ec0 72656374 6f727945 72726f72 24753230 rectoryError$u20
+  0x00017ed0 24617324 75323024 636f7265 2e2e666d $as$u20$core..fm
+  0x00017ee0 742e2e44 6973706c 61792447 54243366 t..Display$GT$3f
+  0x00017ef0 6d743137 68313239 38346231 30653065 mt17h12984b10e0e
+  0x00017f00 62666538 3445005f 5a4e3630 5f244c54 bfe84E._ZN60_$LT
+  0x00017f10 24737464 2e2e696f 2e2e6572 726f722e $std..io..error.
+  0x00017f20 2e457272 6f722475 32302461 73247532 .Error$u20$as$u2
+  0x00017f30 3024636f 72652e2e 666d742e 2e446973 0$core..fmt..Dis
+  0x00017f40 706c6179 24475424 33666d74 31376833 play$GT$3fmt17h3
+  0x00017f50 65333432 39326636 63643566 63343045 e34292f6cd5fc40E
+  0x00017f60 005f5f72 646c5f72 65616c6c 6f630061 .__rdl_realloc.a
+  0x00017f70 6e6f6e2e 36383266 30353362 61336436 non.682f053ba3d6
+  0x00017f80 64313461 66356232 37636663 62626431 d14af5b27cfcbbd1
+  0x00017f90 36333633 2e34312e 6c6c766d 2e353639 6363.41.llvm.569
+  0x00017fa0 37393239 37363931 33333035 37343736 7929769133057476
+  0x00017fb0 005f5a4e 34636f72 65337074 72313233 ._ZN4core3ptr123
+  0x00017fc0 64726f70 5f696e5f 706c6163 65244c54 drop_in_place$LT
+  0x00017fd0 2470796f 332e2e65 72722e2e 6572725f $pyo3..err..err_
+  0x00017fe0 73746174 652e2e62 6f786564 5f617267 state..boxed_arg
+  0x00017ff0 73244c54 24636f72 652e2e6e 65742e2e s$LT$core..net..
+  0x00018000 70617273 65722e2e 41646472 50617273 parser..AddrPars
+  0x00018010 65457272 6f722447 54242e2e 24753762 eError$GT$..$u7b
+  0x00018020 24247537 6224636c 6f737572 65247537 $$u7b$closure$u7
+  0x00018030 64242475 37642424 47542431 37686163 d$$u7d$$GT$17hac
+  0x00018040 38336635 34393162 63313764 3335452e 83f5491bc17d35E.
+  0x00018050 6c6c766d 2e333136 30393037 32383138 llvm.31609072818
+  0x00018060 38303738 31313233 005f5a4e 35395f24 80781123._ZN59_$
+  0x00018070 4c542463 6f72652e 2e666d74 2e2e4172 LT$core..fmt..Ar
+  0x00018080 67756d65 6e747324 75323024 61732475 guments$u20$as$u
+  0x00018090 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
+  0x000180a0 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
+  0x000180b0 34313735 62303536 65643066 61623236 4175b056ed0fab26
+  0x000180c0 45005f5a 4e337374 64337379 7334756e E._ZN3std3sys4un
+  0x000180d0 6978356c 6f636b73 31326675 7465785f ix5locks12futex_
+  0x000180e0 72776c6f 636b3652 774c6f63 6b323277 rwlock6RwLock22w
+  0x000180f0 616b655f 77726974 65725f6f 725f7265 ake_writer_or_re
+  0x00018100 61646572 73313768 35626134 62376638 aders17h5ba4b7f8
+  0x00018110 30306362 64303434 4500616e 6f6e2e33 00cbd044E.anon.3
+  0x00018120 34376432 36346533 34656233 61306337 47d264e34eb3a0c7
+  0x00018130 34626535 61383966 38393561 6337652e 4be5a89f895ac7e.
+  0x00018140 36312e6c 6c766d2e 31373639 35373632 61.llvm.17695762
+  0x00018150 33343137 38313435 33303132 00616e6f 341781453012.ano
+  0x00018160 6e2e3638 32663035 33626133 64366431 n.682f053ba3d6d1
+  0x00018170 34616635 62323763 66636262 64313633 4af5b27cfcbbd163
+  0x00018180 36332e31 312e6c6c 766d2e35 36393739 63.11.llvm.56979
+  0x00018190 32393736 39313333 30353734 3736005f 29769133057476._
+  0x000181a0 5a4e3463 6f726537 756e6963 6f646539 ZN4core7unicode9
+  0x000181b0 7072696e 7461626c 65313269 735f7072 printable12is_pr
+  0x000181c0 696e7461 626c6531 37683961 36363733 intable17h9a6673
+  0x000181d0 34326337 31323634 66394500 5f5a4e34 42c71264f9E._ZN4
+  0x000181e0 70796f33 35747970 6573366d 6f64756c pyo35types6modul
+  0x000181f0 65385079 4d6f6475 6c65346e 616d6531 e8PyModule4name1
+  0x00018200 37683731 32623463 38336638 34323835 7h712b4c83f84285
+  0x00018210 37304500 5f5a4e35 67696d6c 69347265 70E._ZN5gimli4re
+  0x00018220 61643661 62627265 76313241 62627265 ad6abbrev12Abbre
+  0x00018230 76696174 696f6e33 6e657731 37683138 viation3new17h18
+  0x00018240 61633835 30623435 64383366 64644500 ac850b45d83fddE.
+  0x00018250 5f5a4e37 305f244c 54247079 6f332e2e _ZN70_$LT$pyo3..
+  0x00018260 65786365 7074696f 6e732e2e 50794d65 exceptions..PyMe
+  0x00018270 6d6f7279 4572726f 72247532 30246173 moryError$u20$as
+  0x00018280 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00018290 44697370 6c617924 47542433 666d7431 Display$GT$3fmt1
+  0x000182a0 37686162 63613139 63636535 61666339 7habca19cce5afc9
+  0x000182b0 65664500 5f5a4e35 375f244c 5424636f efE._ZN57_$LT$co
+  0x000182c0 72652e2e 666d742e 2e466f72 6d617474 re..fmt..Formatt
+  0x000182d0 65722475 32302461 73247532 3024636f er$u20$as$u20$co
+  0x000182e0 72652e2e 666d742e 2e577269 74652447 re..fmt..Write$G
+  0x000182f0 54243977 72697465 5f666d74 31376836 T$9write_fmt17h6
+  0x00018300 35643134 63393335 63643731 65666245 5d14c935cd71efbE
+  0x00018310 005f5a4e 3470796f 33336769 6c313352 ._ZN4pyo33gil13R
+  0x00018320 65666572 656e6365 506f6f6c 31337570 eferencePool13up
+  0x00018330 64617465 5f636f75 6e747331 37683334 date_counts17h34
+  0x00018340 38376438 66353730 30323763 31354500 87d8f570027c15E.
+  0x00018350 5f5a4e37 365f244c 54247079 6f332e2e _ZN76_$LT$pyo3..
+  0x00018360 65786365 7074696f 6e732e2e 6173796e exceptions..asyn
+  0x00018370 63696f2e 2e54696d 656f7574 4572726f cio..TimeoutErro
+  0x00018380 72247532 30246173 24753230 24636f72 r$u20$as$u20$cor
+  0x00018390 652e2e66 6d742e2e 44656275 67244754 e..fmt..Debug$GT
+  0x000183a0 2433666d 74313768 35353632 64343731 $3fmt17h5562d471
+  0x000183b0 63663431 30373264 45005f5a 4e34636f cf41072dE._ZN4co
+  0x000183c0 72653370 74723738 64726f70 5f696e5f re3ptr78drop_in_
+  0x000183d0 706c6163 65244c54 2470796f 332e2e69 place$LT$pyo3..i
+  0x000183e0 6e737461 6e63652e 2e507924 4c542470 nstance..Py$LT$p
+  0x000183f0 796f332e 2e747970 65732e2e 74797065 yo3..types..type
+  0x00018400 6f626a65 63742e2e 50795479 70652447 object..PyType$G
+  0x00018410 54242447 54243137 68323231 35643361 T$$GT$17h2215d3a
+  0x00018420 39623062 65393639 63452e6c 6c766d2e 9b0be969cE.llvm.
+  0x00018430 31333836 31383532 37313133 39303237 1386185271139027
+  0x00018440 34373600 5f5a4e34 70796f33 35696d70 476._ZN4pyo35imp
+  0x00018450 6c5f3136 65787472 6163745f 61726775 l_16extract_argu
+  0x00018460 6d656e74 31394675 6e637469 6f6e4465 ment19FunctionDe
+  0x00018470 73637269 7074696f 6e323974 6f6f5f6d scription29too_m
+  0x00018480 616e795f 706f7369 74696f6e 616c5f61 any_positional_a
+  0x00018490 7267756d 656e7473 31376837 39353433 rguments17h79543
+  0x000184a0 66663934 39366661 64623645 005f5a4e ff9496fadb6E._ZN
+  0x000184b0 37325f24 4c542470 796f332e 2e657863 72_$LT$pyo3..exc
+  0x000184c0 65707469 6f6e732e 2e507953 746f7049 eptions..PyStopI
+  0x000184d0 74657261 74696f6e 24753230 24617324 teration$u20$as$
+  0x000184e0 75323024 636f7265 2e2e666d 742e2e44 u20$core..fmt..D
+  0x000184f0 6973706c 61792447 54243366 6d743137 isplay$GT$3fmt17
+  0x00018500 68363036 65666264 39343835 36646236 h606efbd94856db6
+  0x00018510 6645005f 5a4e3463 6f726533 6f707338 fE._ZN4core3ops8
+  0x00018520 66756e63 74696f6e 36466e4f 6e636534 function6FnOnce4
+  0x00018530 3063616c 6c5f6f6e 63652475 37622424 0call_once$u7b$$
+  0x00018540 75376224 76746162 6c652e73 68696d24 u7b$vtable.shim$
+  0x00018550 75376424 24753764 24313768 37336537 u7d$$u7d$17h73e7
+  0x00018560 61393736 35356264 37666130 452e6c6c a97655bd7fa0E.ll
+  0x00018570 766d2e33 31363039 30373238 31383830 vm.3160907281880
+  0x00018580 37383131 3233005f 5a4e3373 74643269 781123._ZN3std2i
+  0x00018590 6f357374 64696f37 5f657072 696e7431 o5stdio7_eprint1
+  0x000185a0 37683231 39326366 38653233 33636436 7h2192cf8e233cd6
+  0x000185b0 61614500 5f5a4e37 375f244c 54247079 aaE._ZN77_$LT$py
+  0x000185c0 6f332e2e 65786365 7074696f 6e732e2e o3..exceptions..
+  0x000185d0 5079556e 69636f64 65456e63 6f646545 PyUnicodeEncodeE
+  0x000185e0 72726f72 24753230 24617324 75323024 rror$u20$as$u20$
+  0x000185f0 636f7265 2e2e666d 742e2e44 6973706c core..fmt..Displ
+  0x00018600 61792447 54243366 6d743137 68666135 ay$GT$3fmt17hfa5
+  0x00018610 39353536 31323738 62633336 6645005f 95561278bc36fE._
+  0x00018620 5a4e3767 656f7267 696f3767 656f7267 ZN7georgio7georg
+  0x00018630 696f3137 68313765 65383462 65383464 io17h17ee84be84d
+  0x00018640 34613339 6245005f 5a4e3834 5f244c54 4a39bE._ZN84_$LT
+  0x00018650 24636f72 652e2e63 6861722e 2e457363 $core..char..Esc
+  0x00018660 61706544 65666175 6c742475 32302461 apeDefault$u20$a
+  0x00018670 73247532 3024636f 72652e2e 69746572 s$u20$core..iter
+  0x00018680 2e2e7472 61697473 2e2e6974 65726174 ..traits..iterat
+  0x00018690 6f722e2e 49746572 61746f72 24475424 or..Iterator$GT$
+  0x000186a0 346e6578 74313768 38356636 36653835 4next17h85f66e85
+  0x000186b0 34366335 62643538 45005f5a 4e34636f 46c5bd58E._ZN4co
+  0x000186c0 72653570 616e6963 31307061 6e69635f re5panic10panic_
+  0x000186d0 696e666f 3950616e 6963496e 666f3130 info9PanicInfo10
+  0x000186e0 63616e5f 756e7769 6e643137 68636262 can_unwind17hcbb
+  0x000186f0 38363336 36386236 37303365 6645005f 863668b6703efE._
+  0x00018700 5a4e3638 5f244c54 24636f72 652e2e66 ZN68_$LT$core..f
+  0x00018710 6d742e2e 6275696c 64657273 2e2e5061 mt..builders..Pa
+  0x00018720 64416461 70746572 24753230 24617324 dAdapter$u20$as$
+  0x00018730 75323024 636f7265 2e2e666d 742e2e57 u20$core..fmt..W
+  0x00018740 72697465 24475424 39777269 74655f73 rite$GT$9write_s
+  0x00018750 74723137 68623331 63303534 35346236 tr17hb31c05454b6
+  0x00018760 38306161 32450061 6e6f6e2e 61383039 80aa2E.anon.a809
+  0x00018770 30326436 62623038 37373362 66363734 02d6bb08773bf674
+  0x00018780 33643032 33633764 66373365 2e31372e 3d023c7df73e.17.
+  0x00018790 6c6c766d 2e313139 34303632 31333637 llvm.11940621367
+  0x000187a0 35363036 36323830 3500616e 6f6e2e33 560662805.anon.3
+  0x000187b0 34376432 36346533 34656233 61306337 47d264e34eb3a0c7
+  0x000187c0 34626535 61383966 38393561 6337652e 4be5a89f895ac7e.
+  0x000187d0 31352e6c 6c766d2e 31373639 35373632 15.llvm.17695762
+  0x000187e0 33343137 38313435 33303132 005f5a4e 341781453012._ZN
+  0x000187f0 34636f72 65336666 6935635f 73747234 4core3ffi5c_str4
+  0x00018800 43537472 31396672 6f6d5f62 79746573 CStr19from_bytes
+  0x00018810 5f776974 685f6e75 6c313768 36306261 _with_nul17h60ba
+  0x00018820 36623739 33363332 35366363 45005f5a 6b79363256ccE._Z
+  0x00018830 4e36385f 244c5424 70796f33 2e2e6578 N68_$LT$pyo3..ex
+  0x00018840 63657074 696f6e73 2e2e5079 42756666 ceptions..PyBuff
+  0x00018850 65724572 726f7224 75323024 61732475 erError$u20$as$u
+  0x00018860 32302463 6f72652e 2e666d74 2e2e4465 20$core..fmt..De
+  0x00018870 62756724 47542433 666d7431 37683165 bug$GT$3fmt17h1e
+  0x00018880 33666234 61333065 30396564 35344500 3fb4a30e09ed54E.
+  0x00018890 616e6f6e 2e623961 30343836 63303061 anon.b9a0486c00a
+  0x000188a0 34313732 62376231 61633532 62333135 4172b7b1ac52b315
+  0x000188b0 61613461 332e3235 2e6c6c76 6d2e3133 aa4a3.25.llvm.13
+  0x000188c0 32333838 39333433 32323030 36393232 2388934322006922
+  0x000188d0 32360061 6e6f6e2e 37623934 36616531 26.anon.7b946ae1
+  0x000188e0 64336136 36363739 37653264 62316633 d3a666797e2db1f3
+  0x000188f0 36653463 64366537 2e32382e 6c6c766d 6e4cd6e7.28.llvm
+  0x00018900 2e313833 35363735 30343835 36313435 .183567504856145
+  0x00018910 31333132 39005f5f 706f7769 73663200 13129.__powisf2.
+  0x00018920 5f5a4e34 70796f33 3367696c 35535441 _ZN4pyo33gil5STA
+  0x00018930 52543137 68353835 32336630 38346238 RT17h58523f084b8
+  0x00018940 66633931 38452e6c 6c766d2e 31333233 fc918E.llvm.1323
+  0x00018950 38383933 34333232 30303639 32323236 8893432200692226
+  0x00018960 00616e6f 6e2e3762 39343661 65316433 .anon.7b946ae1d3
+  0x00018970 61363636 37393765 32646231 66333665 a666797e2db1f36e
+  0x00018980 34636436 65372e32 392e6c6c 766d2e31 4cd6e7.29.llvm.1
+  0x00018990 38333536 37353034 38353631 34353133 8356750485614513
+  0x000189a0 31323900 5f5a4e34 70796f33 35696d70 129._ZN4pyo35imp
+  0x000189b0 6c5f3136 65787472 6163745f 61726775 l_16extract_argu
+  0x000189c0 6d656e74 31394675 6e637469 6f6e4465 ment19FunctionDe
+  0x000189d0 73637269 7074696f 6e323775 6e657870 scription27unexp
+  0x000189e0 65637465 645f6b65 79776f72 645f6172 ected_keyword_ar
+  0x000189f0 67756d65 6e743137 68633265 61303331 gument17hc2ea031
+  0x00018a00 36353439 62376362 3145005f 5a4e3336 6549b7cb1E._ZN36
+  0x00018a10 5f244c54 24542475 32302461 73247532 _$LT$T$u20$as$u2
+  0x00018a20 3024636f 72652e2e 616e792e 2e416e79 0$core..any..Any
+  0x00018a30 24475424 37747970 655f6964 31376833 $GT$7type_id17h3
+  0x00018a40 37643330 38316661 37653931 32383745 7d3081fa7e91287E
+  0x00018a50 005f5a4e 34636f72 6533666d 7439466f ._ZN4core3fmt9Fo
+  0x00018a60 726d6174 74657233 6e657731 37686439 rmatter3new17hd9
+  0x00018a70 34333636 64336165 36636263 64664500 4366d3ae6cbcdfE.
+  0x00018a80 5f5a4e34 636f7265 3570616e 69633130 _ZN4core5panic10
+  0x00018a90 70616e69 635f696e 666f3950 616e6963 panic_info9Panic
+  0x00018aa0 496e666f 37706179 6c6f6164 31376862 Info7payload17hb
+  0x00018ab0 33643231 33343438 37383934 64653845 3d2134487894de8E
+  0x00018ac0 005f5f72 7573745f 616c6c6f 635f6572 .__rust_alloc_er
+  0x00018ad0 726f725f 68616e64 6c657200 5f5a4e35 ror_handler._ZN5
+  0x00018ae0 616c6c6f 63377261 775f7665 63313952 alloc7raw_vec19R
+  0x00018af0 61775665 63244c54 24542443 24412447 awVec$LT$T$C$A$G
+  0x00018b00 54243136 72657365 7276655f 666f725f T$16reserve_for_
+  0x00018b10 70757368 31376831 36386139 30306161 push17h168a900aa
+  0x00018b20 33653063 38623845 005f5a4e 34636f72 3e0c8b8E._ZN4cor
+  0x00018b30 65337074 72353264 726f705f 696e5f70 e3ptr52drop_in_p
+  0x00018b40 6c616365 244c5424 7374642e 2e746872 lace$LT$std..thr
+  0x00018b50 6561642e 2e6c6f63 616c2e2e 41636365 ead..local..Acce
+  0x00018b60 73734572 726f7224 47542431 37683639 ssError$GT$17h69
+  0x00018b70 37626434 35346464 33626131 6662452e 7bd454dd3ba1fbE.
+  0x00018b80 6c6c766d 2e313833 35363735 30343835 llvm.18356750485
+  0x00018b90 36313435 31333132 39005f5a 4e347079 614513129._ZN4py
+  0x00018ba0 6f333574 79706573 36737472 696e6738 o35types6string8
+  0x00018bb0 50795374 72696e67 3135746f 5f737472 PyString15to_str
+  0x00018bc0 696e675f 6c6f7373 79313768 64393966 ing_lossy17hd99f
+  0x00018bd0 32306366 30633832 35623262 45005f5a 20cf0c825b2bE._Z
+  0x00018be0 4e34636f 72653370 74723131 3964726f N4core3ptr119dro
+  0x00018bf0 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
+  0x00018c00 6f332e2e 6572722e 2e657272 5f737461 o3..err..err_sta
+  0x00018c10 74652e2e 626f7865 645f6172 6773244c te..boxed_args$L
+  0x00018c20 5424616c 6c6f632e 2e737472 696e672e T$alloc..string.
+  0x00018c30 2e46726f 6d557466 31364572 726f7224 .FromUtf16Error$
+  0x00018c40 4754242e 2e247537 62242475 37622463 GT$..$u7b$$u7b$c
+  0x00018c50 6c6f7375 72652475 37642424 75376424 losure$u7d$$u7d$
+  0x00018c60 24475424 31376839 34383131 66653461 $GT$17h94811fe4a
+  0x00018c70 63653734 61663245 2e6c6c76 6d2e3331 ce74af2E.llvm.31
+  0x00018c80 36303930 37323831 38383037 38313132 6090728188078112
+  0x00018c90 33005f5a 4e337374 6432696f 35577269 3._ZN3std2io5Wri
+  0x00018ca0 74653977 72697465 5f666d74 31376862 te9write_fmt17hb
+  0x00018cb0 38393631 32636461 63663137 35656545 89612cdacf175eeE
+  0x00018cc0 005f5a4e 3470796f 3335696d 706c5f31 ._ZN4pyo35impl_1
+  0x00018cd0 36657874 72616374 5f617267 756d656e 6extract_argumen
+  0x00018ce0 74313946 756e6374 696f6e44 65736372 t19FunctionDescr
+  0x00018cf0 69707469 6f6e3333 706f7369 74696f6e iption33position
+  0x00018d00 616c5f6f 6e6c795f 6b657977 6f72645f al_only_keyword_
+  0x00018d10 61726775 6d656e74 73313768 36396439 arguments17h69d9
+  0x00018d20 39336430 62393262 64613964 45005f5a 93d0b92bda9dE._Z
+  0x00018d30 4e347079 6f333365 72723137 70616e69 N4pyo33err17pani
+  0x00018d40 635f6166 7465725f 6572726f 72313768 c_after_error17h
+  0x00018d50 65376164 66643361 63386431 64386163 e7adfd3ac8d1d8ac
+  0x00018d60 4500616e 6f6e2e37 62393436 61653164 E.anon.7b946ae1d
+  0x00018d70 33613636 36373937 65326462 31663336 3a666797e2db1f36
+  0x00018d80 65346364 3665372e 33312e6c 6c766d2e e4cd6e7.31.llvm.
+  0x00018d90 31383335 36373530 34383536 31343531 1835675048561451
+  0x00018da0 33313239 005f5a4e 35616c6c 6f633131 3129._ZN5alloc11
+  0x00018db0 636f6c6c 65637469 6f6e7335 62747265 collections5btre
+  0x00018dc0 65346e6f 64653130 73706c69 74706f69 e4node10splitpoi
+  0x00018dd0 6e743137 68333635 35353332 30646637 nt17h36555320df7
+  0x00018de0 39373264 6545005f 5a4e3463 6f726533 972deE._ZN4core3
+  0x00018df0 70747239 3164726f 705f696e 5f706c61 ptr91drop_in_pla
+  0x00018e00 6365244c 5424636f 72652e2e 63656c6c ce$LT$core..cell
+  0x00018e10 2e2e5265 664d7574 244c5424 616c6c6f ..RefMut$LT$allo
+  0x00018e20 632e2e76 65632e2e 56656324 4c542473 c..vec..Vec$LT$s
+  0x00018e30 74642e2e 74687265 61642e2e 54687265 td..thread..Thre
+  0x00018e40 61644964 24475424 24475424 24475424 adId$GT$$GT$$GT$
+  0x00018e50 31376836 36396138 35346431 31653231 17h669a854d11e21
+  0x00018e60 35636245 2e6c6c76 6d2e3138 33353637 5cbE.llvm.183567
+  0x00018e70 35303438 35363134 35313331 3239005f 50485614513129._
+  0x00018e80 5a4e3463 6f726533 70747233 3764726f ZN4core3ptr37dro
+  0x00018e90 705f696e 5f706c61 6365244c 54247079 p_in_place$LT$py
+  0x00018ea0 6f332e2e 6572722e 2e507945 72722447 o3..err..PyErr$G
+  0x00018eb0 54243137 68626437 34353762 30323035 T$17hbd7457b0205
+  0x00018ec0 37336431 62452e6c 6c766d2e 31333836 73d1bE.llvm.1386
+  0x00018ed0 31383532 37313133 39303237 34373600 185271139027476.
+  0x00018ee0 5f5a4e36 355f244c 54247079 6f332e2e _ZN65_$LT$pyo3..
+  0x00018ef0 65786365 7074696f 6e732e2e 50794b65 exceptions..PyKe
+  0x00018f00 79457272 6f722475 32302461 73247532 yError$u20$as$u2
+  0x00018f10 3024636f 72652e2e 666d742e 2e446562 0$core..fmt..Deb
+  0x00018f20 75672447 54243366 6d743137 68313465 ug$GT$3fmt17h14e
+  0x00018f30 33613061 37303539 61333436 66450061 3a0a7059a346fE.a
+  0x00018f40 6e6f6e2e 62396130 34383663 30306134 non.b9a0486c00a4
+  0x00018f50 31373262 37623161 63353262 33313561 172b7b1ac52b315a
+  0x00018f60 61346133 2e33362e 6c6c766d 2e313332 a4a3.36.llvm.132
+  0x00018f70 33383839 33343332 32303036 39323232 3889343220069222
+  0x00018f80 3600616e 6f6e2e33 34376432 36346533 6.anon.347d264e3
+  0x00018f90 34656233 61306337 34626535 61383966 4eb3a0c74be5a89f
+  0x00018fa0 38393561 6337652e 31342e6c 6c766d2e 895ac7e.14.llvm.
+  0x00018fb0 31373639 35373632 33343137 38313435 1769576234178145
+  0x00018fc0 33303132 005f5a4e 34636f72 65337374 3012._ZN4core3st
+  0x00018fd0 72313673 6c696365 5f657272 6f725f66 r16slice_error_f
+  0x00018fe0 61696c31 37683333 63633231 64376538 ail17h33cc21d7e8
+  0x00018ff0 65643134 65634500 616e6f6e 2e333437 ed14ecE.anon.347
+  0x00019000 64323634 65333465 62336130 63373462 d264e34eb3a0c74b
+  0x00019010 65356138 39663839 35616337 652e3630 e5a89f895ac7e.60
+  0x00019020 2e6c6c76 6d2e3137 36393537 36323334 .llvm.1769576234
+  0x00019030 31373831 34353330 3132005f 5a4e3537 1781453012._ZN57
+  0x00019040 5f244c54 24636f72 652e2e66 6d742e2e _$LT$core..fmt..
+  0x00019050 466f726d 61747465 72247532 30246173 Formatter$u20$as
+  0x00019060 24753230 24636f72 652e2e66 6d742e2e $u20$core..fmt..
+  0x00019070 57726974 65244754 24313077 72697465 Write$GT$10write
+  0x00019080 5f636861 72313768 64306463 35333434 _char17hd0dc5344
+  0x00019090 39393734 31356239 45005f5a 4e337374 997415b9E._ZN3st
+  0x000190a0 6432696f 35577269 74653977 72697465 d2io5Write9write
+  0x000190b0 5f616c6c 31376830 64623864 37373262 _all17h0db8d772b
+  0x000190c0 33303266 30306245 005f5a4e 33737464 302f00bE._ZN3std
+  0x000190d0 33737973 34756e69 78346172 67733369 3sys4unix4args3i
+  0x000190e0 6d703135 41524756 5f494e49 545f4152 mp15ARGV_INIT_AR
+  0x000190f0 52415931 37683330 34313261 32326663 RAY17h30412a22fc
+  0x00019100 31373634 39304500 5f5a4e33 73746433 176490E._ZN3std3
+  0x00019110 73797334 756e6978 34617267 7333696d sys4unix4args3im
+  0x00019120 70313541 5247565f 494e4954 5f415252 p15ARGV_INIT_ARR
+  0x00019130 41593132 696e6974 5f777261 70706572 AY12init_wrapper
+  0x00019140 31376835 65643731 39323566 36343730 17h5ed71925f6470
+  0x00019150 32303245 005f5a4e 39315f24 4c542461 202E._ZN91_$LT$a
+  0x00019160 64647232 6c696e65 2e2e4c6f 63617469 ddr2line..Locati
+  0x00019170 6f6e5261 6e676555 6e697449 74657224 onRangeUnitIter$
+  0x00019180 75323024 61732475 32302463 6f72652e u20$as$u20$core.
+  0x00019190 2e697465 722e2e74 72616974 732e2e69 .iter..traits..i
+  0x000191a0 74657261 746f722e 2e497465 7261746f terator..Iterato
+  0x000191b0 72244754 24346e65 78743137 68333236 r$GT$4next17h326
+  0x000191c0 39616334 31373464 32383538 6245005f 9ac4174d2858bE._
+  0x000191d0 5a4e3463 6f726533 70747231 32326472 ZN4core3ptr122dr
+  0x000191e0 6f705f69 6e5f706c 61636524 4c542470 op_in_place$LT$p
+  0x000191f0 796f332e 2e657272 2e2e6572 725f7374 yo3..err..err_st
+  0x00019200 6174652e 2e626f78 65645f61 72677324 ate..boxed_args$
+  0x00019210 4c542463 6f72652e 2e737472 2e2e6572 LT$core..str..er
+  0x00019220 726f722e 2e506172 7365426f 6f6c4572 ror..ParseBoolEr
+  0x00019230 726f7224 4754242e 2e247537 62242475 ror$GT$..$u7b$$u
+  0x00019240 37622463 6c6f7375 72652475 37642424 7b$closure$u7d$$
+  0x00019250 75376424 24475424 31376830 33613734 u7d$$GT$17h03a74
+  0x00019260 30346666 38633831 65623045 2e6c6c76 04ff8c81eb0E.llv
+  0x00019270 6d2e3331 36303930 37323831 38383037 m.31609072818807
+  0x00019280 38313132 33005f5a 4e35616c 6c6f6335 81123._ZN5alloc5
+  0x00019290 616c6c6f 6338626f 785f6672 65653137 alloc8box_free17
+  0x000192a0 68373630 36316163 61383066 62333939 h76061aca80fb399
+  0x000192b0 30452e6c 6c766d2e 31313233 36353732 0E.llvm.11236572
+  0x000192c0 38353335 30393639 32343136 005f5a4e 853509692416._ZN
+  0x000192d0 3561646c 65723741 646c6572 33323131 5adler7Adler3211
+  0x000192e0 77726974 655f736c 69636531 37686532 write_slice17he2
+  0x000192f0 34303466 36663237 64326566 30394500 404f6f27d2ef09E.
+  0x00019300 5f5a4e34 70796f33 35747970 65733361 _ZN4pyo35types3a
+  0x00019310 6e793550 79416e79 37736574 61747472 ny5PyAny7setattr
+  0x00019320 31376834 61656566 38316430 32663862 17h4aeef81d02f8b
+  0x00019330 37666145 005f5a4e 37395f24 4c542473 7faE._ZN79_$LT$s
+  0x00019340 74642e2e 6261636b 74726163 655f7273 td..backtrace_rs
+  0x00019350 2e2e7379 6d626f6c 697a652e 2e53796d ..symbolize..Sym
+  0x00019360 626f6c4e 616d6524 75323024 61732475 bolName$u20$as$u
+  0x00019370 32302463 6f72652e 2e666d74 2e2e4469 20$core..fmt..Di
+  0x00019380 73706c61 79244754 2433666d 74313768 splay$GT$3fmt17h
+  0x00019390 34333461 63623737 32326333 64656362 434acb7722c3decb
+  0x000193a0 45005f5a 4e36385f 244c5424 24524624 E._ZN68_$LT$$RF$
+  0x000193b0 24753562 24753824 75356424 24753230 $u5b$u8$u5d$$u20
+  0x000193c0 24617324 75323024 6f626a65 63742e2e $as$u20$object..
+  0x000193d0 72656164 2e2e7265 61645f72 65662e2e read..read_ref..
+  0x000193e0 52656164 52656624 47542431 39726561 ReadRef$GT$19rea
+  0x000193f0 645f6279 7465735f 61745f75 6e74696c d_bytes_at_until
+  0x00019400 31376831 37306234 30363064 62636165 17h170b4060dbcae
+  0x00019410 37376145 005f5a4e 34636f72 65337374 77aE._ZN4core3st
+  0x00019420 72356c6f 73737939 55746638 4368756e r5lossy9Utf8Chun
+  0x00019430 6b357661 6c696431 37683135 64316539 k5valid17h15d1e9
+  0x00019440 38636331 34353031 38624500 5f5a4e38 8cc145018bE._ZN8
+  0x00019450 315f244c 54247079 6f332e2e 65786365 1_$LT$pyo3..exce
+  0x00019460 7074696f 6e732e2e 5079436f 6e6e6563 ptions..PyConnec
+  0x00019470 74696f6e 52656675 73656445 72726f72 tionRefusedError
+  0x00019480 24753230 24617324 75323024 636f7265 $u20$as$u20$core
+  0x00019490 2e2e666d 742e2e44 6973706c 61792447 ..fmt..Display$G
+  0x000194a0 54243366 6d743137 68616134 66383065 T$3fmt17haa4f80e
+  0x000194b0 36393764 30363966 3445005f 5a4e3463 697d069f4E._ZN4c
+  0x000194c0 6f726535 736c6963 6535696e 64657832 ore5slice5index2
+  0x000194d0 36736c69 63655f73 74617274 5f696e64 6slice_start_ind
+  0x000194e0 65785f6c 656e5f66 61696c31 37683662 ex_len_fail17h6b
+  0x000194f0 65653430 35626163 36643364 32364500 ee405bac6d3d26E.
+  0x00019500 616e6f6e 2e376239 34366165 31643361 anon.7b946ae1d3a
+  0x00019510 36363637 39376532 64623166 33366534 666797e2db1f36e4
+  0x00019520 63643665 372e3334 2e6c6c76 6d2e3138 cd6e7.34.llvm.18
+  0x00019530 33353637 35303438 35363134 35313331 3567504856145131
+  0x00019540 3239005f 5a4e3463 6f726533 70747234 29._ZN4core3ptr4
+  0x00019550 3264726f 705f696e 5f706c61 6365244c 2drop_in_place$L
+  0x00019560 54247374 642e2e69 6f2e2e65 72726f72 T$std..io..error
+  0x00019570 2e2e4572 726f7224 47542431 37686334 ..Error$GT$17hc4
+  0x00019580 38646466 32643230 37376665 6264452e 8ddf2d2077febdE.
+  0x00019590 6c6c766d 2e383336 34373335 31373237 llvm.83647351727
+  0x000195a0 30333437 36333534 005f5a4e 34636f72 03476354._ZN4cor
+  0x000195b0 65397061 6e69636b 696e6735 70616e69 e9panicking5pani
+  0x000195c0 63313768 39353333 62326665 65393062 c17h9533b2fee90b
+  0x000195d0 39393965 45005f5a 4e34636f 72653366 999eE._ZN4core3f
+  0x000195e0 6d743557 72697465 39777269 74655f66 mt5Write9write_f
+  0x000195f0 6d743137 68393461 63323432 61353465 mt17h94ac242a54e
+  0x00019600 34373363 3745005f 44594e41 4d494300 473c7E._DYNAMIC.
+  0x00019610 5f696e69 74005f5a 4e37365f 244c5424 _init._ZN76_$LT$
+  0x00019620 70796f33 2e2e6578 63657074 696f6e73 pyo3..exceptions
+  0x00019630 2e2e5079 49734144 69726563 746f7279 ..PyIsADirectory
+  0x00019640 4572726f 72247532 30246173 24753230 Error$u20$as$u20
+  0x00019650 24636f72 652e2e66 6d742e2e 44697370 $core..fmt..Disp
+  0x00019660 6c617924 47542433 666d7431 37686433 lay$GT$3fmt17hd3
+  0x00019670 34343935 37303632 65366130 36654500 44957062e6a06eE.
+  0x00019680 5f5a4e37 355f244c 54247079 6f332e2e _ZN75_$LT$pyo3..
+  0x00019690 65786365 7074696f 6e732e2e 5079496e exceptions..PyIn
+  0x000196a0 74657272 75707465 64457272 6f722475 terruptedError$u
+  0x000196b0 32302461 73247532 3024636f 72652e2e 20$as$u20$core..
+  0x000196c0 666d742e 2e446973 706c6179 24475424 fmt..Display$GT$
+  0x000196d0 33666d74 31376866 37613264 34616465 3fmt17hf7a2d4ade
+  0x000196e0 30393938 36356445 005f5a4e 34636f72 099865dE._ZN4cor
+  0x000196f0 6533666d 74313770 6f696e74 65725f66 e3fmt17pointer_f
+  0x00019700 6d745f69 6e6e6572 31376839 37623133 mt_inner17h97b13
+  0x00019710 61363132 61383061 34353645 00616e6f a612a80a456E.ano
+  0x00019720 6e2e3334 37643236 34653334 65623361 n.347d264e34eb3a
+  0x00019730 30633734 62653561 38396638 39356163 0c74be5a89f895ac
+  0x00019740 37652e36 342e6c6c 766d2e31 37363935 7e.64.llvm.17695
+  0x00019750 37363233 34313738 31343533 30313200 762341781453012.
+  0x00019760 5f5a4e39 335f244c 5424616c 6c6f632e _ZN93_$LT$alloc.
+  0x00019770 2e636f6c 6c656374 696f6e73 2e2e6274 .collections..bt
+  0x00019780 7265652e 2e6d656d 2e2e7265 706c6163 ree..mem..replac
+  0x00019790 652e2e50 616e6963 47756172 64247532 e..PanicGuard$u2
+  0x000197a0 30246173 24753230 24636f72 652e2e6f 0$as$u20$core..o
+  0x000197b0 70732e2e 64726f70 2e2e4472 6f702447 ps..drop..Drop$G
+  0x000197c0 54243464 726f7031 37683431 38336631 T$4drop17h4183f1
+  0x000197d0 33326662 36343862 30614500 5f5a4e34 32fb648b0aE._ZN4
+  0x000197e0 325f244c 54242452 46245424 75323024 2_$LT$$RF$T$u20$
+  0x000197f0 61732475 32302463 6f72652e 2e666d74 as$u20$core..fmt
+  0x00019800 2e2e4465 62756724 47542433 666d7431 ..Debug$GT$3fmt1
+  0x00019810 37683463 35383062 63376436 38306237 7h4c580bc7d680b7
+  0x00019820 30384500 616e6f6e 2e623961 30343836 08E.anon.b9a0486
+  0x00019830 63303061 34313732 62376231 61633532 c00a4172b7b1ac52
+  0x00019840 62333135 61613461 332e3335 2e6c6c76 b315aa4a3.35.llv
+  0x00019850 6d2e3133 32333838 39333433 32323030 m.13238893432200
+  0x00019860 36393232 32360061 6e6f6e2e 33343764 692226.anon.347d
+  0x00019870 32363465 33346562 33613063 37346265 264e34eb3a0c74be
+  0x00019880 35613839 66383935 61633765 2e382e6c 5a89f895ac7e.8.l
+  0x00019890 6c766d2e 31373639 35373632 33343137 lvm.176957623417
+  0x000198a0 38313435 33303132 005f5a4e 3470796f 81453012._ZN4pyo
+  0x000198b0 3335696d 706c5f31 36657874 72616374 35impl_16extract
+  0x000198c0 5f617267 756d656e 74313946 756e6374 _argument19Funct
+  0x000198d0 696f6e44 65736372 69707469 6f6e3236 ionDescription26
+  0x000198e0 65787472 6163745f 61726775 6d656e74 extract_argument
+  0x000198f0 735f6661 73746361 6c6c3137 68663537 s_fastcall17hf57
+  0x00019900 63353263 38663634 30353766 3845005f c52c8f64057f8E._
+  0x00019910 5a4e3463 6f726533 6e756d32 315f244c ZN4core3num21_$L
+  0x00019920 5424696d 706c2475 32302475 33322447 T$impl$u20$u32$G
+  0x00019930 54243134 66726f6d 5f737472 5f726164 T$14from_str_rad
+  0x00019940 69783137 68326439 37336166 30336336 ix17h2d973af03c6
+  0x00019950 36633632 62450050 79457863 5f426173 6c62bE.PyExc_Bas
+  0x00019960 65457863 65707469 6f6e0050 79457863 eException.PyExc
+  0x00019970 5f496d70 6f727445 72726f72 00707468 _ImportError.pth
+  0x00019980 72656164 5f676574 73706563 69666963 read_getspecific
+  0x00019990 4040474c 4942435f 322e322e 35007369 @@GLIBC_2.2.5.si
+  0x000199a0 6e636f73 66404047 4c494243 5f322e32 ncosf@@GLIBC_2.2
+  0x000199b0 2e350050 79556e69 636f6465 5f417345 .5.PyUnicode_AsE
+  0x000199c0 6e636f64 65645374 72696e67 005f556e ncodedString._Un
+  0x000199d0 77696e64 5f476574 52656769 6f6e5374 wind_GetRegionSt
+  0x000199e0 61727440 40474343 5f332e30 006d656d art@@GCC_3.0.mem
+  0x000199f0 73657440 40474c49 42435f32 2e322e35 set@@GLIBC_2.2.5
+  0x00019a00 00507945 78636570 74696f6e 5f536574 .PyException_Set
+  0x00019a10 43617573 65005f55 6e77696e 645f5365 Cause._Unwind_Se
+  0x00019a20 74475240 40474343 5f332e30 00706f73 tGR@@GCC_3.0.pos
+  0x00019a30 69785f6d 656d616c 69676e40 40474c49 ix_memalign@@GLI
+  0x00019a40 42435f32 2e322e35 00636c6f 73654040 BC_2.2.5.close@@
+  0x00019a50 474c4942 435f322e 322e3500 5f556e77 GLIBC_2.2.5._Unw
+  0x00019a60 696e645f 47657444 61746152 656c4261 ind_GetDataRelBa
+  0x00019a70 73654040 4743435f 332e3000 50794578 se@@GCC_3.0.PyEx
+  0x00019a80 635f5661 6c756545 72726f72 0061626f c_ValueError.abo
+  0x00019a90 72744040 474c4942 435f322e 322e3500 rt@@GLIBC_2.2.5.
+  0x00019aa0 70746872 6561645f 73657473 70656369 pthread_setspeci
+  0x00019ab0 66696340 40474c49 42435f32 2e322e35 fic@@GLIBC_2.2.5
+  0x00019ac0 00507945 78635f53 79737465 6d457272 .PyExc_SystemErr
+  0x00019ad0 6f72005f 5f676d6f 6e5f7374 6172745f or.__gmon_start_
+  0x00019ae0 5f005079 47494c53 74617465 5f52656c _.PyGILState_Rel
+  0x00019af0 65617365 00507942 79746573 5f53697a ease.PyBytes_Siz
+  0x00019b00 65005079 45786365 7074696f 6e5f4765 e.PyException_Ge
+  0x00019b10 74436175 7365006d 616c6c6f 63404047 tCause.malloc@@G
+  0x00019b20 4c494243 5f322e32 2e350050 79457863 LIBC_2.2.5.PyExc
+  0x00019b30 5f547970 65457272 6f720050 79457272 _TypeError.PyErr
+  0x00019b40 5f476976 656e4578 63657074 696f6e4d _GivenExceptionM
+  0x00019b50 61746368 65730073 63686564 5f796965 atches.sched_yie
+  0x00019b60 6c644040 474c4942 435f322e 322e3500 ld@@GLIBC_2.2.5.
+  0x00019b70 5f556e77 696e645f 44656c65 74654578 _Unwind_DeleteEx
+  0x00019b80 63657074 696f6e40 40474343 5f332e30 ception@@GCC_3.0
+  0x00019b90 0050794f 626a6563 745f5374 72005079 .PyObject_Str.Py
+  0x00019ba0 556e6963 6f64655f 41735554 4638416e Unicode_AsUTF8An
+  0x00019bb0 6453697a 65005079 496e6974 5f67656f dSize.PyInit_geo
+  0x00019bc0 7267696f 0050794c 6f6e675f 41734c6f rgio.PyLong_AsLo
+  0x00019bd0 6e67005f 5f637861 5f746872 6561645f ng.__cxa_thread_
+  0x00019be0 61746578 69745f69 6d706c00 5f5f6678 atexit_impl.__fx
+  0x00019bf0 73746174 36344040 474c4942 435f322e stat64@@GLIBC_2.
+  0x00019c00 322e3500 5f49544d 5f646572 65676973 2.5._ITM_deregis
+  0x00019c10 74657254 4d436c6f 6e655461 626c6500 terTMCloneTable.
+  0x00019c20 5079466c 6f61745f 46726f6d 446f7562 PyFloat_FromDoub
+  0x00019c30 6c650061 74616e32 66404047 4c494243 le.atan2f@@GLIBC
+  0x00019c40 5f322e32 2e35005f 556e7769 6e645f47 _2.2.5._Unwind_G
+  0x00019c50 65744c61 6e677561 67655370 65636966 etLanguageSpecif
+  0x00019c60 69634461 74614040 4743435f 332e3000 icData@@GCC_3.0.
+  0x00019c70 50794f62 6a656374 5f476574 41747472 PyObject_GetAttr
+  0x00019c80 00667265 65404047 4c494243 5f322e32 .free@@GLIBC_2.2
+  0x00019c90 2e350073 74726c65 6e404047 4c494243 .5.strlen@@GLIBC
+  0x00019ca0 5f322e32 2e35005f 49544d5f 72656769 _2.2.5._ITM_regi
+  0x00019cb0 73746572 544d436c 6f6e6554 61626c65 sterTMCloneTable
+  0x00019cc0 005f556e 77696e64 5f526169 73654578 ._Unwind_RaiseEx
+  0x00019cd0 63657074 696f6e40 40474343 5f332e30 ception@@GCC_3.0
+  0x00019ce0 005f5f63 78615f66 696e616c 697a6540 .__cxa_finalize@
+  0x00019cf0 40474c49 42435f32 2e322e35 00726561 @GLIBC_2.2.5.rea
+  0x00019d00 6c706174 68404047 4c494243 5f322e33 lpath@@GLIBC_2.3
+  0x00019d10 00707468 72656164 5f6b6579 5f64656c .pthread_key_del
+  0x00019d20 65746540 40474c49 42435f32 2e322e35 ete@@GLIBC_2.2.5
+  0x00019d30 00507942 79746573 5f417353 7472696e .PyBytes_AsStrin
+  0x00019d40 67005f5f 746c735f 6765745f 61646472 g.__tls_get_addr
+  0x00019d50 4040474c 4942435f 322e3300 73797363 @@GLIBC_2.3.sysc
+  0x00019d60 616c6c40 40474c49 42435f32 2e322e35 all@@GLIBC_2.2.5
+  0x00019d70 005f556e 77696e64 5f476574 49504040 ._Unwind_GetIP@@
+  0x00019d80 4743435f 332e3000 5f556e77 696e645f GCC_3.0._Unwind_
+  0x00019d90 4261636b 74726163 65404047 43435f33 Backtrace@@GCC_3
+  0x00019da0 2e33006f 70656e36 34404047 4c494243 .3.open64@@GLIBC
+  0x00019db0 5f322e32 2e350050 79457272 5f526573 _2.2.5.PyErr_Res
+  0x00019dc0 746f7265 0062636d 70404047 4c494243 tore.bcmp@@GLIBC
+  0x00019dd0 5f322e32 2e350072 6561646c 696e6b40 _2.2.5.readlink@
+  0x00019de0 40474c49 42435f32 2e322e35 00507945 @GLIBC_2.2.5.PyE
+  0x00019df0 72725f4e 65774578 63657074 696f6e57 rr_NewExceptionW
+  0x00019e00 69746844 6f630050 7947494c 53746174 ithDoc.PyGILStat
+  0x00019e10 655f456e 73757265 00507945 72725f4e e_Ensure.PyErr_N
+  0x00019e20 6f726d61 6c697a65 45786365 7074696f ormalizeExceptio
+  0x00019e30 6e006d65 6d6d6f76 65404047 4c494243 n.memmove@@GLIBC
+  0x00019e40 5f322e32 2e350050 79457272 5f466574 _2.2.5.PyErr_Fet
+  0x00019e50 63680050 794d6f64 756c655f 4765744e ch.PyModule_GetN
+  0x00019e60 616d6500 6174616e 66404047 4c494243 ame.atanf@@GLIBC
+  0x00019e70 5f322e32 2e350050 79466c6f 61745f41 _2.2.5.PyFloat_A
+  0x00019e80 73446f75 626c6500 67657465 6e764040 sDouble.getenv@@
+  0x00019e90 474c4942 435f322e 322e3500 5f556e77 GLIBC_2.2.5._Unw
+  0x00019ea0 696e645f 47657449 50496e66 6f404047 ind_GetIPInfo@@G
+  0x00019eb0 43435f34 2e322e30 00646c5f 69746572 CC_4.2.0.dl_iter
+  0x00019ec0 6174655f 70686472 4040474c 4942435f ate_phdr@@GLIBC_
+  0x00019ed0 322e322e 35005f5f 6572726e 6f5f6c6f 2.2.5.__errno_lo
+  0x00019ee0 63617469 6f6e4040 474c4942 435f322e cation@@GLIBC_2.
+  0x00019ef0 322e3500 50794578 635f4f76 6572666c 2.5.PyExc_Overfl
+  0x00019f00 6f774572 726f7200 50794c69 73745f41 owError.PyList_A
+  0x00019f10 7070656e 64005079 4f626a65 63745f53 ppend.PyObject_S
+  0x00019f20 65744174 74720067 65746377 64404047 etAttr.getcwd@@G
+  0x00019f30 4c494243 5f322e32 2e350050 79457272 LIBC_2.2.5.PyErr
+  0x00019f40 5f507269 6e740050 79457863 5f417474 _Print.PyExc_Att
+  0x00019f50 72696275 74654572 726f7200 73746174 ributeError.stat
+  0x00019f60 78006361 6c6c6f63 4040474c 4942435f x.calloc@@GLIBC_
+  0x00019f70 322e322e 35006d75 6e6d6170 4040474c 2.2.5.munmap@@GL
+  0x00019f80 4942435f 322e322e 35005f5f 7870675f IBC_2.2.5.__xpg_
+  0x00019f90 73747265 72726f72 5f724040 474c4942 strerror_r@@GLIB
+  0x00019fa0 435f322e 332e3400 5f50795f 4465616c C_2.3.4._Py_Deal
+  0x00019fb0 6c6f6300 77726974 65764040 474c4942 loc.writev@@GLIB
+  0x00019fc0 435f322e 322e3500 50794d6f 64756c65 C_2.2.5.PyModule
+  0x00019fd0 5f437265 61746532 00507954 75706c65 _Create2.PyTuple
+  0x00019fe0 5f4e6577 005f5f78 73746174 36344040 _New.__xstat64@@
+  0x00019ff0 474c4942 435f322e 322e3500 5079434d GLIBC_2.2.5.PyCM
+  0x0001a000 6574686f 645f4e65 77005f55 6e77696e ethod_New._Unwin
+  0x0001a010 645f4765 74546578 7452656c 42617365 d_GetTextRelBase
+  0x0001a020 40404743 435f332e 30005079 5475706c @@GCC_3.0.PyTupl
+  0x0001a030 655f5365 74497465 6d006173 696e6640 e_SetItem.asinf@
+  0x0001a040 40474c49 42435f32 2e322e35 00507955 @GLIBC_2.2.5.PyU
+  0x0001a050 6e69636f 64655f46 726f6d53 7472696e nicode_FromStrin
+  0x0001a060 67416e64 53697a65 00726561 6c6c6f63 gAndSize.realloc
+  0x0001a070 4040474c 4942435f 322e322e 35007074 @@GLIBC_2.2.5.pt
+  0x0001a080 68726561 645f6b65 795f6372 65617465 hread_key_create
+  0x0001a090 4040474c 4942435f 322e322e 35007772 @@GLIBC_2.2.5.wr
+  0x0001a0a0 69746540 40474c49 42435f32 2e322e35 ite@@GLIBC_2.2.5
+  0x0001a0b0 0073696e 68664040 474c4942 435f322e .sinhf@@GLIBC_2.
+  0x0001a0c0 322e3500 5f556e77 696e645f 52657375 2.5._Unwind_Resu
+  0x0001a0d0 6d654040 4743435f 332e3000 636c6f63 me@@GCC_3.0.cloc
+  0x0001a0e0 6b5f6765 7474696d 65404047 4c494243 k_gettime@@GLIBC
+  0x0001a0f0 5f322e32 2e350050 794c6973 745f4e65 _2.2.5.PyList_Ne
+  0x0001a100 77005079 4572725f 5072696e 74457800 w.PyErr_PrintEx.
+  0x0001a110 6d656d63 70794040 474c4942 435f322e memcpy@@GLIBC_2.
+  0x0001a120 31340050 79556e69 636f6465 5f496e74 14.PyUnicode_Int
+  0x0001a130 65726e49 6e506c61 63650050 795f4973 ernInPlace.Py_Is
+  0x0001a140 496e6974 69616c69 7a656400 50794e75 Initialized.PyNu
+  0x0001a150 6d626572 5f496e64 6578006d 6d617040 mber_Index.mmap@
+  0x0001a160 40474c49 42435f32 2e322e35 005f556e @GLIBC_2.2.5._Un
+  0x0001a170 77696e64 5f536574 49504040 4743435f wind_SetIP@@GCC_
+  0x0001a180 332e3000 50794f62 6a656374 5f526570 3.0.PyObject_Rep
+  0x0001a190 7200                                r.
```

## Comparing `georgio-2023.118.1193.dist-info/METADATA` & `georgio-2023.118.1197.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: georgio
-Version: 2023.118.1193
+Version: 2023.118.1197
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 License-File: NOTICE
 Summary: Fast Geo Rust functions for Python
 Author-email: Spectric Labs <foss@spectric.com>
```

## Comparing `georgio-2023.118.1193.dist-info/license_files/LICENSE` & `georgio-2023.118.1197.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

