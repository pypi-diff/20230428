# Comparing `tmp/python3_utils_tdinoto-1.0.3.tar.gz` & `tmp/python3_utils_tdinoto-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/newuser/PycharmProjects/python3_utils_tdinoto/dist/.tmp-tc0hofwp/python3_utils_tdinoto-1.0.3.tar", last modified: Tue Feb 14 10:41:07 2023, max compression
+gzip compressed data, was "python3_utils_tdinoto-1.0.4.tar", last modified: Fri Apr 28 15:45:42 2023, max compression
```

## Comparing `python3_utils_tdinoto-1.0.3.tar` & `python3_utils_tdinoto-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxrwxr-x   0 newuser   (1003) newuser   (1003)        0 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     1067 2022-08-14 15:19:29.000000 python3_utils_tdinoto-1.0.3/LICENSE
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     2542 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/PKG-INFO
--rw-rw-r--   0 newuser   (1003) newuser   (1003)      756 2022-10-26 11:29:50.000000 python3_utils_tdinoto-1.0.3/README.md
--rw-rw-r--   0 newuser   (1003) newuser   (1003)      753 2023-02-14 10:37:39.000000 python3_utils_tdinoto-1.0.3/pyproject.toml
--rw-rw-r--   0 newuser   (1003) newuser   (1003)       38 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/setup.cfg
-drwxrwxr-x   0 newuser   (1003) newuser   (1003)        0 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/
-drwxrwxr-x   0 newuser   (1003) newuser   (1003)        0 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     2542 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/PKG-INFO
--rw-rw-r--   0 newuser   (1003) newuser   (1003)      551 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/SOURCES.txt
--rw-rw-r--   0 newuser   (1003) newuser   (1003)        1 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/dependency_links.txt
--rw-rw-r--   0 newuser   (1003) newuser   (1003)       34 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/requires.txt
--rw-rw-r--   0 newuser   (1003) newuser   (1003)       14 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/top_level.txt
-drwxrwxr-x   0 newuser   (1003) newuser   (1003)        0 2023-02-14 10:41:07.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/
--rw-rw-r--   0 newuser   (1003) newuser   (1003)        0 2022-08-14 13:34:35.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/__init__.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     1475 2022-10-26 09:43:10.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/numeric.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     8586 2023-02-14 10:24:13.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_bids_dcm_dataset.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)      360 2023-02-14 10:25:35.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_dict.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)    11479 2022-10-11 09:33:00.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_lists.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)    13505 2023-02-14 10:30:43.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_nifti_dicom.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     4715 2023-01-05 16:21:09.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_numpy.py
--rw-rw-r--   0 newuser   (1003) newuser   (1003)     2947 2022-10-11 07:08:39.000000 python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_strings.py
+drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.115136 python3_utils_tdinoto-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2600 2023-04-28 15:45:42.114181 python3_utils_tdinoto-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      778 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/README.md
+-rw-rw-rw-   0        0        0      779 2023-04-28 15:28:37.000000 python3_utils_tdinoto-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-28 15:45:42.115136 python3_utils_tdinoto-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.022699 python3_utils_tdinoto-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.053829 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/
+-rw-rw-rw-   0        0        0     2600 2023-04-28 15:45:41.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      581 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-04-28 15:45:42.000000 python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-28 15:45:42.113124 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/__init__.py
+-rw-rw-rw-   0        0        0     1509 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/numeric.py
+-rw-rw-rw-   0        0        0     8736 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_bids_dcm_dataset.py
+-rw-rw-rw-   0        0        0     1641 2023-04-12 13:20:11.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_dict.py
+-rw-rw-rw-   0        0        0      337 2023-04-03 13:25:55.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_io.py
+-rw-rw-rw-   0        0        0    11797 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_lists.py
+-rw-rw-rw-   0        0        0    13801 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_nifti_dicom.py
+-rw-rw-rw-   0        0        0     5255 2023-04-14 07:30:39.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_numpy.py
+-rw-rw-rw-   0        0        0     3045 2023-04-03 13:20:44.000000 python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_strings.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python3_utils_tdinoto-1.0.3/LICENSE` & `python3_utils_tdinoto-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2018 Real Python
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+MIT License
+
+Copyright (c) 2018 Real Python
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
```

### Comparing `python3_utils_tdinoto-1.0.3/PKG-INFO` & `python3_utils_tdinoto-1.0.4/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: python3_utils_tdinoto
-Version: 1.0.3
-Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
-Author-email: Tommaso Di Noto <tommydino@hotmail.it>
-License: MIT License
-        
-        Copyright (c) 2018 Real Python
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/tommydino93/python3_utils_tdinoto
-Keywords: utils,wrappers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Utils
-This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
-
-### Installation
-python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
-To install it, ensure you have python installed and then run:
-```python
-python3 -m pip install python3_utils_tdinoto
-```
-
-### Example usage
-```python
->>> from utils_tdinoto.utils_lists import find_common_elements
->>> list_1 = [1, 2, 3]
->>> list_2 = [3, 4, 5]
->>> find_common_elements(list_1, list_2)
-[3]
-
->>> from utils_tdinoto.utils_strings import keep_only_digits
->>> s = 'ses-20221026'
->>> keep_only_digits(s)
-'20221046'
-```
+Metadata-Version: 2.1
+Name: python3_utils_tdinoto
+Version: 1.0.4
+Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
+Author-email: Tommaso Di Noto <tommydino@hotmail.it>
+License: MIT License
+        
+        Copyright (c) 2018 Real Python
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/tommydino93/python3_utils_tdinoto
+Keywords: utils,wrappers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Utils
+This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
+
+### Installation
+python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
+To install it, ensure you have python installed and then run:
+```python
+python3 -m pip install python3_utils_tdinoto
+```
+
+### Example usage
+```python
+>>> from utils_tdinoto.utils_lists import find_common_elements
+>>> list_1 = [1, 2, 3]
+>>> list_2 = [3, 4, 5]
+>>> find_common_elements(list_1, list_2)
+[3]
+
+>>> from utils_tdinoto.utils_strings import keep_only_digits
+>>> s = 'ses-20221026'
+>>> keep_only_digits(s)
+'20221046'
+```
```

### Comparing `python3_utils_tdinoto-1.0.3/README.md` & `python3_utils_tdinoto-1.0.4/README.md`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Python Utils
-This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
-
-### Installation
-python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
-To install it, ensure you have python installed and then run:
-```python
-python3 -m pip install python3_utils_tdinoto
-```
-
-### Example usage
-```python
->>> from utils_tdinoto.utils_lists import find_common_elements
->>> list_1 = [1, 2, 3]
->>> list_2 = [3, 4, 5]
->>> find_common_elements(list_1, list_2)
-[3]
-
->>> from utils_tdinoto.utils_strings import keep_only_digits
->>> s = 'ses-20221026'
->>> keep_only_digits(s)
-'20221046'
+# Python Utils
+This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
+
+### Installation
+python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
+To install it, ensure you have python installed and then run:
+```python
+python3 -m pip install python3_utils_tdinoto
+```
+
+### Example usage
+```python
+>>> from utils_tdinoto.utils_lists import find_common_elements
+>>> list_1 = [1, 2, 3]
+>>> list_2 = [3, 4, 5]
+>>> find_common_elements(list_1, list_2)
+[3]
+
+>>> from utils_tdinoto.utils_strings import keep_only_digits
+>>> s = 'ses-20221026'
+>>> keep_only_digits(s)
+'20221046'
 ```
```

### Comparing `python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/PKG-INFO` & `python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-Metadata-Version: 2.1
-Name: python3-utils-tdinoto
-Version: 1.0.3
-Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
-Author-email: Tommaso Di Noto <tommydino@hotmail.it>
-License: MIT License
-        
-        Copyright (c) 2018 Real Python
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
-Project-URL: Homepage, https://github.com/tommydino93/python3_utils_tdinoto
-Keywords: utils,wrappers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Python Utils
-This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
-
-### Installation
-python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
-To install it, ensure you have python installed and then run:
-```python
-python3 -m pip install python3_utils_tdinoto
-```
-
-### Example usage
-```python
->>> from utils_tdinoto.utils_lists import find_common_elements
->>> list_1 = [1, 2, 3]
->>> list_2 = [3, 4, 5]
->>> find_common_elements(list_1, list_2)
-[3]
-
->>> from utils_tdinoto.utils_strings import keep_only_digits
->>> s = 'ses-20221026'
->>> keep_only_digits(s)
-'20221046'
-```
+Metadata-Version: 2.1
+Name: python3-utils-tdinoto
+Version: 1.0.4
+Summary: Useful wrapper functions for the most common python data types, and for nifti/dicom arrays.
+Author-email: Tommaso Di Noto <tommydino@hotmail.it>
+License: MIT License
+        
+        Copyright (c) 2018 Real Python
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+Project-URL: Homepage, https://github.com/tommydino93/python3_utils_tdinoto
+Keywords: utils,wrappers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Python Utils
+This repository contains wrapper functions and code snippets for the most common python dtypes. Truth is I'm tired of searching on Stack Overflow the same problems over and over again, so I am just gathering them here :)
+
+### Installation
+python_utils_tdinoto is OS independent and compatible with Python >= 3.7. 
+To install it, ensure you have python installed and then run:
+```python
+python3 -m pip install python3_utils_tdinoto
+```
+
+### Example usage
+```python
+>>> from utils_tdinoto.utils_lists import find_common_elements
+>>> list_1 = [1, 2, 3]
+>>> list_2 = [3, 4, 5]
+>>> find_common_elements(list_1, list_2)
+[3]
+
+>>> from utils_tdinoto.utils_strings import keep_only_digits
+>>> s = 'ses-20221026'
+>>> keep_only_digits(s)
+'20221046'
+```
```

### Comparing `python3_utils_tdinoto-1.0.3/src/python3_utils_tdinoto.egg-info/SOURCES.txt` & `python3_utils_tdinoto-1.0.4/src/python3_utils_tdinoto.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -6,11 +6,12 @@
 src/python3_utils_tdinoto.egg-info/dependency_links.txt
 src/python3_utils_tdinoto.egg-info/requires.txt
 src/python3_utils_tdinoto.egg-info/top_level.txt
 src/utils_tdinoto/__init__.py
 src/utils_tdinoto/numeric.py
 src/utils_tdinoto/utils_bids_dcm_dataset.py
 src/utils_tdinoto/utils_dict.py
+src/utils_tdinoto/utils_io.py
 src/utils_tdinoto/utils_lists.py
 src/utils_tdinoto/utils_nifti_dicom.py
 src/utils_tdinoto/utils_numpy.py
 src/utils_tdinoto/utils_strings.py
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/numeric.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/numeric.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import math
-
-
-def round_half_up(n: float,
-                  decimals: int = 0) -> float:
-    """This function rounds to the nearest integer number (e.g 2.4 becomes 2.0 and 2.6 becomes 3);
-     in case of tie, it rounds up (e.g. 1.5 becomes 2.0 and not 1.0)
-    Args:
-        n: number to round
-        decimals: number of decimal figures that we want to keep; defaults to zero
-    Returns:
-        rounded_number: input number rounded with the desired decimals
-    """
-    multiplier = 10 ** decimals
-
-    rounded_number = math.floor(n * multiplier + 0.5) / multiplier
-
-    return rounded_number
-
-
-def print_running_time(start_time: float,
-                       end_time: float, process_name: str) -> None:
-    """This function takes as input the start and the end time of a process and prints to console the time elapsed for this process
-    Args:
-        start_time: instant when the timer was started
-        end_time: instant when the timer was stopped
-        process_name: name of the process
-    """
-    sentence = str(process_name)  # convert to string whatever the user inputs as third argument
-    temp = end_time - start_time  # compute time difference
-    hours = temp // 3600  # compute hours
-    temp = temp - 3600 * hours  # if hours is not zero, remove equivalent amount of seconds
-    minutes = temp // 60  # compute minutes
-    seconds = temp - 60 * minutes  # compute minutes
+import math
+
+
+def round_half_up(n: float,
+                  decimals: int = 0) -> float:
+    """This function rounds to the nearest integer number (e.g 2.4 becomes 2.0 and 2.6 becomes 3);
+     in case of tie, it rounds up (e.g. 1.5 becomes 2.0 and not 1.0)
+    Args:
+        n: number to round
+        decimals: number of decimal figures that we want to keep; defaults to zero
+    Returns:
+        rounded_number: input number rounded with the desired decimals
+    """
+    multiplier = 10 ** decimals
+
+    rounded_number = math.floor(n * multiplier + 0.5) / multiplier
+
+    return rounded_number
+
+
+def print_running_time(start_time: float,
+                       end_time: float, process_name: str) -> None:
+    """This function takes as input the start and the end time of a process and prints to console the time elapsed for this process
+    Args:
+        start_time: instant when the timer was started
+        end_time: instant when the timer was stopped
+        process_name: name of the process
+    """
+    sentence = str(process_name)  # convert to string whatever the user inputs as third argument
+    temp = end_time - start_time  # compute time difference
+    hours = temp // 3600  # compute hours
+    temp = temp - 3600 * hours  # if hours is not zero, remove equivalent amount of seconds
+    minutes = temp // 60  # compute minutes
+    seconds = temp - 60 * minutes  # compute minutes
     print('\n%s time: %d hh %d mm %d ss' % (sentence, hours, minutes, seconds))
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_bids_dcm_dataset.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_bids_dcm_dataset.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import os
-import pydicom
-from collections import Counter
-import numpy as np
-from utils_tdinoto.utils_strings import keep_only_digits
-import SimpleITK as sitk
-import pandas as pd
-from utils_tdinoto.numeric import round_half_up
-
-
-def print_patient_sex_and_age(bids_dir: str, bids_dcm_dir: str) -> None:
-    """This function loops over a pseudo-BIDS dataset dir and prints the patient sex
-    Args:
-        bids_dir: directory containing the BIDS dataset
-        bids_dcm_dir: directory containing the dcm series of the dataset. A pseudo-BIDS organization is expected. Specifically:
-            sub-000
-                |__ses-yyyymm01
-                      |__dcm_series_1
-                      |__dcm_series_2
-                |__ses-yyyymm02
-                      |__dcm_series_1
-                      |__dcm_series_2
-    """
-    all_sex = []
-    all_ages = []
-    for sub in sorted(os.listdir(bids_dir)):
-        if "sub" in sub and os.path.isdir(os.path.join(bids_dir, sub)):
-            if len(os.listdir(os.path.join(bids_dir, sub))) >= 1:  # if there is at least one ses
-                first_ses = os.listdir(os.path.join(bids_dir, sub))[0]
-                if os.path.exists(os.path.join(bids_dcm_dir, sub, first_ses)):
-                    if len(os.listdir(os.path.join(bids_dcm_dir, sub, first_ses))) >= 1:  # if there is at least one series
-                        first_dcm_series = os.listdir(os.path.join(bids_dcm_dir, sub, first_ses))[0]
-                        if len(os.listdir(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series))) >= 1:  # if there is at least one dcm image
-                            first_dcm_img = os.listdir(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series))[0]
-                            first_dcm_img_tags = pydicom.dcmread(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series, first_dcm_img))
-                            sex = first_dcm_img_tags.PatientSex
-                            age = first_dcm_img_tags.PatientAge
-                            all_sex.append(sex)
-                            all_ages.append(age)
-                else:
-                    print(f"{sub}_{first_ses} missing")
-    print(f"\n{len(all_sex)} subjects found")
-    occurrence_count_sex = Counter(all_sex)
-    print(f"\nSex: {occurrence_count_sex}")
-    all_ages_only_numbers = [int(keep_only_digits(x)) for x in all_ages]
-    mean_age, std_age = np.mean(all_ages_only_numbers), np.std(all_ages_only_numbers)
-    print(f"\nAge: mean={mean_age}, std={std_age}")
-
-
-def print_median_values(df, scanner_name):
-    median_tr = df['TR'].median()
-    median_te = df['TE'].median()
-    median_spacing_x = df['spacing_x'].median()
-    median_spacing_y = df['spacing_y'].median()
-    median_spacing_z = df['spacing_z'].median()
-
-    print(f"\nmedian values {scanner_name}: TR = {round_half_up(median_tr)}, TE = {round_half_up(median_te)}, spacing = {median_spacing_x} x {median_spacing_y} x {median_spacing_z}")
-
-
-def find_mr_acquisition_params(bids_ds, dcm_dir):
-    cnt_subs = 0
-    vendor_scanner_field_strength = []
-    for sub in sorted(os.listdir(bids_ds)):
-        if "sub" in sub and os.path.isdir(os.path.join(bids_ds, sub)):
-            sub_dir_dmc_dir = os.path.join(dcm_dir, sub)
-            if os.path.isdir(sub_dir_dmc_dir):
-                cnt_subs += 1
-                # if cnt_subs % 100 == 0:
-                #     print(f"{cnt_subs}) {sub}:")
-                for ses in sorted(os.listdir(sub_dir_dmc_dir)):
-                    assert os.path.isdir(os.path.join(sub_dir_dmc_dir, ses))
-                    # print(f"    {ses}")
-                    for series in sorted(os.listdir(os.path.join(sub_dir_dmc_dir, ses))):
-                        assert os.path.isdir(os.path.join(sub_dir_dmc_dir, ses, series))
-                        cnt_images = 0
-                        img_position_patient = []
-                        for dcm_img in sorted(os.listdir(os.path.join(sub_dir_dmc_dir, ses, series))):
-                            cnt_images += 1
-                            one_dcm_img = pydicom.dcmread(os.path.join(sub_dir_dmc_dir, ses, series, dcm_img))
-                            manufacturer = one_dcm_img.Manufacturer
-                            model = one_dcm_img.ManufacturerModelName
-                            field_strength = one_dcm_img.MagneticFieldStrength
-                            tr = one_dcm_img.RepetitionTime
-                            te = one_dcm_img.EchoTime
-
-                            sitk_img = sitk.ReadImage(os.path.join(sub_dir_dmc_dir, ses, series, dcm_img))
-                            voxel_spacing = sitk_img.GetSpacing()
-                            spacing_x = round(voxel_spacing[0], 2)
-                            spacing_y = round(voxel_spacing[1], 2)
-                            spacing_z = round(voxel_spacing[2], 2)
-
-                            vendor_scanner_field_strength.append([manufacturer, model, field_strength, tr, te, spacing_x, spacing_y, spacing_z])
-                            break  # we only loop through one image
-                        break  # we only loop through one series
-            else:
-                print(f"{sub} missing")
-
-    df_vendor_scanner_field_strength = pd.DataFrame(vendor_scanner_field_strength, columns=['vendor', 'scanner', 'field_strength', 'TR', 'TE', 'spacing_x', 'spacing_y', 'spacing_z'])
-
-    # re-adjust weird values
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.field_strength < 1.5, 'field_strength'] = 1.5
-    df_vendor_scanner_field_strength.loc[(df_vendor_scanner_field_strength.field_strength < 3.0) & (df_vendor_scanner_field_strength.field_strength > 2.8), 'field_strength'] = 3.0
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Trio', 'scanner'] = 'TrioTim'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Skyra_fit', 'scanner'] = 'Skyra'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Prisma_fit', 'scanner'] = 'Prisma'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'SymphonyVision', 'scanner'] = 'Symphony'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'GENESIS_SIGNA', 'scanner'] = 'Signa'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Signa HDxt', 'scanner'] = 'Signa'
-    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.field_strength == 15000, 'field_strength'] = 1.5
-
-    # sort dataframe
-    df_vendor_scanner_field_strength_sorted = df_vendor_scanner_field_strength.sort_values(["vendor", "scanner"], ignore_index=True)  # ignore_index=True re-starts the indexes from 0
-
-    print()
-    print(df_vendor_scanner_field_strength_sorted.value_counts(["vendor", "scanner"]))
-
-    df_intera = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Intera"]
-    df_skyra = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Skyra"]
-    df_symphony = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Symphony"]
-    df_triotim = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "TrioTim"]
-    df_verio = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Verio"]
-    df_aera = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Aera"]
-    df_prisma = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Prisma"]
-
-    if not df_intera.empty:
-        print_median_values(df_intera, scanner_name="Intera")
-    if not df_skyra.empty:
-        print_median_values(df_skyra, scanner_name="Skyra")
-    if not df_symphony.empty:
-        print_median_values(df_symphony, scanner_name="Symphony")
-    if not df_triotim.empty:
-        print_median_values(df_triotim, scanner_name="TrioTim")
-    if not df_verio.empty:
-        print_median_values(df_verio, scanner_name="Verio")
-    if not df_aera.empty:
-        print_median_values(df_aera, scanner_name="Aera")
-    if not df_prisma.empty:
-        print_median_values(df_prisma, scanner_name="Prisma")
-
-
-def main():
-    # input args
-    path_bids_ds = "/path/to/BIDS_Dataset/"
-    all_dicoms = "/path/to/dir/ALL_DICOMS/"
-    print_patient_sex_and_age(path_bids_ds, all_dicoms)
-    find_mr_acquisition_params(path_bids_ds, all_dicoms)
-
-
-if __name__ == '__main__':
-    main()
+import os
+import pydicom
+from collections import Counter
+import numpy as np
+from utils_tdinoto.utils_strings import keep_only_digits
+import SimpleITK as sitk
+import pandas as pd
+from utils_tdinoto.numeric import round_half_up
+
+
+def print_patient_sex_and_age(bids_dir: str, bids_dcm_dir: str) -> None:
+    """This function loops over a pseudo-BIDS dataset dir and prints the patient sex
+    Args:
+        bids_dir: directory containing the BIDS dataset
+        bids_dcm_dir: directory containing the dcm series of the dataset. A pseudo-BIDS organization is expected. Specifically:
+            sub-000
+                |__ses-yyyymm01
+                      |__dcm_series_1
+                      |__dcm_series_2
+                |__ses-yyyymm02
+                      |__dcm_series_1
+                      |__dcm_series_2
+    """
+    all_sex = []
+    all_ages = []
+    for sub in sorted(os.listdir(bids_dir)):
+        if "sub" in sub and os.path.isdir(os.path.join(bids_dir, sub)):
+            if len(os.listdir(os.path.join(bids_dir, sub))) >= 1:  # if there is at least one ses
+                first_ses = os.listdir(os.path.join(bids_dir, sub))[0]
+                if os.path.exists(os.path.join(bids_dcm_dir, sub, first_ses)):
+                    if len(os.listdir(os.path.join(bids_dcm_dir, sub, first_ses))) >= 1:  # if there is at least one series
+                        first_dcm_series = os.listdir(os.path.join(bids_dcm_dir, sub, first_ses))[0]
+                        if len(os.listdir(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series))) >= 1:  # if there is at least one dcm image
+                            first_dcm_img = os.listdir(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series))[0]
+                            first_dcm_img_tags = pydicom.dcmread(os.path.join(bids_dcm_dir, sub, first_ses, first_dcm_series, first_dcm_img))
+                            sex = first_dcm_img_tags.PatientSex
+                            age = first_dcm_img_tags.PatientAge
+                            all_sex.append(sex)
+                            all_ages.append(age)
+                else:
+                    print(f"{sub}_{first_ses} missing")
+    print(f"\n{len(all_sex)} subjects found")
+    occurrence_count_sex = Counter(all_sex)
+    print(f"\nSex: {occurrence_count_sex}")
+    all_ages_only_numbers = [int(keep_only_digits(x)) for x in all_ages]
+    mean_age, std_age = np.mean(all_ages_only_numbers), np.std(all_ages_only_numbers)
+    print(f"\nAge: mean={mean_age}, std={std_age}")
+
+
+def print_median_values(df, scanner_name):
+    median_tr = df['TR'].median()
+    median_te = df['TE'].median()
+    median_spacing_x = df['spacing_x'].median()
+    median_spacing_y = df['spacing_y'].median()
+    median_spacing_z = df['spacing_z'].median()
+
+    print(f"\nmedian values {scanner_name}: TR = {round_half_up(median_tr)}, TE = {round_half_up(median_te)}, spacing = {median_spacing_x} x {median_spacing_y} x {median_spacing_z}")
+
+
+def find_mr_acquisition_params(bids_ds, dcm_dir):
+    cnt_subs = 0
+    vendor_scanner_field_strength = []
+    for sub in sorted(os.listdir(bids_ds)):
+        if "sub" in sub and os.path.isdir(os.path.join(bids_ds, sub)):
+            sub_dir_dmc_dir = os.path.join(dcm_dir, sub)
+            if os.path.isdir(sub_dir_dmc_dir):
+                cnt_subs += 1
+                # if cnt_subs % 100 == 0:
+                #     print(f"{cnt_subs}) {sub}:")
+                for ses in sorted(os.listdir(sub_dir_dmc_dir)):
+                    assert os.path.isdir(os.path.join(sub_dir_dmc_dir, ses))
+                    # print(f"    {ses}")
+                    for series in sorted(os.listdir(os.path.join(sub_dir_dmc_dir, ses))):
+                        assert os.path.isdir(os.path.join(sub_dir_dmc_dir, ses, series))
+                        cnt_images = 0
+                        img_position_patient = []
+                        for dcm_img in sorted(os.listdir(os.path.join(sub_dir_dmc_dir, ses, series))):
+                            cnt_images += 1
+                            one_dcm_img = pydicom.dcmread(os.path.join(sub_dir_dmc_dir, ses, series, dcm_img))
+                            manufacturer = one_dcm_img.Manufacturer
+                            model = one_dcm_img.ManufacturerModelName
+                            field_strength = one_dcm_img.MagneticFieldStrength
+                            tr = one_dcm_img.RepetitionTime
+                            te = one_dcm_img.EchoTime
+
+                            sitk_img = sitk.ReadImage(os.path.join(sub_dir_dmc_dir, ses, series, dcm_img))
+                            voxel_spacing = sitk_img.GetSpacing()
+                            spacing_x = round(voxel_spacing[0], 2)
+                            spacing_y = round(voxel_spacing[1], 2)
+                            spacing_z = round(voxel_spacing[2], 2)
+
+                            vendor_scanner_field_strength.append([manufacturer, model, field_strength, tr, te, spacing_x, spacing_y, spacing_z])
+                            break  # we only loop through one image
+                        break  # we only loop through one series
+            else:
+                print(f"{sub} missing")
+
+    df_vendor_scanner_field_strength = pd.DataFrame(vendor_scanner_field_strength, columns=['vendor', 'scanner', 'field_strength', 'TR', 'TE', 'spacing_x', 'spacing_y', 'spacing_z'])
+
+    # re-adjust weird values
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.field_strength < 1.5, 'field_strength'] = 1.5
+    df_vendor_scanner_field_strength.loc[(df_vendor_scanner_field_strength.field_strength < 3.0) & (df_vendor_scanner_field_strength.field_strength > 2.8), 'field_strength'] = 3.0
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Trio', 'scanner'] = 'TrioTim'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Skyra_fit', 'scanner'] = 'Skyra'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Prisma_fit', 'scanner'] = 'Prisma'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'SymphonyVision', 'scanner'] = 'Symphony'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'GENESIS_SIGNA', 'scanner'] = 'Signa'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.scanner == 'Signa HDxt', 'scanner'] = 'Signa'
+    df_vendor_scanner_field_strength.loc[df_vendor_scanner_field_strength.field_strength == 15000, 'field_strength'] = 1.5
+
+    # sort dataframe
+    df_vendor_scanner_field_strength_sorted = df_vendor_scanner_field_strength.sort_values(["vendor", "scanner"], ignore_index=True)  # ignore_index=True re-starts the indexes from 0
+
+    print()
+    print(df_vendor_scanner_field_strength_sorted.value_counts(["vendor", "scanner"]))
+
+    df_intera = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Intera"]
+    df_skyra = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Skyra"]
+    df_symphony = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Symphony"]
+    df_triotim = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "TrioTim"]
+    df_verio = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Verio"]
+    df_aera = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Aera"]
+    df_prisma = df_vendor_scanner_field_strength_sorted.loc[df_vendor_scanner_field_strength_sorted["scanner"] == "Prisma"]
+
+    if not df_intera.empty:
+        print_median_values(df_intera, scanner_name="Intera")
+    if not df_skyra.empty:
+        print_median_values(df_skyra, scanner_name="Skyra")
+    if not df_symphony.empty:
+        print_median_values(df_symphony, scanner_name="Symphony")
+    if not df_triotim.empty:
+        print_median_values(df_triotim, scanner_name="TrioTim")
+    if not df_verio.empty:
+        print_median_values(df_verio, scanner_name="Verio")
+    if not df_aera.empty:
+        print_median_values(df_aera, scanner_name="Aera")
+    if not df_prisma.empty:
+        print_median_values(df_prisma, scanner_name="Prisma")
+
+
+def main():
+    # input args
+    path_bids_ds = "/path/to/BIDS_Dataset/"
+    all_dicoms = "/path/to/dir/ALL_DICOMS/"
+    print_patient_sex_and_age(path_bids_ds, all_dicoms)
+    find_mr_acquisition_params(path_bids_ds, all_dicoms)
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_lists.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_lists.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,318 +1,318 @@
-import os
-import pickle
-from collections import Counter
-import glob
-import random
-from typing import Any, Tuple
-import operator
-
-
-def save_list_to_disk_with_pickle(list_to_save: list,
-                                  out_dir: str,
-                                  out_filename: str) -> None:
-    """This function saves a list to disk
-    Args:
-        list_to_save: list that we want to save
-        out_dir: path to output folder; will be created if not present
-        out_filename: output filename
-    """
-    if not os.path.exists(out_dir):  # if output folder does not exist
-        os.makedirs(out_dir)  # create it
-    open_file = open(os.path.join(out_dir, out_filename), "wb")
-    pickle.dump(list_to_save, open_file)  # save list with pickle
-    open_file.close()
-
-
-def load_list_from_disk_with_pickle(path_to_list: str) -> list:
-    """This function loads a list from disk
-    Args:
-        path_to_list: path to where the list is saved
-    Returns:
-        loaded_list: loaded list
-    Raises:
-        AssertionError: if list path does not exist
-    """
-    assert os.path.exists(path_to_list), "Path {} does not exist".format(path_to_list)
-    open_file = open(path_to_list, "rb")
-    loaded_list = pickle.load(open_file)  # load from disk
-    open_file.close()
-
-    return loaded_list
-
-
-def load_list_from_partial_name_with_glob(input_dir: str,
-                                          partial_filename: str) -> list:
-    """This function loads a list from disk by knowing only part of the filename
-    Args:
-        input_dir: directory where list was saved
-        partial_filename: partial filename (use * as wildcare)
-    Returns:
-        list_of_interest: loaded list
-    Example:
-        # suppose the filename is y_true_fold_1, we can call:
-        >>> y_true = load_list_with_glob(path_to_dir, 'y_true*')
-    """
-    file_path = glob.glob(os.path.join(input_dir, partial_filename))  # type: list
-    assert len(file_path) == 1, "We expect only one filename to match"
-    list_of_interest = load_list_from_disk_with_pickle(file_path[0])
-
-    return list_of_interest
-
-
-def find_common_elements(list1: list,
-                         list2: list) -> list:
-    """This function takes as input two lists and returns a list with the common elements
-    Args:
-        list1: first list
-        list2: second list
-    Returns:
-        intersection_as_list: list containing the common elements between the two input lists
-    """
-    list1_as_set = set(list1)  # type: set
-    intersection = list1_as_set.intersection(list2)  # type: set
-    intersection_as_list = list(intersection)  # type: list
-
-    return intersection_as_list
-
-
-def most_frequent_n_elements(input_list: list,
-                             n: int) -> Any:
-    """This function is given a list as input and it returns its most frequent element
-    Args:
-        input_list: list where we search the most frequent element
-        n: number of most frequent elements we want to retrieve
-    Returns:
-        most_frequent_item (*): most frequent item in the list; can be of Any type
-    """
-    occurrence_count = Counter(input_list)  # type: Counter
-    most_frequent_n_items = occurrence_count.most_common(n)
-
-    return most_frequent_n_items
-
-
-def flatten_list(list_of_lists: list) -> list:
-    """This function flattens the input list
-    Args:
-        list_of_lists: input list of lists that we want to flatten
-    Returns:
-        flattened_list: flattened list
-    """
-    flattened_list = [item for sublist in list_of_lists for item in sublist]
-
-    return flattened_list
-
-
-def find_difference_list(list1: list,
-                         list2: list) -> list:
-    """This function takes as input two lists and returns the difference list between them
-    Args:
-        list1: first list
-        list2: second list
-    Returns:
-        difference_list: list containing the difference elements between the two input lists
-    """
-    difference_list = list(set(list1) - set(list2))
-
-    return difference_list
-
-
-def split_list_equal_sized_groups(lst: list,
-                                  n: int,
-                                  seed: int = 123) -> list:
-    """This function splits a list in n approximately equal-sized subgroups
-    Args:
-        lst: input list that we want to split
-        n: number of splits
-        seed: random seed to use; defaults to 123
-    Returns:
-        out_list: list of lists, where each internal list is one split
-    """
-    random.Random(seed).shuffle(lst)  # shuffle list with fixed seed
-    division = len(lst) / float(n)  # find number of items per split
-    out_list = [lst[int(round(division * i)): int(round(division * (i + 1)))] for i in range(n)]  # list of lists
-    return out_list
-
-
-def find_indexes_where_lists_differ(list1: list,
-                                    list2: list) -> list:
-    """This function returns the indexes where the two input lists differ. The input lists are expected to have same length
-    Args:
-        list1: first input list
-        list2: second input list
-    Returns:
-        out_list: output list containing the indexes where the two input list differ
-    Raises:
-        AssertionError: if the two input lists do not have the same length
-    """
-    assert len(list1) == len(list2), "The two input lists must have same length"
-    out_list = [idx for idx, (first, second) in enumerate(zip(list1, list2)) if first != second]
-    return out_list
-
-
-def extract_unique_elements(lst: list,
-                            ordered: bool = True) -> list:
-    """This function extracts the unique elements of the input list (i.e. it removes duplicates)
-    and returns them as an output list; if ordered=True (as by default), the returned list is ordered.
-    Args:
-        lst: input list from which we want to extract the unique elements
-        ordered: whether the output list of unique values is sorted or not; True by default
-    Returns:
-        out_list: list containing unique values
-    """
-    out_list = list(set(lst))  # type: list
-
-    if ordered:  # if we want to sort the list of unique values
-        out_list.sort()  # type: list
-
-    return out_list
-
-
-def find_idxs_of_element_in_list(lst: list,
-                                 element: Any) -> list:
-    """This function returns the indexes of the input list that have value == element
-    Args:
-        lst: input list where we search for indexes
-        element: element of which we want to find the indexes
-    Returns:
-        idxs: list of indexes corresponding to element
-    """
-    idxs = [i for i, x in enumerate(lst) if x == element]
-
-    return idxs
-
-
-def list_is_nested(input_list: list) -> bool:
-    """This function checks whether the input_list is nested (i.e. it is a list of lists).
-    Args:
-        input_list: the input list
-    Returns:
-        is_nested: True if list is nested, False if it isn’t
-    """
-    is_nested = any(isinstance(i, list) for i in input_list)
-
-    return is_nested
-
-
-def list_has_duplicates(input_list: list) -> bool:
-    """This function checks whether the input_list contains duplicates or not.
-    Args:
-        input_list: the input list where we look for duplicates
-    Returns:
-        has_duplicates: True if list has duplicates, False if it doesn't
-    """
-    if list_is_nested(input_list):
-        input_list = flatten_list(input_list)  # flatten list
-    has_duplicates = len(input_list) != len(set(input_list))
-
-    return has_duplicates
-
-
-def first_argmax(input_list: list) -> int:
-    """This function returns the index of the max value. If there are duplicate max values in input_list,
-    the index of the first maximum value found will be returned.
-    Args:
-        input_list: list for which we want to find the argmax
-    Returns:
-        idx_max: index corresponding to the maximum value
-    """
-    idx_max = input_list.index(max(input_list))
-
-    return idx_max
-
-
-def shuffle_two_lists_with_same_order(x: list,
-                                      y: list,
-                                      chosen_seed: int = 123) -> Tuple[list, list]:
-    """This function shuffles the two input lists with the same order
-    Args:
-        x: first input list
-        y: second input list
-        chosen_seed: seed to set for reproducibility
-    Returns:
-        shuffled_x: shuffled version of first list
-        shuffled_y: shuffled version of second list
-    Raises:
-        AssertionError: if the two input lists do not have the same length
-    """
-    assert len(x) == len(y), "The two input lists must have the same length"
-    random.seed(chosen_seed)  # set seed for reproducibility
-    zipped_x_and_y = list(zip(x, y))  # zip x and y together so we don't lose the order when shuffling
-    random.shuffle(zipped_x_and_y)  # shuffle
-    shuffled_x, shuffled_y = zip(*zipped_x_and_y)  # unzip into x and y
-
-    return shuffled_x, shuffled_y
-
-
-def slice_by_index(lst: list,
-                   indexes) -> list:
-    """Slice list by positional indexes.
-    Args:
-        lst: list to slice.
-        indexes: iterable of 0-based indexes of the list positions to return.
-    Returns:
-        a new list containing elements of lst on positions specified by indexes.
-    Examples:
-        >>> slice_by_index([], [])
-        []
-        >>> slice_by_index([], [0, 1])
-        []
-        >>> slice_by_index(['a', 'b', 'c'], [])
-        []
-        >>> slice_by_index(['a', 'b', 'c'], [0, 2])
-        ['a', 'c']
-        >>> slice_by_index(['a', 'b', 'c'], [0, 1])
-        ['a', 'b']
-        >>> slice_by_index(['a', 'b', 'c'], [1])
-        ['b']
-    """
-    if not lst or not indexes:
-        return []
-    slice_ = operator.itemgetter(*indexes)(lst)
-    if len(indexes) == 1:
-        return [slice_]
-    return list(slice_)
-
-
-def keep_only_duplicates(input_list: list) -> list:
-    """This function removes all unique values from input_list and keeps only the duplicates
-    Args:
-        input_list: list from which we want to remove unique values
-    Returns:
-        list_only_with_duplicates: output list that only contains the duplicates
-    Example:
-        >>> l = [1, 2, 2, 3, 3, 3, 4]
-        >>> out_list = keep_only_duplicates(l)
-        >>> out_list
-        [2,3]
-    """
-    counts = Counter(input_list)
-    list_only_with_duplicates = [id for id in counts if counts[id] > 1]
-
-    return list_only_with_duplicates
-
-
-def check_if_string_is_in_any_item_of_list(input_list: list,
-                                           match_string: str) -> bool:
-    """This function checks whether match_string is in any of the items of input_list;
-    if yes, it returns True, otherwise it returns False.
-    Args:
-       input_list: input list where we search for a match
-       match_string: string to match
-    Returns:
-        list_contains_match_string: True if list contains match_string; False otherwise
-    """
-    list_contains_match_string = bool([item for item in input_list if (match_string in item)])
-
-    return list_contains_match_string
-
-
-def all_elements_in_list_are_identical(input_list: list) -> bool:
-    """This function checks whether all the elements in input_list are identical. If they are, True is returned; otherwise, False is returned
-    Args:
-        input_list: input list for which we check that all elements are identical
-    Returns:
-        all_elements_are_identical: bool that indicates whether all elements are identical or not
-    """
-    all_elements_are_identical = all(x == input_list[0] for x in input_list)
-
-    return all_elements_are_identical
+import os
+import pickle
+from collections import Counter
+import glob
+import random
+from typing import Any, Tuple
+import operator
+
+
+def save_list_to_disk_with_pickle(list_to_save: list,
+                                  out_dir: str,
+                                  out_filename: str) -> None:
+    """This function saves a list to disk
+    Args:
+        list_to_save: list that we want to save
+        out_dir: path to output folder; will be created if not present
+        out_filename: output filename
+    """
+    if not os.path.exists(out_dir):  # if output folder does not exist
+        os.makedirs(out_dir)  # create it
+    open_file = open(os.path.join(out_dir, out_filename), "wb")
+    pickle.dump(list_to_save, open_file)  # save list with pickle
+    open_file.close()
+
+
+def load_list_from_disk_with_pickle(path_to_list: str) -> list:
+    """This function loads a list from disk
+    Args:
+        path_to_list: path to where the list is saved
+    Returns:
+        loaded_list: loaded list
+    Raises:
+        AssertionError: if list path does not exist
+    """
+    assert os.path.exists(path_to_list), "Path {} does not exist".format(path_to_list)
+    open_file = open(path_to_list, "rb")
+    loaded_list = pickle.load(open_file)  # load from disk
+    open_file.close()
+
+    return loaded_list
+
+
+def load_list_from_partial_name_with_glob(input_dir: str,
+                                          partial_filename: str) -> list:
+    """This function loads a list from disk by knowing only part of the filename
+    Args:
+        input_dir: directory where list was saved
+        partial_filename: partial filename (use * as wildcare)
+    Returns:
+        list_of_interest: loaded list
+    Example:
+        # suppose the filename is y_true_fold_1, we can call:
+        >>> y_true = load_list_with_glob(path_to_dir, 'y_true*')
+    """
+    file_path = glob.glob(os.path.join(input_dir, partial_filename))  # type: list
+    assert len(file_path) == 1, "We expect only one filename to match"
+    list_of_interest = load_list_from_disk_with_pickle(file_path[0])
+
+    return list_of_interest
+
+
+def find_common_elements(list1: list,
+                         list2: list) -> list:
+    """This function takes as input two lists and returns a list with the common elements
+    Args:
+        list1: first list
+        list2: second list
+    Returns:
+        intersection_as_list: list containing the common elements between the two input lists
+    """
+    list1_as_set = set(list1)  # type: set
+    intersection = list1_as_set.intersection(list2)  # type: set
+    intersection_as_list = list(intersection)  # type: list
+
+    return intersection_as_list
+
+
+def most_frequent_n_elements(input_list: list,
+                             n: int) -> Any:
+    """This function is given a list as input and it returns its most frequent element
+    Args:
+        input_list: list where we search the most frequent element
+        n: number of most frequent elements we want to retrieve
+    Returns:
+        most_frequent_item (*): most frequent item in the list; can be of Any type
+    """
+    occurrence_count = Counter(input_list)  # type: Counter
+    most_frequent_n_items = occurrence_count.most_common(n)
+
+    return most_frequent_n_items
+
+
+def flatten_list(list_of_lists: list) -> list:
+    """This function flattens the input list
+    Args:
+        list_of_lists: input list of lists that we want to flatten
+    Returns:
+        flattened_list: flattened list
+    """
+    flattened_list = [item for sublist in list_of_lists for item in sublist]
+
+    return flattened_list
+
+
+def find_difference_list(list1: list,
+                         list2: list) -> list:
+    """This function takes as input two lists and returns the difference list between them
+    Args:
+        list1: first list
+        list2: second list
+    Returns:
+        difference_list: list containing the difference elements between the two input lists
+    """
+    difference_list = list(set(list1) - set(list2))
+
+    return difference_list
+
+
+def split_list_equal_sized_groups(lst: list,
+                                  n: int,
+                                  seed: int = 123) -> list:
+    """This function splits a list in n approximately equal-sized subgroups
+    Args:
+        lst: input list that we want to split
+        n: number of splits
+        seed: random seed to use; defaults to 123
+    Returns:
+        out_list: list of lists, where each internal list is one split
+    """
+    random.Random(seed).shuffle(lst)  # shuffle list with fixed seed
+    division = len(lst) / float(n)  # find number of items per split
+    out_list = [lst[int(round(division * i)): int(round(division * (i + 1)))] for i in range(n)]  # list of lists
+    return out_list
+
+
+def find_indexes_where_lists_differ(list1: list,
+                                    list2: list) -> list:
+    """This function returns the indexes where the two input lists differ. The input lists are expected to have same length
+    Args:
+        list1: first input list
+        list2: second input list
+    Returns:
+        out_list: output list containing the indexes where the two input list differ
+    Raises:
+        AssertionError: if the two input lists do not have the same length
+    """
+    assert len(list1) == len(list2), "The two input lists must have same length"
+    out_list = [idx for idx, (first, second) in enumerate(zip(list1, list2)) if first != second]
+    return out_list
+
+
+def extract_unique_elements(lst: list,
+                            ordered: bool = True) -> list:
+    """This function extracts the unique elements of the input list (i.e. it removes duplicates)
+    and returns them as an output list; if ordered=True (as by default), the returned list is ordered.
+    Args:
+        lst: input list from which we want to extract the unique elements
+        ordered: whether the output list of unique values is sorted or not; True by default
+    Returns:
+        out_list: list containing unique values
+    """
+    out_list = list(set(lst))  # type: list
+
+    if ordered:  # if we want to sort the list of unique values
+        out_list.sort()  # type: list
+
+    return out_list
+
+
+def find_idxs_of_element_in_list(lst: list,
+                                 element: Any) -> list:
+    """This function returns the indexes of the input list that have value == element
+    Args:
+        lst: input list where we search for indexes
+        element: element of which we want to find the indexes
+    Returns:
+        idxs: list of indexes corresponding to element
+    """
+    idxs = [i for i, x in enumerate(lst) if x == element]
+
+    return idxs
+
+
+def list_is_nested(input_list: list) -> bool:
+    """This function checks whether the input_list is nested (i.e. it is a list of lists).
+    Args:
+        input_list: the input list
+    Returns:
+        is_nested: True if list is nested, False if it isn’t
+    """
+    is_nested = any(isinstance(i, list) for i in input_list)
+
+    return is_nested
+
+
+def list_has_duplicates(input_list: list) -> bool:
+    """This function checks whether the input_list contains duplicates or not.
+    Args:
+        input_list: the input list where we look for duplicates
+    Returns:
+        has_duplicates: True if list has duplicates, False if it doesn't
+    """
+    if list_is_nested(input_list):
+        input_list = flatten_list(input_list)  # flatten list
+    has_duplicates = len(input_list) != len(set(input_list))
+
+    return has_duplicates
+
+
+def first_argmax(input_list: list) -> int:
+    """This function returns the index of the max value. If there are duplicate max values in input_list,
+    the index of the first maximum value found will be returned.
+    Args:
+        input_list: list for which we want to find the argmax
+    Returns:
+        idx_max: index corresponding to the maximum value
+    """
+    idx_max = input_list.index(max(input_list))
+
+    return idx_max
+
+
+def shuffle_two_lists_with_same_order(x: list,
+                                      y: list,
+                                      chosen_seed: int = 123) -> Tuple[list, list]:
+    """This function shuffles the two input lists with the same order
+    Args:
+        x: first input list
+        y: second input list
+        chosen_seed: seed to set for reproducibility
+    Returns:
+        shuffled_x: shuffled version of first list
+        shuffled_y: shuffled version of second list
+    Raises:
+        AssertionError: if the two input lists do not have the same length
+    """
+    assert len(x) == len(y), "The two input lists must have the same length"
+    random.seed(chosen_seed)  # set seed for reproducibility
+    zipped_x_and_y = list(zip(x, y))  # zip x and y together so we don't lose the order when shuffling
+    random.shuffle(zipped_x_and_y)  # shuffle
+    shuffled_x, shuffled_y = zip(*zipped_x_and_y)  # unzip into x and y
+
+    return shuffled_x, shuffled_y
+
+
+def slice_by_index(lst: list,
+                   indexes) -> list:
+    """Slice list by positional indexes.
+    Args:
+        lst: list to slice.
+        indexes: iterable of 0-based indexes of the list positions to return.
+    Returns:
+        a new list containing elements of lst on positions specified by indexes.
+    Examples:
+        >>> slice_by_index([], [])
+        []
+        >>> slice_by_index([], [0, 1])
+        []
+        >>> slice_by_index(['a', 'b', 'c'], [])
+        []
+        >>> slice_by_index(['a', 'b', 'c'], [0, 2])
+        ['a', 'c']
+        >>> slice_by_index(['a', 'b', 'c'], [0, 1])
+        ['a', 'b']
+        >>> slice_by_index(['a', 'b', 'c'], [1])
+        ['b']
+    """
+    if not lst or not indexes:
+        return []
+    slice_ = operator.itemgetter(*indexes)(lst)
+    if len(indexes) == 1:
+        return [slice_]
+    return list(slice_)
+
+
+def keep_only_duplicates(input_list: list) -> list:
+    """This function removes all unique values from input_list and keeps only the duplicates
+    Args:
+        input_list: list from which we want to remove unique values
+    Returns:
+        list_only_with_duplicates: output list that only contains the duplicates
+    Example:
+        >>> l = [1, 2, 2, 3, 3, 3, 4]
+        >>> out_list = keep_only_duplicates(l)
+        >>> out_list
+        [2,3]
+    """
+    counts = Counter(input_list)
+    list_only_with_duplicates = [id for id in counts if counts[id] > 1]
+
+    return list_only_with_duplicates
+
+
+def check_if_string_is_in_any_item_of_list(input_list: list,
+                                           match_string: str) -> bool:
+    """This function checks whether match_string is in any of the items of input_list;
+    if yes, it returns True, otherwise it returns False.
+    Args:
+       input_list: input list where we search for a match
+       match_string: string to match
+    Returns:
+        list_contains_match_string: True if list contains match_string; False otherwise
+    """
+    list_contains_match_string = bool([item for item in input_list if (match_string in item)])
+
+    return list_contains_match_string
+
+
+def all_elements_in_list_are_identical(input_list: list) -> bool:
+    """This function checks whether all the elements in input_list are identical. If they are, True is returned; otherwise, False is returned
+    Args:
+        input_list: input list for which we check that all elements are identical
+    Returns:
+        all_elements_are_identical: bool that indicates whether all elements are identical or not
+    """
+    all_elements_are_identical = all(x == input_list[0] for x in input_list)
+
+    return all_elements_are_identical
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_nifti_dicom.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_nifti_dicom.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,296 +1,296 @@
-import os
-import SimpleITK as sitk
-import nibabel as nib
-from typing import Tuple
-import numpy as np
-import pydicom
-from datetime import datetime
-
-
-def resample_volume(volume_path: str,
-                    new_spacing: list,
-                    out_path: str,
-                    interpolator: int = sitk.sitkLinear) -> Tuple[sitk.Image, nib.Nifti1Image, np.ndarray]:
-    """This function resamples the input volume to a specified voxel spacing
-    Args:
-        volume_path (str): input volume path
-        new_spacing (list): desired voxel spacing that we want
-        out_path (str): path where we temporarily save the resampled output volume
-        interpolator (int): interpolator that we want to use (e.g. 1= NearNeigh., 2=linear, ...)
-    Returns:
-        resampled_volume_sitk_obj: resampled volume as sitk object
-        resampled_volume_nii_obj: resampled volume as nib object
-        resampled_volume_nii: resampled volume as numpy array
-    """
-    volume = sitk.ReadImage(volume_path)  # read volume
-    original_size = volume.GetSize()  # extract size
-    original_spacing = volume.GetSpacing()  # extract spacing
-    new_size = [int(round(osz * ospc / nspc)) for osz, ospc, nspc in zip(original_size, original_spacing, new_spacing)]
-    resampled_volume_sitk_obj = sitk.Resample(volume, new_size, sitk.Transform(), interpolator,
-                                              volume.GetOrigin(), new_spacing, volume.GetDirection(), 0,
-                                              volume.GetPixelID())
-    sitk.WriteImage(resampled_volume_sitk_obj, out_path)  # write sitk volume object to disk
-    resampled_volume_nii_obj = nib.load(out_path)  # type: nib.Nifti1Image # load volume as nibabel object
-    resampled_volume_nii = np.asanyarray(resampled_volume_nii_obj.dataobj)  # type: np.ndarray # convert from nibabel object to np.array
-    os.remove(out_path)  # remove volume from disk to save space
-
-    return resampled_volume_sitk_obj, resampled_volume_nii_obj, resampled_volume_nii
-
-
-def remove_zeros_ijk_from_volume(input_volume: np.ndarray) -> np.ndarray:
-    """This function removes all the rows, columns and slices of the input volume that only contain zero values.
-    Args:
-        input_volume: volume from which we want to remove zeros
-    Returns:
-        cropped_volume: cropped volume (i.e. input volume with zeros removed)
-    """
-
-    def remove_zeros_one_coordinate(input_volume_: np.ndarray, range_spatial_dim: int, spatial_dim: int):
-        idxs_nonzero_slices = []  # will the contain the indexes of all the slices that have nonzero values
-        for idx in range(range_spatial_dim):  # loop over coordinate
-            if spatial_dim == 0:
-                one_slice = input_volume_[idx, :, :]
-            elif spatial_dim == 1:
-                one_slice = input_volume_[:, idx, :]
-            elif spatial_dim == 2:
-                one_slice = input_volume_[:, :, idx]
-            else:
-                raise ValueError(f"spatial_dim can only be 0, 1, or 2. Got {spatial_dim} instead")
-
-            if np.count_nonzero(one_slice) > 0:  # if the slice has some nonzero values
-                idxs_nonzero_slices.append(idx)  # save slice index
-
-        # retain only indexes with nonzero values from the two input volumes
-        if spatial_dim == 0:
-            cropped_volume_ = input_volume_[idxs_nonzero_slices, :, :]
-        elif spatial_dim == 1:
-            cropped_volume_ = input_volume_[:, idxs_nonzero_slices, :]
-        elif spatial_dim == 2:
-            cropped_volume_ = input_volume_[:, :, idxs_nonzero_slices]
-        else:
-            raise ValueError(f"spatial_dim can only be 0, 1, or 2. Got {spatial_dim} instead")
-
-        return cropped_volume_
-
-    assert len(input_volume.shape) == 3, "The input volume must be 3D"
-
-    # i coordinate
-    cropped_volume = remove_zeros_one_coordinate(input_volume, input_volume.shape[0], spatial_dim=0)
-    # j coordinate
-    cropped_volume = remove_zeros_one_coordinate(cropped_volume, input_volume.shape[1], spatial_dim=1)
-    # k coordinate
-    cropped_volume = remove_zeros_one_coordinate(cropped_volume, input_volume.shape[2], spatial_dim=2)
-
-    return cropped_volume
-
-
-def get_axes_orientations_with_nibabel(input_nifti_volume: nib.Nifti1Image) -> tuple:
-    """This function returns the axes orientations as a tuple
-    Args:
-        input_nifti_volume: the input volume for which we want the axes orientations
-    Returns:
-        orientations: the axes orientations
-    """
-    aff_mat = input_nifti_volume.affine  # type: np.ndarray # extract affine matrix
-    orientations = nib.aff2axcodes(aff_mat)
-
-    return orientations
-
-
-def get_nibabel_header(input_nifti_volume: nib.Nifti1Image,
-                       print_header: bool = False) -> nib.nifti1.Nifti1Header:
-    """This function returns the header of the nifti image/volume
-    Args:
-        input_nifti_volume: the input volume for which we want the header
-        print_header: whether to print the header or not; defaults to False
-    Returns:
-        header (nib.nifti1.Nifti1Header): the axes orientations
-    """
-    header = input_nifti_volume.header
-    if print_header:
-        print(header)
-
-    return header
-
-
-def read_dcm_series(dcm_dir: str) -> sitk.Image:
-    """This function reads a dicom series with SimpleITK
-    Args:
-        dcm_dir: directory where dicom files are stored
-    Returns:
-        volume_sitk: volume loaded as sitk.Image
-    """
-    reader = sitk.ImageSeriesReader()  # create reader
-    dicom_names = reader.GetGDCMSeriesFileNames(dcm_dir)  # read dicom series
-    reader.SetFileNames(dicom_names)
-
-    volume_sitk = reader.Execute()  # extract sitk.Image
-
-    return volume_sitk
-
-
-def get_sitk_volume_info(path_to_nii_or_dcm: str,
-                         print_info: bool = False) -> dict:
-    """This function prints basic info of the input volume
-    Args:
-        path_to_nii_or_dcm: path to volume that we want to explore
-        print_info: whether to print the volume info or no; defaults to False
-    Returns:
-        volume_info: it contains all the main volume information
-    """
-    if os.path.isdir(path_to_nii_or_dcm):  # if path_to_nii_or_dcm is a directory
-        volume_sitk = read_dcm_series(path_to_nii_or_dcm)
-    else:  # if instead path_to_nii_or_dcm is a file
-        volume_sitk = sitk.ReadImage(path_to_nii_or_dcm)  # read as sitk Image
-
-    volume_info = {"dimensions": volume_sitk.GetDimension(),
-                   "size": volume_sitk.GetSize(),
-                   "origin": volume_sitk.GetOrigin(),
-                   "spacing": volume_sitk.GetSpacing(),
-                   "direction": volume_sitk.GetDirection(),
-                   "nb_components_per_pixel": volume_sitk.GetNumberOfComponentsPerPixel(),
-                   "pixel_type": volume_sitk.GetPixelID(),
-                   "pixel_id_type_as_string": volume_sitk.GetPixelIDTypeAsString(),
-                   "pixel_id_value": volume_sitk.GetPixelIDValue()
-                   }
-
-    if print_info:
-        print(f"Dimensions: {volume_sitk.GetDimension()}")
-        print(f"Size: {volume_sitk.GetSize()}")
-        print(f"Origin: {volume_sitk.GetOrigin()}")
-        print(f"Spacing: {volume_sitk.GetSpacing()}")
-        print(f"Direction cosine matrix: {volume_sitk.GetDirection()}")
-        print(f"Nb. components per pixel {volume_sitk.GetNumberOfComponentsPerPixel()}")
-        print(f"Pixel type: {volume_sitk.GetPixelID()}")
-        print(f"Pixel ID type as string: {volume_sitk.GetPixelIDTypeAsString()}")
-        print(f"Pixel ID value: {volume_sitk.GetPixelIDValue()}")
-
-    return volume_info
-
-
-def re_orient_to_nib_closest_canonical(path_to_nii_volume: str,
-                                       sub: str,
-                                       ses: str,
-                                       volume_name: str,
-                                       orig_anat_dir: str) -> None:
-    """This function re-orients the input volume to the nibabel closest canonical orientation (i.e. RAS+)
-    Args:
-        path_to_nii_volume: path to volume that we want to re-oriented
-        sub: subject of interest
-        ses: session of interest
-        volume_name: name of volume to re-orient
-        orig_anat_dir: path to directory containing original TOF volume
-    """
-    # load mask volume
-    nii_obj = nib.load(path_to_nii_volume)  # load as nibabel object
-    nii_obj = nib.as_closest_canonical(nii_obj)  # re-orient to nibabel canonical axis orientation
-
-    # load original volume; we use it to enforce the same affine matrix for the re-oriented mask
-    original_volume_path = os.path.join(orig_anat_dir, f"{sub}_{ses}_{volume_name}.nii.gz")
-    original_volume_obj = nib.load(original_volume_path)  # load as nibabel object
-
-    # save re-oriented mask to disk, OVERWRITING the previous one
-    nib.Nifti1Image(nii_obj.dataobj, original_volume_obj.affine, nii_obj.header).to_filename(path_to_nii_volume)
-
-
-def change_dcm_tags_one_derived_image(ds: pydicom.dataset.FileDataset,
-                                      series_date: str,
-                                      invented_manufacturer: str,
-                                      invented_model_name: str,
-                                      series_time: str,
-                                      new_series_name: str,
-                                      new_protocol_name: str,
-                                      original_study_instance_uid: pydicom.uid.UID) -> pydicom.dataset.FileDataset:
-    """This function changes some dicom tags for the derived volume (following https://gdcm.sourceforge.net/wiki/index.php/Writing_DICOM but not only).
-    Args:
-        ds: pydicom object that contains the dicom tags
-        series_date: today's date (used as series' date)
-        invented_manufacturer: invented manufacturer name
-        invented_model_name: invented model name
-        series_time: generated time of series
-        new_series_name: name of new generated series
-        new_protocol_name: name of new generated protocol
-        original_study_instance_uid: study instance UID of the study; all series should have the same
-    Returns:
-        ds: same pydicom object, but with some modified tags
-    """
-    # below, we report all the dcm tags that will be changed
-
-    # 1) Media Storage SOP Instance UID (0002, 0003), it's a tag in the file meta information
-    generated_media_storage_sop_instance_uid = pydicom.uid.generate_uid()  # generate UID
-    ds.file_meta.MediaStorageSOPInstanceUID = generated_media_storage_sop_instance_uid
-
-    # 2) Image Type (0008, 0008) was already modified within MeVisLab
-
-    # 3) Instance creation date (0008, 0012)
-    if "InstanceCreationDate" in ds:
-        ds.InstanceCreationDate = series_date
-
-    # 4) Instance creation time (0008, 0013)
-    if "InstanceCreationTime" in ds:
-        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
-        ds.InstanceCreationTime = time_now
-
-    # 5) SOP Instance UID (0008, 0018)
-    if "SOPInstanceUID" in ds:
-        generated_sop_instance_uid = pydicom.uid.generate_uid()  # generate UID
-        ds.SOPInstanceUID = generated_sop_instance_uid
-
-    # 6) Acquisition Time (0008, 0032); generate a unique time for each dcm image
-    if "AcquisitionTime" in ds:
-        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
-        ds.AcquisitionTime = time_now
-
-    # 7) Series Time (0008, 0031); this needs to be the same for all dcm images in the series, so we define it outside of the function
-    if "SeriesTime" in ds:
-        ds.SeriesTime = series_time
-
-    # 8) Content Time (0008, 0032); this needs to be different for each dcm image
-    if "ContentTime" in ds:
-        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
-        ds.ContentTime = time_now
-
-    # 9) Manufacturer (0008, 0070)
-    if "Manufacturer" in ds:
-        ds.Manufacturer = invented_manufacturer
-
-    # 10) Series Description (0008, 103E) was already modified within MeVisLab
-
-    # 11) Manufacturer's model name (0008, 1090)
-    if "ManufacturerModelName" in ds:
-        ds.ManufacturerModelName = invented_model_name
-
-    # 12) Referenced Image Sequence (0008, 1140)
-    ref_img_seq = ds.ReferencedImageSequence
-    for idx, _ in enumerate(ref_img_seq):
-        if "ReferencedSOPInstanceUID" in ref_img_seq[idx]:
-            new_uid = pydicom.uid.generate_uid()  # generate UID
-            ref_img_seq[idx].ReferencedSOPInstanceUID = new_uid
-
-    # 13) Derivation description (0008, 2111)
-    ds.add_new(0x00082111, 'ST', 'Segmentation_Neuroinformatics_Paper')
-
-    # 14) Source image sequence (0008, 2112): don't know what to put and how to generate a valid SQ tag
-    # ds.add_new(0x00082112, 'SQ', '')
-
-    # 15) Sequence Name (0018, 0024)
-    if "SequenceName" in ds:
-        ds.SequenceName = new_series_name
-
-    # 16) Protocol Name (0018, 1030)
-    if "ProtocolName" in ds:
-        ds.ProtocolName = new_protocol_name
-
-    # 17) Study Instance UID (0020, 000D): this should be identical to the one of the original series cause the study is the same
-    if ds.StudyInstanceUID != original_study_instance_uid:  # if it's different
-        ds.StudyInstanceUID = original_study_instance_uid  # change it
-
-    # 18) Series Instance UID (0020, 000E) was already modified in MeVisLab
-
-    # 19) Series Number (0020, 0011) was already modified in MeVisLab
-
-    # 20) Image Comments (0020, 4000) was already modified in MeVisLab
-
-    # 21) Pixel Data (7FE0, 0010) was already modified in MeVisLab
-
-    return ds
+import os
+import SimpleITK as sitk
+import nibabel as nib
+from typing import Tuple
+import numpy as np
+import pydicom
+from datetime import datetime
+
+
+def resample_volume(volume_path: str,
+                    new_spacing: list,
+                    out_path: str,
+                    interpolator: int = sitk.sitkLinear) -> Tuple[sitk.Image, nib.Nifti1Image, np.ndarray]:
+    """This function resamples the input volume to a specified voxel spacing
+    Args:
+        volume_path (str): input volume path
+        new_spacing (list): desired voxel spacing that we want
+        out_path (str): path where we temporarily save the resampled output volume
+        interpolator (int): interpolator that we want to use (e.g. 1= NearNeigh., 2=linear, ...)
+    Returns:
+        resampled_volume_sitk_obj: resampled volume as sitk object
+        resampled_volume_nii_obj: resampled volume as nib object
+        resampled_volume_nii: resampled volume as numpy array
+    """
+    volume = sitk.ReadImage(volume_path)  # read volume
+    original_size = volume.GetSize()  # extract size
+    original_spacing = volume.GetSpacing()  # extract spacing
+    new_size = [int(round(osz * ospc / nspc)) for osz, ospc, nspc in zip(original_size, original_spacing, new_spacing)]
+    resampled_volume_sitk_obj = sitk.Resample(volume, new_size, sitk.Transform(), interpolator,
+                                              volume.GetOrigin(), new_spacing, volume.GetDirection(), 0,
+                                              volume.GetPixelID())
+    sitk.WriteImage(resampled_volume_sitk_obj, out_path)  # write sitk volume object to disk
+    resampled_volume_nii_obj = nib.load(out_path)  # type: nib.Nifti1Image # load volume as nibabel object
+    resampled_volume_nii = np.asanyarray(resampled_volume_nii_obj.dataobj)  # type: np.ndarray # convert from nibabel object to np.array
+    os.remove(out_path)  # remove volume from disk to save space
+
+    return resampled_volume_sitk_obj, resampled_volume_nii_obj, resampled_volume_nii
+
+
+def remove_zeros_ijk_from_volume(input_volume: np.ndarray) -> np.ndarray:
+    """This function removes all the rows, columns and slices of the input volume that only contain zero values.
+    Args:
+        input_volume: volume from which we want to remove zeros
+    Returns:
+        cropped_volume: cropped volume (i.e. input volume with zeros removed)
+    """
+
+    def remove_zeros_one_coordinate(input_volume_: np.ndarray, range_spatial_dim: int, spatial_dim: int):
+        idxs_nonzero_slices = []  # will the contain the indexes of all the slices that have nonzero values
+        for idx in range(range_spatial_dim):  # loop over coordinate
+            if spatial_dim == 0:
+                one_slice = input_volume_[idx, :, :]
+            elif spatial_dim == 1:
+                one_slice = input_volume_[:, idx, :]
+            elif spatial_dim == 2:
+                one_slice = input_volume_[:, :, idx]
+            else:
+                raise ValueError(f"spatial_dim can only be 0, 1, or 2. Got {spatial_dim} instead")
+
+            if np.count_nonzero(one_slice) > 0:  # if the slice has some nonzero values
+                idxs_nonzero_slices.append(idx)  # save slice index
+
+        # retain only indexes with nonzero values from the two input volumes
+        if spatial_dim == 0:
+            cropped_volume_ = input_volume_[idxs_nonzero_slices, :, :]
+        elif spatial_dim == 1:
+            cropped_volume_ = input_volume_[:, idxs_nonzero_slices, :]
+        elif spatial_dim == 2:
+            cropped_volume_ = input_volume_[:, :, idxs_nonzero_slices]
+        else:
+            raise ValueError(f"spatial_dim can only be 0, 1, or 2. Got {spatial_dim} instead")
+
+        return cropped_volume_
+
+    assert len(input_volume.shape) == 3, "The input volume must be 3D"
+
+    # i coordinate
+    cropped_volume = remove_zeros_one_coordinate(input_volume, input_volume.shape[0], spatial_dim=0)
+    # j coordinate
+    cropped_volume = remove_zeros_one_coordinate(cropped_volume, input_volume.shape[1], spatial_dim=1)
+    # k coordinate
+    cropped_volume = remove_zeros_one_coordinate(cropped_volume, input_volume.shape[2], spatial_dim=2)
+
+    return cropped_volume
+
+
+def get_axes_orientations_with_nibabel(input_nifti_volume: nib.Nifti1Image) -> tuple:
+    """This function returns the axes orientations as a tuple
+    Args:
+        input_nifti_volume: the input volume for which we want the axes orientations
+    Returns:
+        orientations: the axes orientations
+    """
+    aff_mat = input_nifti_volume.affine  # type: np.ndarray # extract affine matrix
+    orientations = nib.aff2axcodes(aff_mat)
+
+    return orientations
+
+
+def get_nibabel_header(input_nifti_volume: nib.Nifti1Image,
+                       print_header: bool = False) -> nib.nifti1.Nifti1Header:
+    """This function returns the header of the nifti image/volume
+    Args:
+        input_nifti_volume: the input volume for which we want the header
+        print_header: whether to print the header or not; defaults to False
+    Returns:
+        header (nib.nifti1.Nifti1Header): the axes orientations
+    """
+    header = input_nifti_volume.header
+    if print_header:
+        print(header)
+
+    return header
+
+
+def read_dcm_series(dcm_dir: str) -> sitk.Image:
+    """This function reads a dicom series with SimpleITK
+    Args:
+        dcm_dir: directory where dicom files are stored
+    Returns:
+        volume_sitk: volume loaded as sitk.Image
+    """
+    reader = sitk.ImageSeriesReader()  # create reader
+    dicom_names = reader.GetGDCMSeriesFileNames(dcm_dir)  # read dicom series
+    reader.SetFileNames(dicom_names)
+
+    volume_sitk = reader.Execute()  # extract sitk.Image
+
+    return volume_sitk
+
+
+def get_sitk_volume_info(path_to_nii_or_dcm: str,
+                         print_info: bool = False) -> dict:
+    """This function prints basic info of the input volume
+    Args:
+        path_to_nii_or_dcm: path to volume that we want to explore
+        print_info: whether to print the volume info or no; defaults to False
+    Returns:
+        volume_info: it contains all the main volume information
+    """
+    if os.path.isdir(path_to_nii_or_dcm):  # if path_to_nii_or_dcm is a directory
+        volume_sitk = read_dcm_series(path_to_nii_or_dcm)
+    else:  # if instead path_to_nii_or_dcm is a file
+        volume_sitk = sitk.ReadImage(path_to_nii_or_dcm)  # read as sitk Image
+
+    volume_info = {"dimensions": volume_sitk.GetDimension(),
+                   "size": volume_sitk.GetSize(),
+                   "origin": volume_sitk.GetOrigin(),
+                   "spacing": volume_sitk.GetSpacing(),
+                   "direction": volume_sitk.GetDirection(),
+                   "nb_components_per_pixel": volume_sitk.GetNumberOfComponentsPerPixel(),
+                   "pixel_type": volume_sitk.GetPixelID(),
+                   "pixel_id_type_as_string": volume_sitk.GetPixelIDTypeAsString(),
+                   "pixel_id_value": volume_sitk.GetPixelIDValue()
+                   }
+
+    if print_info:
+        print(f"Dimensions: {volume_sitk.GetDimension()}")
+        print(f"Size: {volume_sitk.GetSize()}")
+        print(f"Origin: {volume_sitk.GetOrigin()}")
+        print(f"Spacing: {volume_sitk.GetSpacing()}")
+        print(f"Direction cosine matrix: {volume_sitk.GetDirection()}")
+        print(f"Nb. components per pixel {volume_sitk.GetNumberOfComponentsPerPixel()}")
+        print(f"Pixel type: {volume_sitk.GetPixelID()}")
+        print(f"Pixel ID type as string: {volume_sitk.GetPixelIDTypeAsString()}")
+        print(f"Pixel ID value: {volume_sitk.GetPixelIDValue()}")
+
+    return volume_info
+
+
+def re_orient_to_nib_closest_canonical(path_to_nii_volume: str,
+                                       sub: str,
+                                       ses: str,
+                                       volume_name: str,
+                                       orig_anat_dir: str) -> None:
+    """This function re-orients the input volume to the nibabel closest canonical orientation (i.e. RAS+)
+    Args:
+        path_to_nii_volume: path to volume that we want to re-oriented
+        sub: subject of interest
+        ses: session of interest
+        volume_name: name of volume to re-orient
+        orig_anat_dir: path to directory containing original TOF volume
+    """
+    # load mask volume
+    nii_obj = nib.load(path_to_nii_volume)  # load as nibabel object
+    nii_obj = nib.as_closest_canonical(nii_obj)  # re-orient to nibabel canonical axis orientation
+
+    # load original volume; we use it to enforce the same affine matrix for the re-oriented mask
+    original_volume_path = os.path.join(orig_anat_dir, f"{sub}_{ses}_{volume_name}.nii.gz")
+    original_volume_obj = nib.load(original_volume_path)  # load as nibabel object
+
+    # save re-oriented mask to disk, OVERWRITING the previous one
+    nib.Nifti1Image(nii_obj.dataobj, original_volume_obj.affine, nii_obj.header).to_filename(path_to_nii_volume)
+
+
+def change_dcm_tags_one_derived_image(ds: pydicom.dataset.FileDataset,
+                                      series_date: str,
+                                      invented_manufacturer: str,
+                                      invented_model_name: str,
+                                      series_time: str,
+                                      new_series_name: str,
+                                      new_protocol_name: str,
+                                      original_study_instance_uid: pydicom.uid.UID) -> pydicom.dataset.FileDataset:
+    """This function changes some dicom tags for the derived volume (following https://gdcm.sourceforge.net/wiki/index.php/Writing_DICOM but not only).
+    Args:
+        ds: pydicom object that contains the dicom tags
+        series_date: today's date (used as series' date)
+        invented_manufacturer: invented manufacturer name
+        invented_model_name: invented model name
+        series_time: generated time of series
+        new_series_name: name of new generated series
+        new_protocol_name: name of new generated protocol
+        original_study_instance_uid: study instance UID of the study; all series should have the same
+    Returns:
+        ds: same pydicom object, but with some modified tags
+    """
+    # below, we report all the dcm tags that will be changed
+
+    # 1) Media Storage SOP Instance UID (0002, 0003), it's a tag in the file meta information
+    generated_media_storage_sop_instance_uid = pydicom.uid.generate_uid()  # generate UID
+    ds.file_meta.MediaStorageSOPInstanceUID = generated_media_storage_sop_instance_uid
+
+    # 2) Image Type (0008, 0008) was already modified within MeVisLab
+
+    # 3) Instance creation date (0008, 0012)
+    if "InstanceCreationDate" in ds:
+        ds.InstanceCreationDate = series_date
+
+    # 4) Instance creation time (0008, 0013)
+    if "InstanceCreationTime" in ds:
+        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
+        ds.InstanceCreationTime = time_now
+
+    # 5) SOP Instance UID (0008, 0018)
+    if "SOPInstanceUID" in ds:
+        generated_sop_instance_uid = pydicom.uid.generate_uid()  # generate UID
+        ds.SOPInstanceUID = generated_sop_instance_uid
+
+    # 6) Acquisition Time (0008, 0032); generate a unique time for each dcm image
+    if "AcquisitionTime" in ds:
+        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
+        ds.AcquisitionTime = time_now
+
+    # 7) Series Time (0008, 0031); this needs to be the same for all dcm images in the series, so we define it outside of the function
+    if "SeriesTime" in ds:
+        ds.SeriesTime = series_time
+
+    # 8) Content Time (0008, 0032); this needs to be different for each dcm image
+    if "ContentTime" in ds:
+        time_now = datetime.today().strftime('%H%M%S.%f')  # save time now
+        ds.ContentTime = time_now
+
+    # 9) Manufacturer (0008, 0070)
+    if "Manufacturer" in ds:
+        ds.Manufacturer = invented_manufacturer
+
+    # 10) Series Description (0008, 103E) was already modified within MeVisLab
+
+    # 11) Manufacturer's model name (0008, 1090)
+    if "ManufacturerModelName" in ds:
+        ds.ManufacturerModelName = invented_model_name
+
+    # 12) Referenced Image Sequence (0008, 1140)
+    ref_img_seq = ds.ReferencedImageSequence
+    for idx, _ in enumerate(ref_img_seq):
+        if "ReferencedSOPInstanceUID" in ref_img_seq[idx]:
+            new_uid = pydicom.uid.generate_uid()  # generate UID
+            ref_img_seq[idx].ReferencedSOPInstanceUID = new_uid
+
+    # 13) Derivation description (0008, 2111)
+    ds.add_new(0x00082111, 'ST', 'Segmentation_Neuroinformatics_Paper')
+
+    # 14) Source image sequence (0008, 2112): don't know what to put and how to generate a valid SQ tag
+    # ds.add_new(0x00082112, 'SQ', '')
+
+    # 15) Sequence Name (0018, 0024)
+    if "SequenceName" in ds:
+        ds.SequenceName = new_series_name
+
+    # 16) Protocol Name (0018, 1030)
+    if "ProtocolName" in ds:
+        ds.ProtocolName = new_protocol_name
+
+    # 17) Study Instance UID (0020, 000D): this should be identical to the one of the original series cause the study is the same
+    if ds.StudyInstanceUID != original_study_instance_uid:  # if it's different
+        ds.StudyInstanceUID = original_study_instance_uid  # change it
+
+    # 18) Series Instance UID (0020, 000E) was already modified in MeVisLab
+
+    # 19) Series Number (0020, 0011) was already modified in MeVisLab
+
+    # 20) Image Comments (0020, 4000) was already modified in MeVisLab
+
+    # 21) Pixel Data (7FE0, 0010) was already modified in MeVisLab
+
+    return ds
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_numpy.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_numpy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,131 +1,144 @@
-import numpy as np
-from typing import Any
-
-
-def find_most_frequent_value(input_array: np.ndarray) -> Any:
-    """This function finds the most common value in the input numpy array
-    Args:
-        input_array: input array for which we want to find the most frequent value
-    Returns:
-        most_frequent_value: most frequent value
-    """
-    values, counts = np.unique(input_array, return_counts=True)
-
-    idx = np.argmax(counts)
-    most_frequent_value = values[idx]  # extract the most frequent element
-
-    return most_frequent_value
-
-
-def has_nans(input_array: np.ndarray) -> bool:
-    """"This function checks whether the input array contains any nan.
-    If yes, it returns True, otherwise it returns False.
-    Args:
-        input_array: input array where we check for nans
-    Returns:
-        array_has_nan: True if input_array contains nans; False otherwise
-    """
-    array_sum = np.sum(input_array)
-    array_has_nan = np.isnan(array_sum)
-
-    return array_has_nan
-
-
-def is_binary(input_array: np.ndarray) -> bool:
-    """This function checks whether the input array is binary (i.e. contains only 0s and 1s).
-    If yes, it returns True, otherwise it returns False.
-    Args:
-        input_array: input array that we want to inspect
-    Returns:
-        array_is_binary: True if input_array is binary; False otherwise
-    """
-    array_is_binary = np.array_equal(input_array, input_array.astype(bool))
-
-    return array_is_binary
-
-
-def has_values_all_in_range(input_array: np.ndarray,
-                            low: int,
-                            high: int) -> bool:
-    """This function checks whether the input array has values that lie within the range (low, high).
-    If yes, it returns True, otherwise it returns False.
-    Args:
-        input_array: input array that we want to inspect
-        low: lower bound
-        high: upper bound
-    Returns:
-        array_is_withing_range: True if input_array has values in range (low, high); False otherwise
-    """
-    mask_array_bool = (input_array > low) & (input_array < high)
-
-    if False in mask_array_bool:  # if there is just one False value
-        array_is_withing_range = False
-    else:  # if instead all values are True
-        array_is_withing_range = True
-
-    return array_is_withing_range
-
-
-def pad_image_to_specified_shape(input_img: np.ndarray,
-                                 desired_x_dim: int,
-                                 desired_y_dim: int) -> np.ndarray:
-    """This function zero-pads input_img up to the specified shape (desired_x_dim, desired_y_dim)
-    Args:
-        input_img: input image that we want to pad
-        desired_x_dim: desired dimension 1
-        desired_y_dim: desired dimension 2
-    Returns:
-        padded_img: output padded image
-    """
-
-    assert len(input_img.shape) == 2, "This function is intended for 2D arrays"
-
-    # extract dims of input image
-    h = input_img.shape[0]
-    w = input_img.shape[1]
-
-    # extract padding width (before and after) for rows
-    a = (desired_x_dim - h) // 2
-    aa = desired_x_dim - a - h
-
-    # extract padding width (before and after) for cols
-    b = (desired_y_dim - w) // 2
-    bb = desired_y_dim - b - w
-
-    padded_img = np.pad(input_img, pad_width=((a, aa), (b, bb)), mode='constant', constant_values=0)
-
-    return padded_img
-
-
-def generate_binary_array_with_exact_proportion(array_len: int,
-                                                nb_zeros: int,
-                                                shuffle: bool = True):
-    """This function creates a 1D binary array with an exact proportion of 0s and 1s.
-    The array will contain exactly nb_zeros 0s, and (array_len - nb_zeros) 1s. By
-    default, the generated array is shuffled.
-    Args:
-        array_len: length of generated array
-        nb_zeros: number of 0s in the generated array (the rest will be 1s)
-        shuffle: whether to shuffle the generated array
-    Returns:
-        generated_binary_array: generated binary array
-    """
-    generated_binary_array = np.array([0] * nb_zeros + [1] * (array_len - nb_zeros))
-    if shuffle:
-        np.random.shuffle(generated_binary_array)
-
-    return generated_binary_array
-
-
-def mean_excluding_zeros(input_array: np.ndarray) -> float:
-    """This function computes the mean of non-zero values
-    Args:
-        input_array: input array for which we want to compute the mean
-    Returns:
-        mean_value_excluding_zeros: the arithmetic mean computed neglecting all zero elements
-    """
-    input_array = input_array.astype('float')  # cast array to float
-    input_array[input_array == 0] = np.nan  # set zero values to NaN
-    mean_value_excluding_zeros = np.nanmean(input_array)
-
-    return mean_value_excluding_zeros
+import numpy as np
+from typing import Any
+
+
+def find_most_frequent_value(input_array: np.ndarray) -> Any:
+    """This function finds the most common value in the input numpy array
+    Args:
+        input_array: input array for which we want to find the most frequent value
+    Returns:
+        most_frequent_value: most frequent value
+    """
+    values, counts = np.unique(input_array, return_counts=True)
+
+    idx = np.argmax(counts)
+    most_frequent_value = values[idx]  # extract the most frequent element
+
+    return most_frequent_value
+
+
+def has_nans(input_array: np.ndarray) -> bool:
+    """"This function checks whether the input array contains any nan.
+    If yes, it returns True, otherwise it returns False.
+    Args:
+        input_array: input array where we check for nans
+    Returns:
+        array_has_nan: True if input_array contains nans; False otherwise
+    """
+    array_sum = np.sum(input_array)
+    array_has_nan = np.isnan(array_sum)
+
+    return array_has_nan
+
+
+def is_binary(input_array: np.ndarray) -> bool:
+    """This function checks whether the input array is binary (i.e. contains only 0s and 1s).
+    If yes, it returns True, otherwise it returns False.
+    Args:
+        input_array: input array that we want to inspect
+    Returns:
+        array_is_binary: True if input_array is binary; False otherwise
+    """
+    array_is_binary = np.array_equal(input_array, input_array.astype(bool))
+
+    return array_is_binary
+
+
+def has_values_all_in_range(input_array: np.ndarray,
+                            low: int,
+                            high: int) -> bool:
+    """This function checks whether the input array has values that lie within the range (low, high).
+    If yes, it returns True, otherwise it returns False.
+    Args:
+        input_array: input array that we want to inspect
+        low: lower bound
+        high: upper bound
+    Returns:
+        array_is_withing_range: True if input_array has values in range (low, high); False otherwise
+    """
+    mask_array_bool = (input_array > low) & (input_array < high)
+
+    if False in mask_array_bool:  # if there is just one False value
+        array_is_withing_range = False
+    else:  # if instead all values are True
+        array_is_withing_range = True
+
+    return array_is_withing_range
+
+
+def pad_image_to_specified_shape(input_img: np.ndarray,
+                                 desired_x_dim: int,
+                                 desired_y_dim: int) -> np.ndarray:
+    """This function zero-pads input_img up to the specified shape (desired_x_dim, desired_y_dim)
+    Args:
+        input_img: input image that we want to pad
+        desired_x_dim: desired dimension 1
+        desired_y_dim: desired dimension 2
+    Returns:
+        padded_img: output padded image
+    """
+
+    assert len(input_img.shape) == 2, "This function is intended for 2D arrays"
+
+    # extract dims of input image
+    h = input_img.shape[0]
+    w = input_img.shape[1]
+
+    # extract padding width (before and after) for rows
+    a = (desired_x_dim - h) // 2
+    aa = desired_x_dim - a - h
+
+    # extract padding width (before and after) for cols
+    b = (desired_y_dim - w) // 2
+    bb = desired_y_dim - b - w
+
+    padded_img = np.pad(input_img, pad_width=((a, aa), (b, bb)), mode='constant', constant_values=0)
+
+    return padded_img
+
+
+def generate_binary_array_with_exact_proportion(array_len: int,
+                                                nb_zeros: int,
+                                                shuffle: bool = True):
+    """This function creates a 1D binary array with an exact proportion of 0s and 1s.
+    The array will contain exactly nb_zeros 0s, and (array_len - nb_zeros) 1s. By
+    default, the generated array is shuffled.
+    Args:
+        array_len: length of generated array
+        nb_zeros: number of 0s in the generated array (the rest will be 1s)
+        shuffle: whether to shuffle the generated array
+    Returns:
+        generated_binary_array: generated binary array
+    """
+    generated_binary_array = np.array([0] * nb_zeros + [1] * (array_len - nb_zeros))
+    if shuffle:
+        np.random.shuffle(generated_binary_array)
+
+    return generated_binary_array
+
+
+def mean_excluding_zeros(input_array: np.ndarray) -> float:
+    """This function computes the mean of non-zero values
+    Args:
+        input_array: input array for which we want to compute the mean
+    Returns:
+        mean_value_excluding_zeros: the arithmetic mean computed neglecting all zero elements
+    """
+    input_array = input_array.astype('float')  # cast array to float
+    input_array[input_array == 0] = np.nan  # set zero values to NaN
+    mean_value_excluding_zeros = np.nanmean(input_array)
+
+    return mean_value_excluding_zeros
+
+
+def is_empty(input_array: np.ndarray) -> bool:
+    """This function checks whether the input array is empty.
+    If yes, it returns True, otherwise it returns False.
+    Args:
+        input_array: input array that we want to inspect
+    Returns:
+        array_is_empty: True if input_array is empty; False otherwise
+    """
+    array_is_empty = input_array.size == 0
+
+    return array_is_empty
```

### Comparing `python3_utils_tdinoto-1.0.3/src/utils_tdinoto/utils_strings.py` & `python3_utils_tdinoto-1.0.4/src/utils_tdinoto/utils_strings.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,98 +1,98 @@
-from dateutil.parser import parse
-
-
-def is_date(input_string: str,
-            fuzzy: bool = False) -> bool:
-    """This function checks whether in the input string there is a date
-    Args:
-        input_string: string to check for date
-        fuzzy: ignore unknown tokens in string if True
-    Returns:
-         True: whether the string can be interpreted as a date.
-         False: otherwise
-    """
-    try:
-        parse(input_string, fuzzy=fuzzy)
-        return True
-
-    except ValueError:
-        return False
-
-
-def keep_only_digits(input_string: str) -> str:
-    """This function takes as input a string and returns the same string but only containing digits
-    Args:
-        input_string: the input string from which we want to remove non-digit characters
-    Returns:
-        output_string: the output string that only contains digit characters
-    """
-    numeric_filter = filter(str.isdigit, input_string)
-    output_string = "".join(numeric_filter)
-
-    return output_string
-
-
-def load_txt_file_as_string(path_txt_file: str) -> str:
-    """This function loads a txt file and returns its content as a string.
-    Args:
-        path_txt_file: path to txt file
-    Returns:
-        content: content of txt file
-    """
-    file = open(path_txt_file)
-    content = file.read()
-    file.close()
-
-    return content
-
-
-def add_leading_zeros(input_string: str,
-                      out_len: int) -> str:
-    """This function adds leading zeros to the input string. The output string will have length == out_len
-    Args:
-        input_string: the input string
-        out_len: length of output string with leading zeros
-    Returns:
-        out_string: the initial string but with leading zeros up to out_len characters
-    Example:
-        >>> s = "13"
-        >>> s_out = add_leading_zeros(input_string=s, out_len=4)
-        >>> s_out
-        '0013'
-    """
-    out_string = input_string.zfill(out_len)
-
-    return out_string
-
-
-def remove_leading_zeros(input_string: str) -> str:
-    """This function removes the leading zeros from input_string
-    Args:
-        input_string: the input string
-    Returns:
-        out_string: the input string without leading zeros
-    """
-    # use lstrip setting '0' as leading character, by default it would be space
-    out_string = input_string.lstrip('0')
-
-    return out_string
-
-
-def str2bool(v: str) -> bool:
-    """This function converts the input string into a boolean
-    Args:
-        v: input argument
-    Returns:
-        True: if the input argument is 'yes', 'true', 't', 'y', '1'
-        False: if the input argument is 'no', 'false', 'f', 'n', '0'
-    Raises:
-        ValueError: if the input argument is none of the above
-    """
-    if isinstance(v, bool):
-        return v
-    if v.lower() in ('yes', 'true', 't', 'y', '1'):
-        return True
-    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
-        return False
-    else:
-        raise ValueError('Boolean value expected.')
+from dateutil.parser import parse
+
+
+def is_date(input_string: str,
+            fuzzy: bool = False) -> bool:
+    """This function checks whether in the input string there is a date
+    Args:
+        input_string: string to check for date
+        fuzzy: ignore unknown tokens in string if True
+    Returns:
+         True: whether the string can be interpreted as a date.
+         False: otherwise
+    """
+    try:
+        parse(input_string, fuzzy=fuzzy)
+        return True
+
+    except ValueError:
+        return False
+
+
+def keep_only_digits(input_string: str) -> str:
+    """This function takes as input a string and returns the same string but only containing digits
+    Args:
+        input_string: the input string from which we want to remove non-digit characters
+    Returns:
+        output_string: the output string that only contains digit characters
+    """
+    numeric_filter = filter(str.isdigit, input_string)
+    output_string = "".join(numeric_filter)
+
+    return output_string
+
+
+def load_txt_file_as_string(path_txt_file: str) -> str:
+    """This function loads a txt file and returns its content as a string.
+    Args:
+        path_txt_file: path to txt file
+    Returns:
+        content: content of txt file
+    """
+    file = open(path_txt_file)
+    content = file.read()
+    file.close()
+
+    return content
+
+
+def add_leading_zeros(input_string: str,
+                      out_len: int) -> str:
+    """This function adds leading zeros to the input string. The output string will have length == out_len
+    Args:
+        input_string: the input string
+        out_len: length of output string with leading zeros
+    Returns:
+        out_string: the initial string but with leading zeros up to out_len characters
+    Example:
+        >>> s = "13"
+        >>> s_out = add_leading_zeros(input_string=s, out_len=4)
+        >>> s_out
+        '0013'
+    """
+    out_string = input_string.zfill(out_len)
+
+    return out_string
+
+
+def remove_leading_zeros(input_string: str) -> str:
+    """This function removes the leading zeros from input_string
+    Args:
+        input_string: the input string
+    Returns:
+        out_string: the input string without leading zeros
+    """
+    # use lstrip setting '0' as leading character, by default it would be space
+    out_string = input_string.lstrip('0')
+
+    return out_string
+
+
+def str2bool(v: str) -> bool:
+    """This function converts the input string into a boolean
+    Args:
+        v: input argument
+    Returns:
+        True: if the input argument is 'yes', 'true', 't', 'y', '1'
+        False: if the input argument is 'no', 'false', 'f', 'n', '0'
+    Raises:
+        ValueError: if the input argument is none of the above
+    """
+    if isinstance(v, bool):
+        return v
+    if v.lower() in ('yes', 'true', 't', 'y', '1'):
+        return True
+    elif v.lower() in ('no', 'false', 'f', 'n', '0'):
+        return False
+    else:
+        raise ValueError('Boolean value expected.')
```

