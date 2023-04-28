# Comparing `tmp/bamsalvage-0.1.6.tar.gz` & `tmp/bamsalvage-0.1.7.tar.gz`

## Comparing `bamsalvage-0.1.6.tar` & `bamsalvage-0.1.7.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0  1943761 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/log.2.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/requirements.txt
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/setup.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/src/bamsalvage/__init__.py
--rwxr-xr-x   0        0        0    25964 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/src/bamsalvage/_bamsalvage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/tests/test_bamsalvage.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/LICENSE
--rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 bamsalvage-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/cp.pdf
+-rw-r--r--   0        0        0  1943761 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/log.2.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/nohup.out
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/requirements.txt
+-rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/setup.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/tmp.png
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/src/bamsalvage/__init__.py
+-rwxr-xr-x   0        0        0    28381 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/src/bamsalvage/_bamsalvage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/tests/test_bamsalvage.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 bamsalvage-0.1.7/PKG-INFO
```

### Comparing `bamsalvage-0.1.6/log.2.txt` & `bamsalvage-0.1.7/log.2.txt`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.6/setup.py` & `bamsalvage-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.6/src/bamsalvage/_bamsalvage.py` & `bamsalvage-0.1.7/src/bamsalvage/_bamsalvage.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import argparse, struct
 import mgzip
 import zlib, logging, json
 import numba
 import numpy as np
 
 def version():
-    import bamsalvage
-    return bamsalvage.__version__
+    try:
+        import bamsalvage
+        return bamsalvage.__version__
+    except:
+        return '0.1.7'
 
 # Error handling
 class BAMException(Exception):
     """Exception for BAM decoding
     """
     NO_BAM_FILE = 0
     BLOCK_CORRUPTED = 1
@@ -49,29 +52,49 @@
         if kind == -3:
             return ''
         return 'Unknown error'
     kind = property(lambda s:s.__kind)
 
 # Optimized functions using Numba
 @numba.njit(cache=True)
-def convert_bytes_to_seq(buffer:bytes, start:int, l_seq:int, text:bytearray):
+def convert_bytes_to_seq(buffer:bytes, start:int, l_seq:int, text:bytearray)->None:
     """Convert 4-byte encoded sequence to ASCII
+    Args:
+        buffer (readonly byte array) : uncompressed block
+        start (int64) : start position
+        l_seq (int64) : length of the sequence
+        text (mutable byte array) : text
+    Raises:
+        BamException: BAM processing error
+    Returns:
+        void
     """
     bases = [61, 65, 67, 77, 71, 82, 83, 86, 84, 87, 89, 72, 75, 68, 66, 78] # '=ACMGRSVTWYHKDBN'
     j = 0
     end = start + (l_seq + 1) // 2
     for i in range(start, end):
         b = buffer[i]
         text[j] = bases[b >> 4]
         if j + 1 >= l_seq: break
         text[j+1] = bases[b & 15]
         j += 2
+
 @numba.njit(cache=True)
-def convert_bytes_to_qual(buffer:bytes, start:int, l_seq:int, text:bytearray):
-    """Convert byte array into QUAL sequence"""
+def convert_bytes_to_qual(buffer:bytes, start:int, l_seq:int, text:bytearray)->None:
+    """Convert byte array into QUAL sequence
+    Args:
+        buffer (readonly byte array) : uncompressed block
+        start (int64) : start position
+        l_seq (int64) : length of the sequence
+        text (mutable byte array) : text
+    Raises:
+        BamException: BAM processing error
+    Returns:
+        void
+    """
     for i in range(l_seq):
         text[i] = min(33 + buffer[start+i], 126)
 
 @numba.njit(cache=True)
 def scan_block_header(buffer:bytes, start:numba.int64)->numba.int64:
     """Scan magic number and signature bytes int data block"""
     # le_I = np.uint32
@@ -132,54 +155,54 @@
     Args:
         handler (_io.TextIOWrapper): File handler
         strict : Check block size and CRC32
 
     Raises:
         BamException: BAM processing error
     Returns:
-        _type_: _description_
+        bytearray : uncompressed block
     """
     current_pos = handler.tell()
     strict_mode = kwargs.get('strict', False)
     buf = handler.read(18)
     while buf[0] != 31 or buf[1] != 139 or buf[2] != 8 or buf[3] != 4 or buf[12] != 66 or buf[13] != 67:
         offset = False
         for i in range(1, 18):
             if buf[i] == 31:
                 offset = True
                 buf = buf[i:] + handler.read(i)
                 break
         if not offset:
             buf = handler.read(18)
         if len(buf) < 18: 
-            raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot scan header anymore AT {} '.format(handler.tell()))
+            raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot scan header anymore @{} '.format(handler.tell()))
             
     gzheader = struct.unpack('<BBBBIBBHBBHH', buf)
     xlen = gzheader[7]
     block_size = gzheader[11]
     if xlen >= 6 and block_size > xlen + 19:
         _skip_bytes = xlen - 6
         handler.read(_skip_bytes)
     if len(buf) < xlen:
-        raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot load gzipped block AT {} '.format(current_pos))
+        raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot load gzipped block @{} '.format(current_pos))
     compressed_data_size = block_size - xlen - 19
     return decompress_and_validate(handler, compressed_data_size, strict_mode)
 
     
 def read_next_block(handler, **kwargs):
     """Read BGZF block, block corruption is not assumed.
 
     Args:
         handler (_io.TextIOWrapper): File handler
         strict (bool) : Check block size and CRC32
 
     Raises:
         BamException: BAM processing error
     Returns:
-        _type_: _description_
+        bytearray : uncompressed block
     """
     # GZIP header, ID1=31, ID2=139
     strict_mode = kwargs.get('strict', False)
     buf = handler.read(2)
     if len(buf) < 2:
         raise BAMException(BAMException.BUFFER_TERMINATED, 'cannot scan header anymore')
     gzheader = struct.unpack('BB', buf)
@@ -205,48 +228,49 @@
     Raises:
         BAMException: Corrupted block detected
 
     Returns:
         byte array : data block
     """
     if compressed_data_size < 0:
-        raise BAMException(BAMException.NEGATIVE_DATA_SIZE, ' AT {} '.format(handler.tell()))
+        raise BAMException(BAMException.NEGATIVE_DATA_SIZE, ' @{} '.format(handler.tell()))
     current_pos = handler.tell()
     cdata = handler.read(compressed_data_size)
 
     decobj = zlib.decompressobj(-15) # no header
     try:
         decompressed = decobj.decompress(cdata) + decobj.flush()
     except Exception as e:
-        raise BAMException(BAMException.DECOMPRESSION_FAILURE, '{} AT {} '.format(str(e), current_pos))
+        raise BAMException(BAMException.DECOMPRESSION_FAILURE, '{} @{} '.format(str(e), current_pos))
 
     buf = handler.read(8)
     if len(buf) < 8:
-        raise BAMException(BAMException.BUFFER_TERMINATED, ' AT {} '.format(current_pos))
+        raise BAMException(BAMException.BUFFER_TERMINATED, ' @{} '.format(current_pos))
     crc32, input_size = struct.unpack('<II', buf)
     if not strict_mode:
         if 0 < len(decompressed) <= 65535:
             return decompressed
     if input_size == len(decompressed):
         crc32_calc = zlib.crc32(decompressed)
         if crc32_calc != crc32:            
-            raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x} AT {} '.format(crc32_calc, crc32, current_pos))
+            raise BAMException(BAMException.INCONSISTENT_CHECKSUM, 'CRC is {:x} , not {:x} @{} '.format(crc32_calc, crc32, current_pos))
         return decompressed
     else:
         # sys.stderr.write(f'inconsistent size of decompressed buffer {expected_size} / {len(data)}\n')
         raise BAMException(BAMException.INCONSISTENT_BLOCK_SIZE, 
-                           'inconsistent zlib size expected={}, decompressed={} AT {} '.format(
+                           'inconsistent zlib size expected={}, decompressed={} @{} '.format(
                                 input_size, len(decompressed), current_pos))
 
 def retrieve_fastq_from_bam(filename_bam:str, filename_fastq:str, **kwargs)->dict:
     """Retrieving fastq sequences from BAM file
 
     Args:
         filename_bam (str): BAM filename
         filename_fastq (str): Fastq filename 
+        split (int64) : split fastq by M read
 
     Returns:
         dict: information of results
     """
     verbose = kwargs.get('verbose', False)
     logger = kwargs.get('logger', None)
     if logger is None:
@@ -260,32 +284,41 @@
     info = {'input':filename_bam, 'output':filename_fastq}
     # force_continuation = kwargs.get('forced', False)
     limit = kwargs.get('limit', 0)
     seek_pos = kwargs.get('fileseek', 0)
     strict_mode = kwargs.get('strict', False) # check block size and CRC32
 
     fasta_mode = filename_fastq is None or re.search('\\.m?fa(\\.gz)?$', filename_fastq)
-
+    n_seqs_split = kwargs.get('split', 0) * 1000000
     if filename_fastq is None:
-        # ostr = None
-        ostr = sys.stdout
-    elif filename_fastq.endswith('.gz'):                                                                                                                                                   
-        n_threads = kwargs.get('threads', 4)
-        ostr = io.TextIOWrapper(mgzip.open(filename_fastq, 'wb', thread=n_threads))
-    else:
-        ostr = open(filename_fastq, 'w')
-        
+        n_seqs_split = 0
+    n_seqs_dump = n_seqs_split        
     filesize = os.path.getsize(filename_bam)
     tracking_data = [] # remember error positions
+    chunk_num = -1
+    fn_title, ext = os.path.splitext(filename_fastq)
+    output_files = []
+    ostr = sys.stdout
+    
+    if n_seqs_split > 0:
+        chunk_num = 1
+        filename_output = f'{fn_title}.{chunk_num}{ext}' if chunk_num > 0 else filename_fastq
+        output_files.append(filename_output)    
+        if filename_fastq.endswith('.gz'):                                                                                                                                                   
+            n_threads = kwargs.get('threads', 4)
+            ostr = io.TextIOWrapper(mgzip.open(filename_output, 'wb', thread=n_threads))
+        else:
+            ostr = open(filename_output, 'w')    
+        logger.info('sequences will be split by {:.1f}M reads'.format(n_seqs_split))
 
     MAXIMUM_BLOCK_SIZE = 1024 * 1024
     MINIMUM_READ_NAME = 2
     with open(filename_bam, 'rb') as fi:
         if seek_pos > 0:
-            logger.info('seek at {}'.format(seek_pos))
+            logger.info('seek @{}'.format(seek_pos))
             fi.seek(min(seek_pos, filesize))
 
         references = []
         n_blocks = 0
         pos = 0
         n_malformed_gzip_blocks = 0
         n_unaligned_blocks = 0
@@ -375,15 +408,15 @@
                 if file_ptr >= filesize: # check position is in the file size
                     tracking_data.append([BAMException.BUFFER_TERMINATED, file_ptr])
                     break
                 if pos > 0:
                     data = data[pos:]
                     pos = 0
                 if len(data) < 36: # buffer is empty
-                    logger.info(f'\033[Kbuffer size below 36 AT {file_ptr}\n')
+                    logger.info(f'\033[Kbuffer size below 36 @{file_ptr}\n')
                     data = []
                     pos = 0
                     break
                 block_size, refid, mappos, l_read_name, mapq, bai_bin, n_cigar_op, flag, l_seq, next_refid, next_pos, tlen \
                     = struct.unpack('<IiiBBHHHIiii', data[pos:pos + 36])
 
                 # assert variable range
@@ -441,14 +474,28 @@
                         if l_seq > 0:
                             convert_bytes_to_qual(data, pos, l_seq, sequence)
                             ostr.write('{}\n'.format(sequence.decode('ascii')))
                         # print('{}:{}\t{}\t{}\t{}/{}'.format(n_blocks, pos, seqid, seq[0:20] + '..' + seq[-20:], len(seq), len(qual)))
                         pos += l_seq
                 pos = ptr_block_start + block_size
                 if n_seqs % 1000 == 0:
+                    if chunk_num > 0 and n_seqs > n_seqs_dump:
+                        n_seqs_dump += n_seqs_split
+                        ostr.close()
+
+                        chunk_num += 1
+                        logger.info('Change file chunk to {} @{} '.format(chunk_num, fi.tell()))
+                        filename_output = f'{fn_title}.{chunk_num}{ext}' if chunk_num > 0 else filename_fastq
+                        output_files.append(filename_output)
+    
+                        if filename_fastq.endswith('.gz'):                                                                                                                                                   
+                            ostr = io.TextIOWrapper(mgzip.open(filename_output, 'wb', thread=n_threads))
+                        else:
+                            ostr = open(filename_output, 'w')    
+                    
                     if limit > 0 and n_seqs >= limit:
                         keep_running = False
                         break
                     percentage = fi.tell() / filesize * 100.0
                     sys.stderr.write('\033[K {:.1f}% {}\t{} kreads\t{} blocks ({} corrupted)\r'.format(
                         percentage, seqid[:16], n_seqs // 1000, n_blocks, len(tracking_data)))
 
@@ -519,15 +566,16 @@
     info['n_seqs'] = n_seqs
     info['n_blocks'] = n_blocks
     info['n_corrupted'] = n_malformed_gzip_blocks + n_unaligned_blocks
     info['n_malformed_gzip_blocks'] =  n_malformed_gzip_blocks
     info['n_unaligned_blocks'] = n_unaligned_blocks
     info['total_bases'] = total_bases
     info['error.log'] = tracking_data
-
+    if len(output_files) > 0:
+        info['chunks'] = output_files
     return info
 
 # def convert_bam_to_seq(filename_input, outdir, **kwargs):
 #     verbose = kwarge.get('verbose', False)
 #     mode = kwargs.mode('mode', 'fastq.gz')
 #     limit = kwargs.get('limit', 0)
 #     n_proc = kwargs.get('n_proc', 4)
@@ -537,24 +585,25 @@
     """Entry point of command "bamsalvage"
     """
     """
     c, b, B, ?, h, H, i, I, l, L, q, Q: 1, 1, 1, 1, 2, 2, 4, 4, 8, 8, 8, 8
     e, f, d : float 2, 4, 8
     """
     parser = argparse.ArgumentParser()
-    parser.add_argument('-i', '--input', nargs='+')
-    parser.add_argument('-o','--outdir', default=None)
-    parser.add_argument('--seek', default=0, type=int, help='seek position, start from given position by percent(0-100, default 0)')
-    parser.add_argument('--verbose', action='store_true')
+    parser.add_argument('-i', '--input', nargs='+', metavar='BAM file')
+    parser.add_argument('-o','--outdir', default=None, metavar='directory', help='Destination of sequences, standard output if not specified')
     parser.add_argument('--mode', choices=['test', 'fasta', 'fasta.gz', 'fastq', 'fastq.gz', 'fa.gz', 'fa', 'fz', 'fq', 'fqz'], default='fastq.gz',
                         help='output mode (test:no output, fq/fastq:fastq fqz/fastq.gz/gzipped fastq, fa/fasta:fasta, fz:gzipped fasta)')
+    parser.add_argument('--seek', default=0, type=int, help='seek position, start from given position by percent(0-100, default 0)')
     parser.add_argument('--limit', type=int, default=0)
-    parser.add_argument('-V', '--version', action='store_true', help='Show current version')
-    parser.add_argument('--strict', action='store_true', help='Check CRC32')
     parser.add_argument('-p', type=int, default=4, metavar='number', help='Number of threads for gzip compression, this option is ignored if mode is not gzipped output')
+    parser.add_argument('--not-strict', action='store_true', help='Skip length and CRC32 validation')
+    parser.add_argument('--verbose', action='store_true')
+    parser.add_argument('--split', type=int, metavar='number', help='split files by size (Mreads), default 0 (integrated)')
+    parser.add_argument('-V', '--version', action='store_true', help='Show current version')
     
     args, cmds = parser.parse_known_args()
     if args.version:
         print(version())
         exit()
     if args.input is None:
         bamfiles = []
@@ -576,25 +625,26 @@
         stdout_mode = False
     else:
         stdout_mode = True
     limit = args.limit
     mode = args.mode
     gzipped = mode in ('fz', 'fastq.gz', 'fqz', 'fasta.gz', 'fa.gz')
     fasta = mode in ('fa', 'fasta', 'fa.gz', 'fz')
+    split_size = args.split
 
     logger = _get_logger(os.path.basename(__file__))
     verbose = args.verbose
     if verbose:
         logger.setLevel(10)
     info = {
         'command':sys.argv,
         'input':filenames,
         'files':[],
     }
-    strict_mode = args.strict
+    strict_mode = not args.not_strict
     
     if filenames is None:
         raise Exception('no BAM files given')
 
     for filename in filenames:
         if filename.endswith('.bam'):
             title = os.path.basename(filename)[0:-4]
@@ -602,15 +652,15 @@
                 filename_out = None
             elif fasta:
                 filename_out = os.path.join(outdir, title + '.fa')
             else:
                 filename_out = os.path.join(outdir, title + '.fastq')
             if (not stdout_mode) and gzipped:
                 filename_out += '.gz'
-            finfo = retrieve_fastq_from_bam(filename, filename_out, verbose=verbose, limit=limit, threads=n_threads, fileseek=seek_pos, strict=strict_mode)
+            finfo = retrieve_fastq_from_bam(filename, filename_out, verbose=verbose, limit=limit, threads=n_threads, fileseek=seek_pos, strict=strict_mode, split=split_size)
             # output error log
             tracking_data = finfo.pop('error.log', [])
             if outdir is not None:
                 filename_log = os.path.join(outdir, '.{}.log'.format(os.path.basename(filename)))
                 with open(filename_log, 'w') as fo:
                     fo.write('#filename={}\n'.format(filename))
                     fo.write('#filesize={}\n'.format(os.path.getsize(filename)))
```

### Comparing `bamsalvage-0.1.6/.gitignore` & `bamsalvage-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.6/LICENSE` & `bamsalvage-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.6/README.md` & `bamsalvage-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `bamsalvage-0.1.6/pyproject.toml` & `bamsalvage-0.1.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bamsalvage"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Takaho A. Endo", email="takaho.endo@gmail.com"},
 ]
 description = "Sequence salvaging script from corrupted BAM files"
 readme = "README.md"
 licence = "MIT"
 requires-python = ">=3.7"
```

### Comparing `bamsalvage-0.1.6/PKG-INFO` & `bamsalvage-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bamsalvage
-Version: 0.1.6
+Version: 0.1.7
 Summary: Sequence salvaging script from corrupted BAM files
 Project-URL: Homepage, https://pypi.org/project/bamsalvage/
 Author-email: "Takaho A. Endo" <takaho.endo@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

