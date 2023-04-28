# Comparing `tmp/libquantum-1.5.0a1.tar.gz` & `tmp/libquantum-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.5.0a1.tar", last modified: Thu Apr 27 23:39:57 2023, max compression
+gzip compressed data, was "libquantum-1.5.1.tar", last modified: Fri Apr 28 19:53:35 2023, max compression
```

## Comparing `libquantum-1.5.0a1.tar` & `libquantum-1.5.1.tar`

### file list

```diff
@@ -1,33 +1,45 @@
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/
--rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.0a1/LICENSE
--rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)     2070 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/README.md
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.582776 libquantum-1.5.0a1/libquantum/
--rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.0a1/libquantum/__init__.py
--rw-r--r--   0 opq       (1000) opq       (1000)    20391 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/atoms.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/atoms_inverse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/blast_pulse.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/doppler.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/entropy.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/export.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.583776 libquantum-1.5.0a1/libquantum/plot_templates/
--rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.0a1/libquantum/plot_templates/__init__.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 opq       (1000) opq       (1000)    40958 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/scales.py
--rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.0a1/libquantum/spectra.py
--rw-r--r--   0 opq       (1000) opq       (1000)    12802 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/synthetics.py
--rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/libquantum/tfr_gate_pick.py
--rw-r--r--   0 opq       (1000) opq       (1000)    14988 2023-04-27 20:12:34.000000 libquantum-1.5.0a1/libquantum/utils.py
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.583776 libquantum-1.5.0a1/libquantum.egg-info/
--rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 opq       (1000) opq       (1000)      722 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      108 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/requires.txt
--rw-r--r--   0 opq       (1000) opq       (1000)       11 2023-04-27 23:39:57.000000 libquantum-1.5.0a1/libquantum.egg-info/top_level.txt
--rw-r--r--   0 opq       (1000) opq       (1000)      870 2023-04-27 23:39:41.000000 libquantum-1.5.0a1/pyproject.toml
--rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/setup.cfg
-drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:39:57.584776 libquantum-1.5.0a1/tests/
--rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.0a1/tests/test_quantum.py
--rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.0a1/tests/test_spectra.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.519199 libquantum-1.5.1/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.1/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-04-28 19:53:35.519199 libquantum-1.5.1/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2989 2023-04-28 19:47:14.000000 libquantum-1.5.1/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.517199 libquantum-1.5.1/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.1/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    22119 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/doppler.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     3104 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/dyadics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/export.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4322 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/gabor_box.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.518199 libquantum-1.5.1/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.1/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    41024 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    42082 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps_black.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     4092 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/rms_envelope.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.1/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    10324 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/stockwell_orig.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    33732 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_cwt.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19514 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_fft.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    11380 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_stx.py
+-rw-r--r--   0 opq       (1000) opq       (1000)     8438 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/styx_stx_loopy.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14611 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.1/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    19522 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.517199 libquantum-1.5.1/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    16374 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     1039 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       23 2023-04-28 19:53:35.000000 libquantum-1.5.1/libquantum.egg-info/top_level.txt
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.518199 libquantum-1.5.1/libquantum2/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum2/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    15727 2023-04-28 19:47:14.000000 libquantum-1.5.1/libquantum2/benchmark_signals.py
+-rw-r--r--   0 opq       (1000) opq       (1000)      864 2023-04-28 19:51:16.000000 libquantum-1.5.1/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-28 19:53:35.519199 libquantum-1.5.1/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-28 19:53:35.519199 libquantum-1.5.1/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.1/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.1/tests/test_spectra.py
```

### Comparing `libquantum-1.5.0a1/LICENSE` & `libquantum-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/PKG-INFO` & `libquantum-1.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.0a1
+Version: 1.5.1
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -244,23 +244,33 @@
 derived from large datasets, 
 Seism. Res. Lett.](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/91/3/1752/582897/Improved-Parametric-Models-for-Explosion-Pressure?redirectedFrom=fulltext)
 
 - [Kim, K, A. R. Rodgers, M. A. Garces, and S. C. Myers (2021).
 Empirical Acoustic Source Model for Chemical Explosions in Air,
 Bulletin of the Seismological Society of America](https://pubs.geoscienceworld.org/ssa/bssa/article-abstract/doi/10.1785/0120210030/600721/Empirical-Acoustic-Source-Model-for-Chemical?redirectedFrom=fulltext)
 
+Recommended reading in chronological order:
+- Gabor, D. Theory of Communication, Part 3. Electr. Eng. 1946, 93, 445–457.
+- Shannon, C.E. The Mathematical Theory of Communication; University of Illinois Press: Urbana, IL, USA, 1998; [1949 first ed].
+- Harris, F. J. On the Use of Windows for Harmonic Analysis with the Discrete Fourier Transform, Proceedings of the IEEE, 1978, 66 (1), 51-83.
+- Cohen, L. Time-Frequency Analysis, Prentice-Hall, NI 07458, 1995.
+- Stockwell, R. G., Mansina, L, and R. P. Lowe. Localization of the Complex Spectrum: The S Transform. Signal Processing, IEEE Transactions, 1996, 44 no. 4, 998-1001.
+- Mallat, S. A Wavelet Tour of Signal Processing: The Sparse Way, 3rd ed.; Academic Press: Cambridge, MA, USA, 2009 [1998 first ed].
+
+
+
 ### Installation
 
 ```shell script
 pip install libquantum
 ```
-More details in the [Installation guide](docs/libquantum/intallation.md).
+More details in the [Installation guide](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/intallation.md#libquantum-installation).
 
 ### Examples
-Full examples can be found in the [examples documentation](docs/libquantum/examples.md).
+Full examples can be found in the [examples documentation](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/examples.md#examples-using-libquantum).
 
 ### API Documentation
 Check the [API Documentation](https://redvoxinc.github.io/libquantum).
 
 ### Resources
 
 - Found an issue? Submit a [bug report](https://github.com/RedVoxInc/libquantum/issues).
```

### Comparing `libquantum-1.5.0a1/README.md` & `libquantum-1.5.1/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -29,23 +29,33 @@
 derived from large datasets, 
 Seism. Res. Lett.](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/91/3/1752/582897/Improved-Parametric-Models-for-Explosion-Pressure?redirectedFrom=fulltext)
 
 - [Kim, K, A. R. Rodgers, M. A. Garces, and S. C. Myers (2021).
 Empirical Acoustic Source Model for Chemical Explosions in Air,
 Bulletin of the Seismological Society of America](https://pubs.geoscienceworld.org/ssa/bssa/article-abstract/doi/10.1785/0120210030/600721/Empirical-Acoustic-Source-Model-for-Chemical?redirectedFrom=fulltext)
 
+Recommended reading in chronological order:
+- Gabor, D. Theory of Communication, Part 3. Electr. Eng. 1946, 93, 445–457.
+- Shannon, C.E. The Mathematical Theory of Communication; University of Illinois Press: Urbana, IL, USA, 1998; [1949 first ed].
+- Harris, F. J. On the Use of Windows for Harmonic Analysis with the Discrete Fourier Transform, Proceedings of the IEEE, 1978, 66 (1), 51-83.
+- Cohen, L. Time-Frequency Analysis, Prentice-Hall, NI 07458, 1995.
+- Stockwell, R. G., Mansina, L, and R. P. Lowe. Localization of the Complex Spectrum: The S Transform. Signal Processing, IEEE Transactions, 1996, 44 no. 4, 998-1001.
+- Mallat, S. A Wavelet Tour of Signal Processing: The Sparse Way, 3rd ed.; Academic Press: Cambridge, MA, USA, 2009 [1998 first ed].
+
+
+
 ### Installation
 
 ```shell script
 pip install libquantum
 ```
-More details in the [Installation guide](docs/libquantum/intallation.md).
+More details in the [Installation guide](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/intallation.md#libquantum-installation).
 
 ### Examples
-Full examples can be found in the [examples documentation](docs/libquantum/examples.md).
+Full examples can be found in the [examples documentation](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/examples.md#examples-using-libquantum).
 
 ### API Documentation
 Check the [API Documentation](https://redvoxinc.github.io/libquantum).
 
 ### Resources
 
 - Found an issue? Submit a [bug report](https://github.com/RedVoxInc/libquantum/issues).
```

### Comparing `libquantum-1.5.0a1/libquantum/atoms.py` & `libquantum-1.5.1/libquantum/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,23 +79,59 @@
 
     angular_frequency_center = 2 * np.pi * scale_frequency_center_hz/frequency_sample_rate_hz
     angular_frequency = 2 * np.pi * frequency_hz/frequency_sample_rate_hz
     offset_phase = angular_frequency * frequency_sample_rate_hz * offset_time_s
     angular_frequency_shifted = angular_frequency - angular_frequency_center
     frequency_shifted_hz = angular_frequency_shifted*frequency_sample_rate_hz/(2*np.pi)
 
-    spectrum_amplitude = np.sqrt(np.pi/p_complex)
+    # spectrum_amplitude = np.sqrt(np.pi/p_complex)
+    spectrum_amplitude = np.sqrt(p_complex/np.abs(p_complex))
     gauss_arg = 1./(4*p_complex)
-    spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted * scale_atom) ** 2)
+    # spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted * scale_atom) ** 2)
+    spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted**2))
     # Phase shift from time offset
     spectrum_gabor = spectrum_amplitude * spectrum_gauss * np.exp(-1j * offset_phase)
 
     return spectrum_gabor, frequency_shifted_hz
 
 
+def chirp_spectrum_centered(band_order_Nth: float,
+                            scale_frequency_center_hz: float,
+                            frequency_sample_rate_hz: float,
+                            index_shift: float = 0,
+                            scale_base: float = scales.Slice.G2) -> Tuple[Union[complex, float, np.ndarray], np.ndarray]:
+    """
+    Spectrum of quantum wavelet for specified band_order_Nth and arbitrary time duration
+
+    :param frequency_hz: frequency range below Nyquist
+    :param offset_time_s: time of wavelet centroid
+    :param band_order_Nth: Nth order of constant Q bands
+    :param scale_frequency_center_hz: band center frequency in Hz
+    :param frequency_sample_rate_hz: sample rate on Hz
+    :param index_shift: index of shift. Default is 0.0
+    :param scale_base: positive reference Base G > 1. Default is G2
+    :return: Fourier transform of the Gabor atom
+    """
+
+    # TODO: Generalize to two dictionaries
+    cycles_M, quality_factor_Q, gamma = \
+        chirp_MQG_from_N(band_order_Nth, index_shift, scale_base)
+    scale_atom = chirp_scale(cycles_M, scale_frequency_center_hz, frequency_sample_rate_hz)
+    p_complex = chirp_p_complex(scale_atom, gamma, index_shift)
+    angular_frequency_shifted = np.arange(-np.pi, np.pi, np.pi/2**7)
+    frequency_shifted_hz = angular_frequency_shifted*frequency_sample_rate_hz/(2*np.pi)
+
+    # spectrum_amplitude = np.sqrt(np.pi/p_complex)
+    spectrum_amplitude = np.sqrt(p_complex/np.abs(p_complex))
+    spectrum_gauss = np.exp(-(angular_frequency_shifted**2)/(4*p_complex))
+    spectrum_gabor = spectrum_amplitude * spectrum_gauss
+
+    return spectrum_gabor, frequency_shifted_hz
+
+
 def chirp_MQG_from_N(band_order_Nth: float,
                      index_shift: float = 0,
                      scale_base: float = scales.Slice.G2) -> Tuple[float, float, float]:
     """
     Compute the quality factor Q and multiplier M for a specified band order N
     N is THE quantization parameter for the binary constant Q wavelet filters
 
@@ -307,17 +343,15 @@
     wavelet_gabor, time_centered_s, amp_dict_0, amp_dict_1 = \
         chirp_complex(band_order_Nth,
                       time_s, offset_time_s, scale_frequency_center_hz, frequency_sample_rate_hz,
                       index_shift, scale_base)
 
     if dictionary_type == "norm":
         wavelet_chirp = amp_dict_0*wavelet_gabor
-    elif dictionary_type == "tone":
-        wavelet_chirp = np.sqrt(2)*amp_dict_1*wavelet_gabor
-    else:
+    else:  # spectrum
         wavelet_chirp = amp_dict_1*wavelet_gabor
 
     return wavelet_chirp, time_centered_s
 
 
 def cwt_chirp_complex(band_order_Nth: float,
                       sig_wf: np.ndarray,
```

### Comparing `libquantum-1.5.0a1/libquantum/atoms_inverse.py` & `libquantum-1.5.1/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/blast_pulse.py` & `libquantum-1.5.1/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/doppler.py` & `libquantum-1.5.1/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/entropy.py` & `libquantum-1.5.1/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/export.py` & `libquantum-1.5.1/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.1/libquantum/plot_templates/plot_time_frequency_reps.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,15 +224,15 @@
                        units_time: str = "s",
                        figure_title: str = "Time Domain Representation",
                        figure_title_show: bool = True,
                        label_panel_show: bool = False,
                        labels_panel_2: str = "(a)",
                        labels_panel_1: str = "(b)",
                        labels_panel_0: str = "(c)",
-                       labels_fontweight: str = None) -> None:
+                       labels_fontweight: str = None) -> plt.Figure:
     """
     Template for aligned time-series display
 
     :param redvox_id: name of station
     :param wf_panel_0_sig: array with signal waveform for top panel
     :param wf_panel_0_time: array with signal timestamps for top panel
     :param wf_panel_1_sig: array with signal waveform for middle panel
@@ -340,14 +340,16 @@
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
 
+    return fig
+
 
 def plot_wf_mesh_mesh_vert(redvox_id: str,
                            wf_panel_2_sig: np.ndarray,
                            wf_panel_2_time: np.ndarray,
                            mesh_time: np.ndarray,
                            mesh_frequency: np.ndarray,
                            mesh_panel_1_trf: np.ndarray,
@@ -370,15 +372,15 @@
                            mesh_colormap: str = "inferno",
                            units_time: str = "s",
                            units_frequency: str = "Hz",
                            wf_panel_2_units: str = "Norm",
                            mesh_panel_1_cbar_units: str = "bits",
                            mesh_panel_0_cbar_units: str = "bits",
                            figure_title: str = "Time-Frequency Representation",
-                           figure_title_show: bool = True) -> None:
+                           figure_title_show: bool = True) -> plt.Figure:
 
     """
     Plot 3 vertical panels - mesh (top panel), mesh (middle panel) and signal waveform (bottom panel)
 
     :param redvox_id: name of station
     :param wf_panel_2_sig: array with signal waveform for bottom panel
     :param wf_panel_2_time: array with signal timestamps for bottom panel
@@ -592,14 +594,16 @@
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
 
+    return fig
+
 
 def plot_wf_mesh_vert(redvox_id: str,
                       wf_panel_2_sig: np.ndarray,
                       wf_panel_2_time: np.ndarray,
                       mesh_time: np.ndarray,
                       mesh_frequency: np.ndarray,
                       mesh_panel_0_tfr: np.ndarray,
@@ -616,15 +620,15 @@
                       waveform_color: str = "midnightblue",
                       mesh_colormap: str = "inferno",
                       units_time: str = "s",
                       units_frequency: str = "Hz",
                       wf_panel_2_units: str = "Norm",
                       mesh_panel_0_cbar_units: str = "bits",
                       figure_title: str = "Time-Frequency Representation",
-                      figure_title_show: bool = True) -> None:
+                      figure_title_show: bool = True) -> plt.Figure:
     """
     Plot 2 vertical panels - mesh (top panel) and signal waveform (bottom panel)
 
     :param redvox_id: name of station
     :param wf_panel_2_sig: array with signal waveform for bottom panel
     :param wf_panel_2_time: array with signal timestamps for bottom panel
     :param mesh_time: array with mesh time
@@ -770,7 +774,9 @@
     wf_panel_2_cax.axis("off")
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
+
+    return fig
```

### Comparing `libquantum-1.5.0a1/libquantum/scales.py` & `libquantum-1.5.1/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/spectra.py` & `libquantum-1.5.1/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/synthetics.py` & `libquantum-1.5.1/libquantum/synthetics.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,53 @@
 import numpy as np
 import scipy.signal as signal
 from scipy.integrate import cumulative_trapezoid
 from typing import Optional, Tuple, Union
 from libquantum import utils, scales, atoms
 
 
+def gabor_loose_grain(band_order_Nth: float,
+                      number_points: int,
+                      scale_frequency_center_hz: float,
+                      frequency_sample_rate_hz: float,
+                      index_shift: float = 0,
+                      frequency_base_input: float = scales.Slice.G2) -> Tuple[np.ndarray, np.ndarray, float]:
+    """
+    Loose grain with tight Tukey wrap to ensure zero at edges
+
+    :param band_order_Nth: Nth order of constant Q bands
+    :param number_points: Number of points in the signal
+    :param scale_frequency_center_hz: center frequency fc in Hz
+    :param frequency_sample_rate_hz: sample rate of frequency in Hz
+    :param index_shift: index of shift for the Gabor chirp, default of zero
+    :param frequency_base_input: G2 or G3. Default is G2
+    :return: numpy array with Tukey grain
+    """
+
+    # Fundamental chirp parameters
+    cycles_M, quality_factor_Q, gamma = \
+        atoms.chirp_MQG_from_N(band_order_Nth, index_shift, frequency_base_input)
+    scale_atom = atoms.chirp_scale(cycles_M, scale_frequency_center_hz, frequency_sample_rate_hz)
+    p_complex = atoms.chirp_p_complex(scale_atom, gamma, index_shift)
+
+    # # Time from nominal duration
+    # grain_duration_s = cycles_M/scale_frequency_center_hz
+    # Time from number of points
+    time_s = np.arange(number_points)/frequency_sample_rate_hz
+    offset_time_s = np.max(time_s)/2.
+
+    xtime_shifted = atoms.chirp_time(time_s, offset_time_s, frequency_sample_rate_hz)
+    wavelet_gauss = np.exp(-p_complex * xtime_shifted**2)
+    wavelet_gabor = wavelet_gauss * np.exp(1j * cycles_M*xtime_shifted/scale_atom)
+    loose_grain_taper = utils.taper_tukey(wavelet_gabor, 0.1)
+    loose_grain = np.copy(wavelet_gabor) * loose_grain_taper
+
+    return loose_grain, time_s, scale_atom
+
+
 def gabor_tight_grain(band_order_Nth: float,
                       scale_frequency_center_hz: float,
                       frequency_sample_rate_hz: float,
                       index_shift: float = 0,
                       frequency_base_input: float = scales.Slice.G2) -> np.ndarray:
     """
     Gabor grain with tight Tukey wrap to ensure zero at edges
```

### Comparing `libquantum-1.5.0a1/libquantum/tfr_gate_pick.py` & `libquantum-1.5.1/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.5.0a1/libquantum/utils.py` & `libquantum-1.5.1/libquantum/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,34 +2,146 @@
 This module contains general utilities that can work with values containing nans.
 """
 
 from enum import Enum
 from typing import Tuple, Union
 
 import numpy as np
-from scipy import signal
+from scipy import interpolate, signal
 
 from scipy.integrate import cumulative_trapezoid
 from libquantum.scales import EPSILON
 from redvox.common import date_time_utils as dt
 
+""" Logical power of two flag """
+
+
+def is_power_of_two(n):
+    """ Returns not if not positive and a power of two """
+    return not (n > 0 and (n & (n - 1)))
+
+
+""" Time/Sample Duration Utils """
+
+
+def duration_points(sample_rate_hz: float, time_s: float) -> Tuple[int, int, int]:
+    """
+    Compute number of points
+    :param sample_rate_hz: sample rate in Hz
+    :param time_s: time scale, period or duration
+    :return: number of points, floor and ceiling of log2 of number of points
+    """
+    points_float: float = sample_rate_hz * time_s
+    points_int: int = int(points_float)
+    points_floor_log2: int = int(np.floor(np.log2(points_float)))
+    points_ceil_log2: int = int(np.ceil(np.log2(points_float)))
+
+    return points_int, points_floor_log2, points_ceil_log2
+
+
+def duration_ceil(sample_rate_hz: float, time_s: float) -> Tuple[int, int, float]:
+    """
+    Compute ceiling of the number of points, and convert to seconds
+    :param sample_rate_hz: sample rate in Hz
+    :param time_s: time scale, period or duration
+    :return: ceil of log 2 of number of points, power of two number of points, corresponding time in s
+    """
+    points_float: float = sample_rate_hz * time_s
+    points_ceil_log2: int = int(np.ceil(np.log2(points_float)))
+    points_ceil_pow2: int = 2**points_ceil_log2
+    time_ceil_pow2_s: float = points_ceil_pow2 / sample_rate_hz
+
+    return points_ceil_log2, points_ceil_pow2, time_ceil_pow2_s
+
+
+def duration_floor(sample_rate_hz: float, time_s: float) -> Tuple[int, int, float]:
+    """
+    Compute floor of the number of points, and convert to seconds
+    :param sample_rate_hz: sample rate in Hz
+    :param time_s: time scale, period or duration
+    :return: floor of log 2 of number of points, power of two number of points, corresponding time in s
+    """
+    points_float: float = sample_rate_hz * time_s
+    points_floor_log2: int = int(np.floor(np.log2(points_float)))
+    points_floor_pow2: int = 2**points_floor_log2
+    time_floor_pow2_s: float = points_floor_pow2 / sample_rate_hz
+
+    return points_floor_log2, points_floor_pow2, time_floor_pow2_s
+
+
+""" Sampling Utils """
+
+
+def resample_uneven_signal(sig_wf: np.ndarray,
+                           sig_epoch_s: np.ndarray,
+                           sample_rate_new_hz: float = None):
+    """
+
+    :param sig_wf:
+    :param sig_epoch_s:
+    :param sample_rate_new_hz:
+    :return:
+    """
+
+    if sample_rate_new_hz is None:
+        interval_from_epoch_s = np.mean(np.diff(sig_epoch_s))
+        # Round up
+        sample_rate_new_hz = np.ceil(1/interval_from_epoch_s)
+
+    interval_s = 1/sample_rate_new_hz
+    sig_new_epoch_s = np.arange(sig_epoch_s[0], sig_epoch_s[-1], interval_s)
+    f = interpolate.interp1d(sig_epoch_s, sig_wf)
+    sig_new_wf = f(sig_new_epoch_s)
+    return sig_new_wf, sig_new_epoch_s
+
+
+def upsample_fourier(sig_wf: np.ndarray,
+                     sig_sample_rate_hz: float,
+                     new_sample_rate_hz: float = 8000.) -> np.ndarray:
+    """
+    Upsample the Fourier way.
+
+    :param sig_wf: input signal waveform, reasonably well preprocessed
+    :param sig_sample_rate_hz: signal sample rate
+    :param new_sample_rate_hz: resampling sample rate
+    :return: resampled signal
+    """
+    sig_len = len(sig_wf)
+    new_len = int(sig_len * new_sample_rate_hz / sig_sample_rate_hz)
+    sig_resampled = signal.resample(x=sig_wf, num=new_len)
+    return sig_resampled
+
 
 def taper_tukey(sig_wf_or_time: np.ndarray,
                 fraction_cosine: float) -> np.ndarray:
     """
     Constructs a symmetric Tukey window with the same dimensions as a time or signal numpy array.
     fraction_cosine = 0 is a rectangular window, 1 is a Hann window
 
     :param sig_wf_or_time: input signal or time
     :param fraction_cosine: fraction of the window inside the cosine tapered window, shared between the head and tail
     :return: tukey taper window amplitude
     """
     return signal.windows.tukey(M=np.size(sig_wf_or_time), alpha=fraction_cosine, sym=True)
 
 
+# def taper_tukey_array(number_signals: int,
+#                       number_samples: int,
+#                       fraction_cosine: float = 0.1) -> np.ndarray:
+#     """
+#     Construct a teper matrix
+#     :param number_signals:
+#     :param number_samples:
+#     :param fraction_cosine:
+#     :return:
+#     """
+#     tukey_nsamples = signal.windows.tukey(M=number_samples, alpha=fraction_cosine, sym=True)
+#     tukey_array = just_tile(tukey_nsamples)
+
+
 def datetime_now_epoch_s() -> float:
     """
     Returns the invocation Unix time in seconds
 
     :return: The current epoch timestamp as seconds since the epoch UTC
     """
     return dt.datetime_to_epoch_seconds_utc(dt.now())
@@ -448,7 +560,26 @@
         raise TypeError('Cannot handle an array of shape {}.'.format(str(d1.shape)))
 
     if d1_matrix.shape == d2.shape:
         d1_x_d2 = d1_matrix * d2
     else:
         raise TypeError('Cannot handle an array of shape {}.'.format(str(d1.shape)))
     return d1_x_d2
+
+
+def decimate_array(sig_wf: np.array,
+                   downsampling_factor: int) -> np.ndarray:
+    """
+    Decimate data and timestamps for an individual station
+    All signals MUST have the same sample rate
+    :param sig_wf: signal waveform
+    :param downsampling_factor: the downsampling factor
+    :param filter_order: the order of the filter
+    :return: np.array decimated data
+    """
+    # decimate signal data
+    decimated_data = signal.decimate(x=sig_wf,
+                                    q=downsampling_factor,
+                                    axis=1,
+                                    zero_phase=True)
+
+    return decimated_data
```

### Comparing `libquantum-1.5.0a1/libquantum.egg-info/PKG-INFO` & `libquantum-1.5.1/libquantum.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libquantum
-Version: 1.5.0a1
+Version: 1.5.1
 Summary: Library for implementing standardized time-frequency representations.
 Author-email: "RedVox, Inc" <support@redvox.io>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -244,23 +244,33 @@
 derived from large datasets, 
 Seism. Res. Lett.](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/91/3/1752/582897/Improved-Parametric-Models-for-Explosion-Pressure?redirectedFrom=fulltext)
 
 - [Kim, K, A. R. Rodgers, M. A. Garces, and S. C. Myers (2021).
 Empirical Acoustic Source Model for Chemical Explosions in Air,
 Bulletin of the Seismological Society of America](https://pubs.geoscienceworld.org/ssa/bssa/article-abstract/doi/10.1785/0120210030/600721/Empirical-Acoustic-Source-Model-for-Chemical?redirectedFrom=fulltext)
 
+Recommended reading in chronological order:
+- Gabor, D. Theory of Communication, Part 3. Electr. Eng. 1946, 93, 445–457.
+- Shannon, C.E. The Mathematical Theory of Communication; University of Illinois Press: Urbana, IL, USA, 1998; [1949 first ed].
+- Harris, F. J. On the Use of Windows for Harmonic Analysis with the Discrete Fourier Transform, Proceedings of the IEEE, 1978, 66 (1), 51-83.
+- Cohen, L. Time-Frequency Analysis, Prentice-Hall, NI 07458, 1995.
+- Stockwell, R. G., Mansina, L, and R. P. Lowe. Localization of the Complex Spectrum: The S Transform. Signal Processing, IEEE Transactions, 1996, 44 no. 4, 998-1001.
+- Mallat, S. A Wavelet Tour of Signal Processing: The Sparse Way, 3rd ed.; Academic Press: Cambridge, MA, USA, 2009 [1998 first ed].
+
+
+
 ### Installation
 
 ```shell script
 pip install libquantum
 ```
-More details in the [Installation guide](docs/libquantum/intallation.md).
+More details in the [Installation guide](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/intallation.md#libquantum-installation).
 
 ### Examples
-Full examples can be found in the [examples documentation](docs/libquantum/examples.md).
+Full examples can be found in the [examples documentation](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/examples.md#examples-using-libquantum).
 
 ### API Documentation
 Check the [API Documentation](https://redvoxinc.github.io/libquantum).
 
 ### Resources
 
 - Found an issue? Submit a [bug report](https://github.com/RedVoxInc/libquantum/issues).
```

### Comparing `libquantum-1.5.0a1/libquantum.egg-info/SOURCES.txt` & `libquantum-1.5.1/libquantum.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -2,25 +2,36 @@
 README.md
 pyproject.toml
 libquantum/__init__.py
 libquantum/atoms.py
 libquantum/atoms_inverse.py
 libquantum/blast_pulse.py
 libquantum/doppler.py
+libquantum/dyadics.py
 libquantum/entropy.py
 libquantum/export.py
+libquantum/gabor_box.py
+libquantum/rms_envelope.py
 libquantum/scales.py
 libquantum/spectra.py
+libquantum/stockwell_orig.py
+libquantum/styx_cwt.py
+libquantum/styx_fft.py
+libquantum/styx_stx.py
+libquantum/styx_stx_loopy.py
 libquantum/synthetics.py
 libquantum/tfr_gate_pick.py
 libquantum/utils.py
 libquantum.egg-info/PKG-INFO
 libquantum.egg-info/SOURCES.txt
 libquantum.egg-info/dependency_links.txt
 libquantum.egg-info/requires.txt
 libquantum.egg-info/top_level.txt
 libquantum/plot_templates/__init__.py
 libquantum/plot_templates/plot_geo_scatter_2d_3d.py
 libquantum/plot_templates/plot_time_frequency_picks.py
 libquantum/plot_templates/plot_time_frequency_reps.py
+libquantum/plot_templates/plot_time_frequency_reps_black.py
+libquantum2/__init__.py
+libquantum2/benchmark_signals.py
 tests/test_quantum.py
 tests/test_spectra.py
```

### Comparing `libquantum-1.5.0a1/pyproject.toml` & `libquantum-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # See:
 # - https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 # - https://packaging.python.org/en/latest/specifications/declaring-project-metadata/
 
 [project]
 name = "libquantum"
-version = "1.5.0a1"
+version = "1.5.1"
 authors = [
     { name = "RedVox, Inc", email = "support@redvox.io" }
 ]
 description = "Library for implementing standardized time-frequency representations."
 readme = "README.md"
 requires-python = ">=3.8,<3.11"
 license = { file = "LICENSE" }
 
 dependencies = [
     "librosa==0.10.0.post2",
-    "redvox==3.4.0a3",
-    "libwwz==1.3.0a1",
+    "redvox==3.4.0",
+    "libwwz==1.3.0",
     "redvox-base[matplotlib,numpy,pandas,scipy]==2023.4.27"
 ]
 
 [project.urls]
 homepage = "https://github.com/RedVoxInc/libquantum"
 PyPI = "https://pypi.org/project/libquantum/"
```

### Comparing `libquantum-1.5.0a1/tests/test_spectra.py` & `libquantum-1.5.1/tests/test_spectra.py`

 * *Files identical despite different names*

