# Comparing `tmp/stempy-3.3.3-cp39-cp39-win_amd64.whl.zip` & `tmp/stempy-3.3.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 2006089 bytes, number of entries: 16
--rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-06 15:12 stempy/__init__.py
--rw-rw-rw-  2.0 fat   265216 b- defN 23-Apr-06 15:22 stempy/_image.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   219648 b- defN 23-Apr-06 15:22 stempy/_io.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat  4203520 b- defN 23-Apr-06 15:22 stempy/stem.dll
--rw-rw-rw-  2.0 fat 17225502 b- defN 23-Apr-06 15:22 stempy/stem.lib
--rw-rw-rw-  2.0 fat      556 b- defN 23-Apr-06 15:12 stempy/utils.py
--rw-rw-rw-  2.0 fat    32699 b- defN 23-Apr-06 15:12 stempy/image/__init__.py
--rw-rw-rw-  2.0 fat    10673 b- defN 23-Apr-06 15:12 stempy/io/__init__.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-06 15:12 stempy/io/compatibility.py
--rw-rw-rw-  2.0 fat    40118 b- defN 23-Apr-06 15:12 stempy/io/sparse_array.py
--rw-rw-rw-  2.0 fat     1496 b- defN 23-Apr-06 15:12 stempy/pipeline/__init__.py
--rw-rw-rw-  2.0 fat     1531 b- defN 23-Apr-06 15:22 stempy-3.3.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-06 15:22 stempy-3.3.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-06 15:22 stempy-3.3.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-06 15:22 stempy-3.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1265 b- defN 23-Apr-06 15:22 stempy-3.3.3.dist-info/RECORD
-16 files, 22006634 bytes uncompressed, 2004049 bytes compressed:  90.9%
+Zip file size: 2006125 bytes, number of entries: 16
+-rw-rw-rw-  2.0 fat      101 b- defN 23-Apr-28 18:49 stempy/__init__.py
+-rw-rw-rw-  2.0 fat   265216 b- defN 23-Apr-28 18:59 stempy/_image.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   219648 b- defN 23-Apr-28 18:59 stempy/_io.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  4203520 b- defN 23-Apr-28 18:59 stempy/stem.dll
+-rw-rw-rw-  2.0 fat 17225502 b- defN 23-Apr-28 18:59 stempy/stem.lib
+-rw-rw-rw-  2.0 fat      556 b- defN 23-Apr-28 18:49 stempy/utils.py
+-rw-rw-rw-  2.0 fat    32699 b- defN 23-Apr-28 18:49 stempy/image/__init__.py
+-rw-rw-rw-  2.0 fat    10673 b- defN 23-Apr-28 18:49 stempy/io/__init__.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-Apr-28 18:49 stempy/io/compatibility.py
+-rw-rw-rw-  2.0 fat    40225 b- defN 23-Apr-28 18:49 stempy/io/sparse_array.py
+-rw-rw-rw-  2.0 fat     1496 b- defN 23-Apr-28 18:49 stempy/pipeline/__init__.py
+-rw-rw-rw-  2.0 fat     1531 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       94 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1265 b- defN 23-Apr-28 18:59 stempy-3.3.4.dist-info/RECORD
+16 files, 22006741 bytes uncompressed, 2004085 bytes compressed:  90.9%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: stempy/io/sparse_array.py
 Comment: 
 
 Filename: stempy/pipeline/__init__.py
 Comment: 
 
-Filename: stempy-3.3.3.dist-info/LICENSE
+Filename: stempy-3.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: stempy-3.3.3.dist-info/METADATA
+Filename: stempy-3.3.4.dist-info/METADATA
 Comment: 
 
-Filename: stempy-3.3.3.dist-info/WHEEL
+Filename: stempy-3.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: stempy-3.3.3.dist-info/top_level.txt
+Filename: stempy-3.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: stempy-3.3.3.dist-info/RECORD
+Filename: stempy-3.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## stempy/stem.dll

### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x00000001800b7568
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Thu Apr  6 15:22:16 2023
+Time/Date		Fri Apr 28 18:59:23 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	29
 SizeOfCode		00000000000bb000
 SizeOfInitializedData	0000000000347000
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	00000000000b7568
@@ -25,15 +25,15 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	6
 MinorSubsystemVersion	0
 Win32Version		00000000
 SizeOfImage		00407000
 SizeOfHeaders		00000400
-CheckSum		00407561
+CheckSum		0040dd61
 Subsystem		00000002	(Windows GUI)
 DllCharacteristics	00000160
 					HIGH_ENTROPY_VA
 					DYNAMIC_BASE
 					NX_COMPAT
 SizeOfStackReserve	0000000000100000
 SizeOfStackCommit	0000000000001000
@@ -488346,16 +488346,17 @@
    1800bfa40:	movabs 0x4000000001803f9d,%al
    1800bfa49:	sahf
    1800bfa4a:	(bad)
    1800bfa4b:	addb   $0x0,(%rcx)
    1800bfa4e:	add    %al,(%rax)
    1800bfa50:	add    %al,(%rax)
    1800bfa52:	add    %al,(%rax)
-   1800bfa54:	test   $0xe3,%al
-   1800bfa56:	cs add %al,%fs:(%rax)
+   1800bfa54:	mov    (%rdi),%edx
+   1800bfa56:	rex.WR
+   1800bfa57:	add    %al,%fs:(%rax)
    1800bfa5a:	add    %al,(%rax)
    1800bfa5c:	or     $0x3c000000,%eax
    1800bfa61:	add    (%rax),%eax
    1800bfa63:	add    %cl,(%rax)
    1800bfa65:	push   %rsp
    1800bfa66:	or     $0x0,%al
    1800bfa68:	or     %cl,0xc(%rax)
```

## stempy/io/sparse_array.py

```diff
@@ -198,16 +198,18 @@
             metadata = {}
             if 'metadata' in f:
                 load_h5_to_dict(f['metadata'], metadata)
 
         scan_shape = scan_shape[::-1]
 
         if version >= 3:
+            # Convert to int to avoid integer division that results in 
+            # a float
+            frames_per_scan = len(data) // np.prod(scan_shape, dtype=int)
             # Need to reshape the data, as it was flattened before saving
-            frames_per_scan = len(data) // np.prod(scan_shape)
             data = data.reshape((np.prod(scan_shape), frames_per_scan))
 
         # We may need to convert the version of the data
         if version != cls.VERSION:
             kwargs = {
                 'data': data,
                 'scan_positions': scan_positions,
```

## Comparing `stempy-3.3.3.dist-info/LICENSE` & `stempy-3.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

