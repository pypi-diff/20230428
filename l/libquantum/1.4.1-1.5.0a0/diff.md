# Comparing `tmp/libquantum-1.4.1.tar.gz` & `tmp/libquantum-1.5.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libquantum-1.4.1.tar", last modified: Thu Sep  1 01:32:01 2022, max compression
+gzip compressed data, was "libquantum-1.5.0a0.tar", last modified: Thu Apr 27 23:23:45 2023, max compression
```

## Comparing `libquantum-1.4.1.tar` & `libquantum-1.5.0a0.tar`

### file list

```diff
@@ -1,39 +1,33 @@
-drwxr-xr-x   0 meritxell   (502) staff       (20)        0 2022-09-01 01:32:01.552394 libquantum-1.4.1/
--rw-r--r--   0 meritxell   (502) staff       (20)    11359 2021-05-26 21:58:53.000000 libquantum-1.4.1/LICENSE
--rw-r--r--   0 meritxell   (502) staff       (20)     3344 2022-09-01 01:32:01.551997 libquantum-1.4.1/PKG-INFO
--rw-r--r--   0 meritxell   (502) staff       (20)     2989 2022-09-01 01:24:19.000000 libquantum-1.4.1/README.md
-drwxr-xr-x   0 meritxell   (502) staff       (20)        0 2022-09-01 01:32:01.546952 libquantum-1.4.1/libquantum/
--rw-r--r--   0 meritxell   (502) staff       (20)        0 2021-05-26 21:58:53.000000 libquantum-1.4.1/libquantum/__init__.py
--rw-r--r--   0 meritxell   (502) staff       (20)    22119 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/atoms.py
--rw-r--r--   0 meritxell   (502) staff       (20)     4531 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/atoms_inverse.py
--rw-r--r--   0 meritxell   (502) staff       (20)    11698 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/blast_pulse.py
--rw-r--r--   0 meritxell   (502) staff       (20)    18779 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/doppler.py
--rw-r--r--   0 meritxell   (502) staff       (20)     3104 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/dyadics.py
--rw-r--r--   0 meritxell   (502) staff       (20)     5000 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/entropy.py
--rw-r--r--   0 meritxell   (502) staff       (20)     3206 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/export.py
--rw-r--r--   0 meritxell   (502) staff       (20)     4322 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/gabor_box.py
-drwxr-xr-x   0 meritxell   (502) staff       (20)        0 2022-09-01 01:32:01.551285 libquantum-1.4.1/libquantum/plot_templates/
--rw-r--r--   0 meritxell   (502) staff       (20)        0 2021-05-26 21:58:53.000000 libquantum-1.4.1/libquantum/plot_templates/__init__.py
--rw-r--r--   0 meritxell   (502) staff       (20)     8402 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
--rw-r--r--   0 meritxell   (502) staff       (20)    30812 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/plot_templates/plot_time_frequency_picks.py
--rw-r--r--   0 meritxell   (502) staff       (20)    41024 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/plot_templates/plot_time_frequency_reps.py
--rw-r--r--   0 meritxell   (502) staff       (20)    42082 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/plot_templates/plot_time_frequency_reps_black.py
--rw-r--r--   0 meritxell   (502) staff       (20)     4092 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/rms_envelope.py
--rw-r--r--   0 meritxell   (502) staff       (20)    23623 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/scales.py
--rw-r--r--   0 meritxell   (502) staff       (20)    16614 2022-09-01 01:27:59.000000 libquantum-1.4.1/libquantum/spectra.py
--rw-r--r--   0 meritxell   (502) staff       (20)    10324 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/stockwell_orig.py
--rw-r--r--   0 meritxell   (502) staff       (20)    33732 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/styx_cwt.py
--rw-r--r--   0 meritxell   (502) staff       (20)    19514 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/styx_fft.py
--rw-r--r--   0 meritxell   (502) staff       (20)    11380 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/styx_stx.py
--rw-r--r--   0 meritxell   (502) staff       (20)     8438 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/styx_stx_loopy.py
--rw-r--r--   0 meritxell   (502) staff       (20)    14611 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/synthetics.py
--rw-r--r--   0 meritxell   (502) staff       (20)     6093 2021-12-09 20:47:51.000000 libquantum-1.4.1/libquantum/tfr_gate_pick.py
--rw-r--r--   0 meritxell   (502) staff       (20)    19522 2022-09-01 01:24:19.000000 libquantum-1.4.1/libquantum/utils.py
-drwxr-xr-x   0 meritxell   (502) staff       (20)        0 2022-09-01 01:32:01.548939 libquantum-1.4.1/libquantum.egg-info/
--rw-r--r--   0 meritxell   (502) staff       (20)     3344 2022-09-01 01:32:01.000000 libquantum-1.4.1/libquantum.egg-info/PKG-INFO
--rw-r--r--   0 meritxell   (502) staff       (20)      932 2022-09-01 01:32:01.000000 libquantum-1.4.1/libquantum.egg-info/SOURCES.txt
--rw-r--r--   0 meritxell   (502) staff       (20)        1 2022-09-01 01:32:01.000000 libquantum-1.4.1/libquantum.egg-info/dependency_links.txt
--rw-r--r--   0 meritxell   (502) staff       (20)       88 2022-09-01 01:32:01.000000 libquantum-1.4.1/libquantum.egg-info/requires.txt
--rw-r--r--   0 meritxell   (502) staff       (20)       11 2022-09-01 01:32:01.000000 libquantum-1.4.1/libquantum.egg-info/top_level.txt
--rw-r--r--   0 meritxell   (502) staff       (20)       38 2022-09-01 01:32:01.552528 libquantum-1.4.1/setup.cfg
--rw-r--r--   0 meritxell   (502) staff       (20)      887 2022-09-01 01:27:12.000000 libquantum-1.4.1/setup.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11359 2021-02-24 02:24:24.000000 libquantum-1.5.0a0/LICENSE
+-rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)     2070 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/README.md
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.517237 libquantum-1.5.0a0/libquantum/
+-rw-r--r--   0 opq       (1000) opq       (1000)        0 2021-02-23 22:07:43.000000 libquantum-1.5.0a0/libquantum/__init__.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    20391 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/atoms.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     4531 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/atoms_inverse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    11698 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/blast_pulse.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    18779 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/doppler.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     5000 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/entropy.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     3206 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/export.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/libquantum/plot_templates/
+-rw-rw-r--   0 opq       (1000) opq       (1000)        0 2021-02-24 02:59:56.000000 libquantum-1.5.0a0/libquantum/plot_templates/__init__.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     8402 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_geo_scatter_2d_3d.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    30812 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_picks.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    40958 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_reps.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)    23623 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/scales.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    16614 2023-04-26 00:10:15.000000 libquantum-1.5.0a0/libquantum/spectra.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    12802 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/synthetics.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)     6093 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/libquantum/tfr_gate_pick.py
+-rw-r--r--   0 opq       (1000) opq       (1000)    14988 2023-04-27 20:12:34.000000 libquantum-1.5.0a0/libquantum/utils.py
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/libquantum.egg-info/
+-rw-r--r--   0 opq       (1000) opq       (1000)    15457 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/PKG-INFO
+-rw-r--r--   0 opq       (1000) opq       (1000)      722 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/SOURCES.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)        1 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/dependency_links.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      104 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/requires.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)       11 2023-04-27 23:23:45.000000 libquantum-1.5.0a0/libquantum.egg-info/top_level.txt
+-rw-r--r--   0 opq       (1000) opq       (1000)      866 2023-04-27 23:22:39.000000 libquantum-1.5.0a0/pyproject.toml
+-rw-r--r--   0 opq       (1000) opq       (1000)       38 2023-04-27 23:23:45.519237 libquantum-1.5.0a0/setup.cfg
+drwxr-xr-x   0 opq       (1000) opq       (1000)        0 2023-04-27 23:23:45.518237 libquantum-1.5.0a0/tests/
+-rw-rw-r--   0 opq       (1000) opq       (1000)      223 2021-02-24 02:24:24.000000 libquantum-1.5.0a0/tests/test_quantum.py
+-rw-rw-r--   0 opq       (1000) opq       (1000)      966 2022-07-07 20:05:44.000000 libquantum-1.5.0a0/tests/test_spectra.py
```

### Comparing `libquantum-1.4.1/LICENSE` & `libquantum-1.5.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/README.md` & `libquantum-1.5.0a0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -29,33 +29,23 @@
 derived from large datasets, 
 Seism. Res. Lett.](https://pubs.geoscienceworld.org/ssa/srl/article-abstract/91/3/1752/582897/Improved-Parametric-Models-for-Explosion-Pressure?redirectedFrom=fulltext)
 
 - [Kim, K, A. R. Rodgers, M. A. Garces, and S. C. Myers (2021).
 Empirical Acoustic Source Model for Chemical Explosions in Air,
 Bulletin of the Seismological Society of America](https://pubs.geoscienceworld.org/ssa/bssa/article-abstract/doi/10.1785/0120210030/600721/Empirical-Acoustic-Source-Model-for-Chemical?redirectedFrom=fulltext)
 
-Recommended reading in chronological order:
-- Gabor, D. Theory of Communication, Part 3. Electr. Eng. 1946, 93, 445–457.
-- Shannon, C.E. The Mathematical Theory of Communication; University of Illinois Press: Urbana, IL, USA, 1998; [1949 first ed].
-- Harris, F. J. On the Use of Windows for Harmonic Analysis with the Discrete Fourier Transform, Proceedings of the IEEE, 1978, 66 (1), 51-83.
-- Cohen, L. Time-Frequency Analysis, Prentice-Hall, NI 07458, 1995.
-- Stockwell, R. G., Mansina, L, and R. P. Lowe. Localization of the Complex Spectrum: The S Transform. Signal Processing, IEEE Transactions, 1996, 44 no. 4, 998-1001.
-- Mallat, S. A Wavelet Tour of Signal Processing: The Sparse Way, 3rd ed.; Academic Press: Cambridge, MA, USA, 2009 [1998 first ed].
-
-
-
 ### Installation
 
 ```shell script
 pip install libquantum
 ```
-More details in the [Installation guide](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/intallation.md#libquantum-installation).
+More details in the [Installation guide](docs/libquantum/intallation.md).
 
 ### Examples
-Full examples can be found in the [examples documentation](https://github.com/RedVoxInc/libquantum/blob/master/docs/libquantum/examples.md#examples-using-libquantum).
+Full examples can be found in the [examples documentation](docs/libquantum/examples.md).
 
 ### API Documentation
 Check the [API Documentation](https://redvoxinc.github.io/libquantum).
 
 ### Resources
 
 - Found an issue? Submit a [bug report](https://github.com/RedVoxInc/libquantum/issues).
```

### Comparing `libquantum-1.4.1/libquantum/atoms.py` & `libquantum-1.5.0a0/libquantum/atoms.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,59 +79,23 @@
 
     angular_frequency_center = 2 * np.pi * scale_frequency_center_hz/frequency_sample_rate_hz
     angular_frequency = 2 * np.pi * frequency_hz/frequency_sample_rate_hz
     offset_phase = angular_frequency * frequency_sample_rate_hz * offset_time_s
     angular_frequency_shifted = angular_frequency - angular_frequency_center
     frequency_shifted_hz = angular_frequency_shifted*frequency_sample_rate_hz/(2*np.pi)
 
-    # spectrum_amplitude = np.sqrt(np.pi/p_complex)
-    spectrum_amplitude = np.sqrt(p_complex/np.abs(p_complex))
+    spectrum_amplitude = np.sqrt(np.pi/p_complex)
     gauss_arg = 1./(4*p_complex)
-    # spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted * scale_atom) ** 2)
-    spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted**2))
+    spectrum_gauss = np.exp(-gauss_arg * (angular_frequency_shifted * scale_atom) ** 2)
     # Phase shift from time offset
     spectrum_gabor = spectrum_amplitude * spectrum_gauss * np.exp(-1j * offset_phase)
 
     return spectrum_gabor, frequency_shifted_hz
 
 
-def chirp_spectrum_centered(band_order_Nth: float,
-                            scale_frequency_center_hz: float,
-                            frequency_sample_rate_hz: float,
-                            index_shift: float = 0,
-                            scale_base: float = scales.Slice.G2) -> Tuple[Union[complex, float, np.ndarray], np.ndarray]:
-    """
-    Spectrum of quantum wavelet for specified band_order_Nth and arbitrary time duration
-
-    :param frequency_hz: frequency range below Nyquist
-    :param offset_time_s: time of wavelet centroid
-    :param band_order_Nth: Nth order of constant Q bands
-    :param scale_frequency_center_hz: band center frequency in Hz
-    :param frequency_sample_rate_hz: sample rate on Hz
-    :param index_shift: index of shift. Default is 0.0
-    :param scale_base: positive reference Base G > 1. Default is G2
-    :return: Fourier transform of the Gabor atom
-    """
-
-    # TODO: Generalize to two dictionaries
-    cycles_M, quality_factor_Q, gamma = \
-        chirp_MQG_from_N(band_order_Nth, index_shift, scale_base)
-    scale_atom = chirp_scale(cycles_M, scale_frequency_center_hz, frequency_sample_rate_hz)
-    p_complex = chirp_p_complex(scale_atom, gamma, index_shift)
-    angular_frequency_shifted = np.arange(-np.pi, np.pi, np.pi/2**7)
-    frequency_shifted_hz = angular_frequency_shifted*frequency_sample_rate_hz/(2*np.pi)
-
-    # spectrum_amplitude = np.sqrt(np.pi/p_complex)
-    spectrum_amplitude = np.sqrt(p_complex/np.abs(p_complex))
-    spectrum_gauss = np.exp(-(angular_frequency_shifted**2)/(4*p_complex))
-    spectrum_gabor = spectrum_amplitude * spectrum_gauss
-
-    return spectrum_gabor, frequency_shifted_hz
-
-
 def chirp_MQG_from_N(band_order_Nth: float,
                      index_shift: float = 0,
                      scale_base: float = scales.Slice.G2) -> Tuple[float, float, float]:
     """
     Compute the quality factor Q and multiplier M for a specified band order N
     N is THE quantization parameter for the binary constant Q wavelet filters
 
@@ -343,15 +307,17 @@
     wavelet_gabor, time_centered_s, amp_dict_0, amp_dict_1 = \
         chirp_complex(band_order_Nth,
                       time_s, offset_time_s, scale_frequency_center_hz, frequency_sample_rate_hz,
                       index_shift, scale_base)
 
     if dictionary_type == "norm":
         wavelet_chirp = amp_dict_0*wavelet_gabor
-    else:  # spectrum
+    elif dictionary_type == "tone":
+        wavelet_chirp = np.sqrt(2)*amp_dict_1*wavelet_gabor
+    else:
         wavelet_chirp = amp_dict_1*wavelet_gabor
 
     return wavelet_chirp, time_centered_s
 
 
 def cwt_chirp_complex(band_order_Nth: float,
                       sig_wf: np.ndarray,
```

### Comparing `libquantum-1.4.1/libquantum/atoms_inverse.py` & `libquantum-1.5.0a0/libquantum/atoms_inverse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/blast_pulse.py` & `libquantum-1.5.0a0/libquantum/blast_pulse.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/doppler.py` & `libquantum-1.5.0a0/libquantum/doppler.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/entropy.py` & `libquantum-1.5.0a0/libquantum/entropy.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/export.py` & `libquantum-1.5.0a0/libquantum/export.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/plot_templates/plot_geo_scatter_2d_3d.py` & `libquantum-1.5.0a0/libquantum/plot_templates/plot_geo_scatter_2d_3d.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/plot_templates/plot_time_frequency_picks.py` & `libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_picks.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/plot_templates/plot_time_frequency_reps.py` & `libquantum-1.5.0a0/libquantum/plot_templates/plot_time_frequency_reps.py`

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
-                       labels_fontweight: str = None) -> plt.Figure:
+                       labels_fontweight: str = None) -> None:
     """
     Template for aligned time-series display
 
     :param redvox_id: name of station
     :param wf_panel_0_sig: array with signal waveform for top panel
     :param wf_panel_0_time: array with signal timestamps for top panel
     :param wf_panel_1_sig: array with signal waveform for middle panel
@@ -340,16 +340,14 @@
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
 
-    return fig
-
 
 def plot_wf_mesh_mesh_vert(redvox_id: str,
                            wf_panel_2_sig: np.ndarray,
                            wf_panel_2_time: np.ndarray,
                            mesh_time: np.ndarray,
                            mesh_frequency: np.ndarray,
                            mesh_panel_1_trf: np.ndarray,
@@ -372,15 +370,15 @@
                            mesh_colormap: str = "inferno",
                            units_time: str = "s",
                            units_frequency: str = "Hz",
                            wf_panel_2_units: str = "Norm",
                            mesh_panel_1_cbar_units: str = "bits",
                            mesh_panel_0_cbar_units: str = "bits",
                            figure_title: str = "Time-Frequency Representation",
-                           figure_title_show: bool = True) -> plt.Figure:
+                           figure_title_show: bool = True) -> None:
 
     """
     Plot 3 vertical panels - mesh (top panel), mesh (middle panel) and signal waveform (bottom panel)
 
     :param redvox_id: name of station
     :param wf_panel_2_sig: array with signal waveform for bottom panel
     :param wf_panel_2_time: array with signal timestamps for bottom panel
@@ -594,16 +592,14 @@
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
 
-    return fig
-
 
 def plot_wf_mesh_vert(redvox_id: str,
                       wf_panel_2_sig: np.ndarray,
                       wf_panel_2_time: np.ndarray,
                       mesh_time: np.ndarray,
                       mesh_frequency: np.ndarray,
                       mesh_panel_0_tfr: np.ndarray,
@@ -620,15 +616,15 @@
                       waveform_color: str = "midnightblue",
                       mesh_colormap: str = "inferno",
                       units_time: str = "s",
                       units_frequency: str = "Hz",
                       wf_panel_2_units: str = "Norm",
                       mesh_panel_0_cbar_units: str = "bits",
                       figure_title: str = "Time-Frequency Representation",
-                      figure_title_show: bool = True) -> plt.Figure:
+                      figure_title_show: bool = True) -> None:
     """
     Plot 2 vertical panels - mesh (top panel) and signal waveform (bottom panel)
 
     :param redvox_id: name of station
     :param wf_panel_2_sig: array with signal waveform for bottom panel
     :param wf_panel_2_time: array with signal timestamps for bottom panel
     :param mesh_time: array with mesh time
@@ -774,9 +770,7 @@
     wf_panel_2_cax.axis("off")
 
     fig.text(.5, .01, time_label, ha='center', size=params_tfr.figure_parameters.text_size)
 
     fig.align_ylabels(axes)
     fig.tight_layout()
     fig.subplots_adjust(bottom=.1, hspace=0.13)
-
-    return fig
```

### Comparing `libquantum-1.4.1/libquantum/scales.py` & `libquantum-1.5.0a0/libquantum/scales.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/spectra.py` & `libquantum-1.5.0a0/libquantum/spectra.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/styx_stx.py` & `libquantum-1.5.0a0/libquantum/synthetics.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,243 +1,293 @@
-""""
-Standardized Stockwell transform (stx) with optimization parameters
-After Moukadem et al., 2022, A new optimized Stockwell transform applied on synthetic and real non-stationary signals
-Rederivation in preparation, Garces et al. 2022; last updated 9 May 2022
-
 """
+This module constructs synthetic signals
+"""
+
 import numpy as np
-from scipy.fft import fft, ifft, fftfreq
-from libquantum import scales, styx_cwt
-from typing import Tuple
+import scipy.signal as signal
+from scipy.integrate import cumulative_trapezoid
+from typing import Optional, Tuple, Union
+from libquantum import utils, scales, atoms
 
 
-def sig_pad_up_to_pow2(sig_wf: np.ndarray, n_fft: int):
+def gabor_tight_grain(band_order_Nth: float,
+                      scale_frequency_center_hz: float,
+                      frequency_sample_rate_hz: float,
+                      index_shift: float = 0,
+                      frequency_base_input: float = scales.Slice.G2) -> np.ndarray:
     """
-    Zero-pad signal to the higher 2**n points for FFT
-    :param sig_wf:
-    :param n_fft:
-    :return:
+    Gabor grain with tight Tukey wrap to ensure zero at edges
+
+    :param band_order_Nth: Nth order of constant Q bands
+    :param scale_frequency_center_hz: center frequency fc in Hz
+    :param frequency_sample_rate_hz: sample rate of frequency in Hz
+    :param index_shift: index of shift
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
+    # Time from nominal duration
+    grain_duration_s = cycles_M/scale_frequency_center_hz
+    time_s = np.arange(int(np.round(grain_duration_s*frequency_sample_rate_hz)))/frequency_sample_rate_hz
+    offset_time_s = np.max(time_s)/2.
+
+    xtime_shifted = atoms.chirp_time(time_s, offset_time_s, frequency_sample_rate_hz)
+    wavelet_gauss = np.exp(-p_complex * xtime_shifted**2)
+    wavelet_gabor = wavelet_gauss * np.exp(1j * cycles_M*xtime_shifted/scale_atom)
+    tight_grain_taper = utils.taper_tukey(wavelet_gabor, 0.1)
+    tight_grain = np.copy(wavelet_gabor)*tight_grain_taper
+
+    return tight_grain
+
+
+def tukey_tight_grain(band_order_Nth: float,
+                      scale_frequency_center_hz: float,
+                      frequency_sample_rate_hz: float,
+                      fraction_cosine: float = 0.5,
+                      index_shift: float = 0,
+                      frequency_base_input: float = scales.Slice.G2) -> np.ndarray:
     """
+    Tukey grain with same support as Gabor atom
 
-    # Flatten to 2 D and memorize original shape
-    n_times = sig_wf.shape[-1]
+    :param band_order_Nth: Nth order of constant Q bands
+    :param scale_frequency_center_hz: center frequency fc in Hz
+    :param frequency_sample_rate_hz: sample rate of frequency in Hz
+    :param fraction_cosine: fraction of the window inside the cosine tapered window, shared between the head and tail.
+        Default is 0.5
+    :param index_shift: index of shift
+    :param frequency_base_input: G2 or G3. Default is G2
+    :return: numpy array with Tukey grain
+    """
 
-    # Legerdemain
-    def _is_power_of_two(n):
-        return not (n > 0 and (n & (n - 1)))
-
-    if n_fft is None or (not _is_power_of_two(n_fft) and n_times > n_fft):
-        # Compute next power of 2
-        n_fft = 2 ** int(np.ceil(np.log2(n_times)))
-    elif n_fft < n_times:
-        raise ValueError("n_fft cannot be smaller than signal size. "
-                         "Got %s < %s." % (n_fft, n_times))
-    if n_times < n_fft:
-        # TODO: Add verbosity
-        # print('The input signal is shorter ({}) than "n_fft" ({}). '
-        #       'Applying zero padding.'.format(sig_wf.shape[-1], n_fft))
-        zero_pad: int = n_fft - n_times
-        pad_array = np.zeros(sig_wf.shape[:-1] + (zero_pad,), sig_wf.dtype)
-        sig_wf = np.concatenate((sig_wf, pad_array), axis=-1)
-    else:
-        zero_pad: int = 0
+    # Fundamental chirp parameters
+    cycles_M, quality_factor_Q, gamma = \
+        atoms.chirp_MQG_from_N(band_order_Nth, index_shift, frequency_base_input)
+    scale_atom = atoms.chirp_scale(cycles_M, scale_frequency_center_hz, frequency_sample_rate_hz)
+    p_complex = atoms.chirp_p_complex(scale_atom, gamma, index_shift)
+
+    # Time from nominal duration
+    grain_duration_s = cycles_M/scale_frequency_center_hz
+    time_s = np.arange(int(np.round(grain_duration_s*frequency_sample_rate_hz)))/frequency_sample_rate_hz
+    offset_time_s = np.max(time_s)/2.
+
+    xtime_shifted = atoms.chirp_time(time_s, offset_time_s, frequency_sample_rate_hz)
+    # Pull out phase component from gaussian envelope
+    wavelet_gauss_phase = np.imag(-p_complex * xtime_shifted**2)
+    wavelet_gabor = np.exp(1j * cycles_M*xtime_shifted/scale_atom + 1j * wavelet_gauss_phase)
+    tight_grain_taper = utils.taper_tukey(wavelet_gabor, fraction_cosine)
+    tight_grain = np.copy(wavelet_gabor)*tight_grain_taper
+
+    return tight_grain
+
+
+def gabor_grain_frequencies(frequency_order_input: float,
+                            frequency_low_input: float,
+                            frequency_high_input: float,
+                            frequency_sample_rate_input: float,
+                            frequency_base_input: float = scales.Slice.G2,
+                            frequency_ref_input: float = 1.0) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """
+    Frequencies for g-chirps
+
+    :param frequency_order_input: Nth order
+    :param frequency_low_input: lowest frequency of interest
+    :param frequency_high_input: highest frequency of interest
+    :param frequency_sample_rate_input: sample rate
+    :param frequency_base_input: G2 or G3. Default is G2
+    :param frequency_ref_input: reference frequency. Default is 1.0
+    :return: three numpy arrays with center frequency, start frequency and end frequency
+    """
 
-    return sig_wf, n_fft, zero_pad
+    scale_order, scale_base, _, frequency_ref, frequency_center_algebraic, \
+    frequency_center, frequency_start, frequency_end = \
+        scales.band_frequencies_low_high(frequency_order_input, frequency_base_input,
+                                         frequency_ref_input,
+                                         frequency_low_input,
+                                         frequency_high_input,
+                                         frequency_sample_rate_input)
+
+    return frequency_center, frequency_start, frequency_end
 
 
-def tfr_stx_fft(sig_wf: np.ndarray,
-                time_sample_interval: float,
-                scale_order_input: float = 8.0,
-                n_fft_in: int = None,
-                frequency_min: float = None,
-                frequency_max: float = None,
-                frequency_step: float = None,
-                factor_q: float = 0.,
-                power_p: float = 0.,
-                power_r: float = 1.,
-                is_geometric: bool = False,
-                is_inferno: bool = False,
-                scale_base_input: float = scales.Slice.G3,
-                scale_ref_input: float = scales.Slice.T1S,
-                ) -> Tuple[np.ndarray, np.ndarray,  np.ndarray, np.ndarray, np.ndarray]:
-    """
-    # Stockwell transform, fft implementation.
-    # Optimized version has more free variables in sigma_scaling; testing in progress
-    :param sig_wf: input waveform. If not 2**n points, it will zero pad up
-    :param time_sample_interval: sample interval, inverse of sample rate
-    :param scale_order_input: fractional octave band order; 12 is the musical standard
-    :param n_fft_in: requested nfft, should be greater or equal to the signal length. Method zero pads up.
-    :param frequency_min: lowest stx frequency of interest
-    :param frequency_max: highest stx frequency of interest
-    :param frequency_step: stx frequency of interest if linearly sampled
-    :param factor_q: sigma_scaling adjustment, under evaluation
-    :param power_p: sigma_scaling adjustment, under evaluation
-    :param power_r: sigma_scaling adjustment. under evaluation
-    :param is_geometric: are frequencies geometrically spaced? If so, overrides frequency_step
-    :param is_inferno: are frequencies geometrically spaced and standardized as in inferno?
-    :param scale_base_input: scale base; default is base 10, base 2 octaves is scales.Slice.G2
-    :param scale_ref_input: scale reference time; default is 1 s
-    # :return: tfr_stx, psd_stx, frequency_stx_hz, frequency_stx_fft, windows_fft
-    # """
-
-    frequency_sample_rate: float = 1 / time_sample_interval
-    cycles_M: float = 12. / 5. * scale_order_input
-    lin_fft_decimate: float = 2.
-
-    # Compute the nearest higher power of two number of points for the fft
-    sig_wf_pow2, n_fft_pow2, zero_pad = sig_pad_up_to_pow2(sig_wf, n_fft_in)
-
-    # For reduction back to the near original signal after taking the ifft. Should match input sig.
-    n_fft_out = n_fft_pow2 - zero_pad
-
-    # Transformations are on zero padded signals from here onwards
-    # Take FFT and concatenate. A leaner version could let the fft do the padding.
-    sig_fft = fft(sig_wf_pow2)
-    sig_fft_cat = np.concatenate([sig_fft, sig_fft], axis=-1)
-
-    frequency_fft = fftfreq(n_fft_pow2, time_sample_interval)   # in units of 1/sample interval
-    omega_fft = 2 * np.pi * frequency_fft / frequency_sample_rate  # scaled angular frequency
-
-    window_longest_time = n_fft_pow2 / frequency_sample_rate
-    frequency_min_nth = cycles_M/window_longest_time
-
-    # Initialize stx frequencies
-    if frequency_min is None:
-        frequency_min = frequency_min_nth
-    if frequency_max is None:
-        frequency_max = frequency_sample_rate / 2.
-
-    # Computing nearest frequency later on anyway, and then using that to compute the fft.
-    start_f_idx = np.abs(frequency_fft - frequency_min).argmin()
-    stop_f_idx = np.abs(frequency_fft - frequency_max).argmin()
-    f_start = frequency_fft[start_f_idx]
-    f_stop = frequency_fft[stop_f_idx]
-
-    # Linear scale
-    if frequency_step is None:
-        # Reduce the fft resolution by a factor of lin_fft_decimate
-        frequency_step = (frequency_max - frequency_min) * lin_fft_decimate/len(frequency_fft)
-        frequency_stx = np.arange(f_start, f_stop, frequency_step)
+def chirp_rdvxm_noise_16bit(duration_points: int = 2**12,
+                            sample_rate_hz: float = 80.,
+                            noise_std_loss_bits: float = 4.,
+                            frequency_center_hz: Optional[float] = None):
+    """
+    Construct chirp with linear frequency sweep, white noise added, anti-aliased filter applied
+
+    :param duration_points: number of points, length of signal. Default is 2 ** 12
+    :param sample_rate_hz: sample rate in Hz. Default is 80.0
+    :param noise_std_loss_bits: number of bits below signal standard deviation. Default is 4.0
+    :param frequency_center_hz: center frequency fc in Hz. Optional
+    :return: numpy ndarray with anti-aliased chirp with white noise
+    """
+
+    duration_s = duration_points/sample_rate_hz
+    if frequency_center_hz:
+        frequency_start_hz = 0.5*frequency_center_hz
+        frequency_end_hz = sample_rate_hz/4.
     else:
-        frequency_stx = np.arange(f_start, f_stop, frequency_step)
+        frequency_center_hz = 8./duration_s
+        frequency_start_hz = 0.5*frequency_center_hz
+        frequency_end_hz = sample_rate_hz/4.
+
+    sig_time_s = np.arange(int(duration_points))/sample_rate_hz
+    chirp_wf = signal.chirp(sig_time_s, frequency_start_hz, sig_time_s[-1],
+                            frequency_end_hz, method='linear', phi=0, vertex_zero=True)
+    chirp_wf *= taper_tukey(chirp_wf, 0.25)
+    noise_wf = white_noise_fbits(sig=chirp_wf, std_bit_loss=noise_std_loss_bits)
+    chirp_white = chirp_wf + noise_wf
+    chirp_white_aa = antialias_halfNyquist(chirp_white)
+    chirp_white_aa.astype(np.float16)
+
+    return chirp_white_aa
+
+
+def sawtooth_rdvxm_noise_16bit(duration_points: int = 2**12,
+                               sample_rate_hz: float = 80.,
+                               noise_std_loss_bits: float = 4.,
+                               frequency_center_hz: Optional[float] = None) -> np.ndarray:
+    """
+    Construct a anti-aliased sawtooth waveform with white noise
 
-    # if geometric (log) frequency
-    if is_geometric is True:
-        # if standardized to ISO3
-        if is_inferno is True:
-            order_Nth, scale_base, scale_band_number, \
-            frequency_ref, frequency_center_algebraic, frequency_center_geometric, \
-            frequency_start, frequency_end = \
-                scales.band_frequencies_low_high(frequency_order_input=scale_order_input,
-                                                 frequency_low_input=f_start,
-                                                 frequency_high_input=f_stop,
-                                                 frequency_sample_rate_input=frequency_sample_rate,
-                                                 frequency_base_input=scale_base_input,
-                                                 frequency_ref_input=scale_ref_input)
-            frequency_stx = frequency_center_geometric
-        else:
-            num_octaves = np.log2(f_stop/f_start)
-            num_bands = int(num_octaves * scale_order_input)
-            frequency_stx = np.logspace(np.log2(f_start), np.log2(f_stop), num=num_bands, base=scale_base_input)
-
-    # Construct shifting frequency indexes
-    frequency_stx_fft = np.empty(len(frequency_stx))
-
-    # Construct time domain and fft of window
-    windows_fft = np.empty((len(frequency_stx), n_fft_pow2), dtype=np.complex128)
-    # tfr_stx_pow2 = np.empty(1, n_fft_pow2, dtype=np.complex128)
-
-    tfr_stx = np.empty((len(frequency_stx), n_fft_out), dtype=np.complex128)
-    psd_stx = np.empty((len(frequency_stx), n_fft_out))
-
-    # Minimized for loops and operations
-    for isx, fsx in enumerate(frequency_stx):
-        stx_index = np.abs(frequency_fft - fsx).argmin()
-        frequency_stx_fft[isx] = frequency_fft[stx_index]
-        # omega_sx = 2*np.pi*frequency_stx_hz/sample_rate    # non-dimensional angular stx frequency
-        omega_sx = 2 * np.pi * frequency_stx_fft[isx]/frequency_sample_rate  # eq non-dimensional angular fft frequency
-        if omega_sx == 0.:
-            windows_fft[isx] = np.ones(len(n_fft_pow2))
-        else:
-            # Sigma is the standard deviation of the Gaussian
-            # Additional flexibility is added in gamma_sigma_scaling
-            sigma_scaling = (1 + factor_q * (omega_sx ** power_p)) * (omega_sx ** (1-power_r))
-            sigma = cycles_M/omega_sx
-            sigma *= sigma_scaling
-            windows_fft[isx] = np.exp(-0.5 * (sigma ** 2.) * (omega_fft ** 2.))
-
-        # This is the main event
-        tfr_stx_pow2 = ifft(sig_fft_cat[stx_index:stx_index + n_fft_pow2] * windows_fft[isx])
-        if zero_pad > 0:
-            tfr_stx[isx, :] = tfr_stx_pow2[:-zero_pad:1]
-        else:
-            tfr_stx[isx, :] = tfr_stx_pow2
-        # Power
-        tfr_abs = np.abs(tfr_stx[isx, :])**2
-        # Add EPSILON for zero handling
-        psd_stx[isx, :] = tfr_abs + scales.EPSILON
-
-    return tfr_stx, psd_stx, frequency_stx, frequency_stx_fft, windows_fft
-
-
-def stx_complex_any_scale_pow2(band_order_Nth: float,
-                               sig_wf: np.ndarray,
-                               frequency_sample_rate_hz: float,
-                               frequency_stx_hz: np.ndarray) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
-    """
-    With some assumptions and simplifications, and with some vectorization
-    :param band_order_Nth: Fractional octave band - revisit
-    :param sig_wf: input signal with 2^M points
-    :param frequency_sample_rate_hz: sample rate in Hz
-    :param frequency_stx_hz: frequency vector in increasing order
-    :return: 
-    """
-    n_fft_pow2 = len(sig_wf)
-    time_stx_s = np.arange(n_fft_pow2)/frequency_sample_rate_hz
-    scale_points = len(frequency_stx_hz)
-    cycles_M = styx_cwt.cycles_from_order(band_order_Nth=band_order_Nth)
-    # Take FFT and concatenate. A leaner version could let the fft do the padding.
-    sig_fft = fft(sig_wf)
-    sig_fft_cat = np.concatenate([sig_fft, sig_fft], axis=-1)
-
-    frequency_fft = fftfreq(n_fft_pow2, 1/frequency_sample_rate_hz)   # in units of 1/sample interval
-    omega_fft = 2 * np.pi * frequency_fft / frequency_sample_rate_hz  # scaled angular frequency
-    omega_stx = 2*np.pi*frequency_stx_hz/frequency_sample_rate_hz    # non-dimensional angular stx frequency
-    sigma_stx = cycles_M/omega_stx  # TODO: revisit; manage order vs frequency, use same nomenclature as cwt
-
-    # Construct 2d matrices
-    # sig_fft_cat_2d = np.tile(sig_fft_cat, (scale_points, 1))
-    omega_fft_2d = np.tile(omega_fft, (scale_points, 1))
-    sigma_stx_2d = np.tile(sigma_stx, (n_fft_pow2, 1)).T
-    windows_fft_2d = np.exp(-0.5 * (sigma_stx_2d ** 2.) * (omega_fft_2d ** 2.))
-
-    # Construct shifting frequency indexes
-    tfr_stx = np.empty((scale_points, n_fft_pow2), dtype=np.complex128)
-
-    # Minimal iteration
-    for isx, fsx in enumerate(frequency_stx_hz):
-        # This is the main event
-        stx_index = np.abs(frequency_fft - fsx).argmin()
-        tfr_stx[isx, :] = ifft(sig_fft_cat[stx_index:stx_index + n_fft_pow2] * windows_fft_2d[isx, :])
+    :param duration_points: number of points, length of signal. Default is 2 ** 12
+    :param sample_rate_hz: sample rate in Hz. Default is 80.0
+    :param noise_std_loss_bits: number of bits below signal standard deviation. Default is 4.0
+    :param frequency_center_hz: center frequency fc in Hz. Optional
+    :return: numpy ndarray with anti-aliased sawtooth signal with white noise
+    """
 
-    return frequency_stx_hz, time_stx_s, tfr_stx
+    duration_s = duration_points/sample_rate_hz
+    if frequency_center_hz:
+        frequency_center_angular = 2*np.pi*frequency_center_hz
+    else:
+        frequency_center_hz = 8./duration_s
+        frequency_center_angular = 2*np.pi*frequency_center_hz
 
+    sig_time_s = np.arange(int(duration_points))/sample_rate_hz
+    saw_wf = signal.sawtooth(frequency_center_angular*sig_time_s, width=0)
+    saw_wf *= taper_tukey(saw_wf, 0.25)
+    noise_wf = white_noise_fbits(sig=saw_wf, std_bit_loss=noise_std_loss_bits)
+    saw_white = saw_wf + noise_wf
+    saw_white_aa = antialias_halfNyquist(saw_white)
+    saw_white_aa.astype(np.float16)
+
+    return saw_white_aa
+
+
+def chirp_linear_in_noise(snr_bits: float,
+                          sample_rate_hz: float,
+                          duration_s: float,
+                          frequency_start_hz: float,
+                          frequency_end_hz: float,
+                          intro_s: Union[int, float],
+                          outro_s: Union[int, float]) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    Construct chirp with linear frequency sweep, white noise added.
 
-def power_and_information_shannon_stx(stx_complex):
+    :param snr_bits: number of bits below signal standard deviation
+    :param sample_rate_hz: sample rate in Hz
+    :param duration_s: duration of chirp in seconds
+    :param frequency_start_hz: start frequency in Hz
+    :param frequency_end_hz: end frequency in Hz
+    :param intro_s: number of seconds before chirp
+    :param outro_s: number of seconds after chirp
+    :return: numpy ndarray with waveform, numpy ndarray with time in seconds
     """
-    Computes power and information metrics
-    :param stx_complex:
+
+    sig_time_s = np.arange(int(sample_rate_hz*duration_s))/sample_rate_hz
+    chirp_wf = signal.chirp(sig_time_s, frequency_start_hz, sig_time_s[-1],
+                            frequency_end_hz, method='linear', phi=0, vertex_zero=True)
+    chirp_wf *= taper_tukey(chirp_wf, 0.25)
+    sig_wf = np.concatenate((np.zeros(int(intro_s*sample_rate_hz)),
+                             chirp_wf,
+                             np.zeros(int(outro_s*sample_rate_hz))))
+    noise_wf = white_noise_fbits(sig=sig_wf, std_bit_loss=snr_bits)
+    synth_wf = sig_wf+noise_wf
+    synth_time_s = np.arange(len(synth_wf))/sample_rate_hz
+    return synth_wf, synth_time_s
+
+
+def white_noise_fbits(sig: np.ndarray,
+                      std_bit_loss: float) -> np.ndarray:
+    """
+    Compute white noise with zero mean and standard deviation that is snr_bits below the input signal
+
+    :param sig: input signal, detrended
+    :param std_bit_loss: number of bits below signal standard deviation
+    :return: gaussian noise with zero mean
+    """
+    sig_std = np.std(sig)
+    # This is in power, or variance
+    noise_loss = 2.**std_bit_loss
+    std_from_fbits = sig_std/noise_loss
+    # White noise, zero mean
+    sig_noise = np.random.normal(0, std_from_fbits, size=sig.size)
+    return sig_noise
+
+
+def taper_tukey(sig_or_time: np.ndarray,
+                fraction_cosine: float) -> np.ndarray:
+    """
+    Constructs a symmetric Tukey window with the same dimensions as a time or signal numpy array.
+    fraction_cosine = 0 is a rectangular window, 1 is a Hann window
+
+    :param sig_or_time: input signal or time
+    :param fraction_cosine: fraction of the window inside the cosine tapered window, shared between the head and tail
+    :return: tukey taper window amplitude
+    """
+    number_points = np.size(sig_or_time)
+    amplitude = signal.windows.tukey(M=number_points, alpha=fraction_cosine, sym=True)
+    return amplitude
+
+
+def antialias_halfNyquist(synth: np.ndarray) -> np.ndarray:
+    """
+    Anti-aliasing filter with -3dB at 1/4 of sample rate, 1/2 of Nyquist
+
+    :param synth: array with signal data
+    :return: numpy array with anti-aliased signal
+    """
+    # Anti-aliasing filter with -3dB at 1/4 of sample rate, 1/2 of Nyquist
+    # Signal frequencies are scaled by Nyquist
+    filter_order = 2
+    edge_high = 0.5
+    [b, a] = signal.butter(filter_order, edge_high, btype='lowpass')
+    synth_anti_aliased = signal.filtfilt(b, a, np.copy(synth))
+    return synth_anti_aliased
+
+
+def frequency_algebraic_Nth(frequency_geometric: np.ndarray,
+                            band_order_Nth: float) -> np.ndarray:
+    """
+    Compute algebraic frequencies in band order
+
+    :param frequency_geometric: geometric frequencies
+    :param band_order_Nth:  Nth order of constant Q bands
     :return:
     """
-    power = 2 * np.abs(np.copy(stx_complex)) ** 2
-    power_per_band = np.sum(power, axis=-1)
-    power_per_sample = np.sum(power, axis=0)
-    power_total = np.sum(power) + scales.EPSILON
-    power_scaled = power/power_total
-    information_bits = -power_scaled*np.log2(power_scaled + scales.EPSILON)
-    information_bits_per_band = np.sum(information_bits, axis=-1)
-    information_bits_per_sample = np.sum(information_bits, axis=0)
-    information_bits_total = np.sum(information_bits) + scales.EPSILON
-    information_scaled = information_bits/information_bits_total
-    return power, power_per_band, power_per_sample, power_total, power_scaled, \
-           information_bits, information_bits_per_band, information_bits_per_sample, \
-           information_bits_total, information_scaled
+    frequency_algebra = frequency_geometric*(np.sqrt(1+1/(8*band_order_Nth**2)))
+    return frequency_algebra
+
+
+def integrate_cumtrapz(timestamps_s: np.ndarray,
+                       sensor_wf: np.ndarray,
+                       initial_value: float = 0) -> np.ndarray:
+    """
+    cumulative trapezoid integration using scipy.integrate.cumulative_trapezoid
+
+    :param timestamps_s: timestamps corresponding to the data in seconds
+    :param sensor_wf: data to integrate using cumulative trapezoid
+    :param initial_value: the value to add in the initial of the integrated data to match length of input (default is 0)
+    :return: integrated data with the same length as the input
+    """
+    integrated_data = cumulative_trapezoid(x=timestamps_s,
+                                           y=sensor_wf,
+                                           initial=initial_value)
+    return integrated_data
```

### Comparing `libquantum-1.4.1/libquantum/tfr_gate_pick.py` & `libquantum-1.5.0a0/libquantum/tfr_gate_pick.py`

 * *Files identical despite different names*

### Comparing `libquantum-1.4.1/libquantum/utils.py` & `libquantum-1.5.0a0/libquantum/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,146 +2,34 @@
 This module contains general utilities that can work with values containing nans.
 """
 
 from enum import Enum
 from typing import Tuple, Union
 
 import numpy as np
-from scipy import interpolate, signal
+from scipy import signal
 
 from scipy.integrate import cumulative_trapezoid
 from libquantum.scales import EPSILON
 from redvox.common import date_time_utils as dt
 
-""" Logical power of two flag """
-
-
-def is_power_of_two(n):
-    """ Returns not if not positive and a power of two """
-    return not (n > 0 and (n & (n - 1)))
-
-
-""" Time/Sample Duration Utils """
-
-
-def duration_points(sample_rate_hz: float, time_s: float) -> Tuple[int, int, int]:
-    """
-    Compute number of points
-    :param sample_rate_hz: sample rate in Hz
-    :param time_s: time scale, period or duration
-    :return: number of points, floor and ceiling of log2 of number of points
-    """
-    points_float: float = sample_rate_hz * time_s
-    points_int: int = int(points_float)
-    points_floor_log2: int = int(np.floor(np.log2(points_float)))
-    points_ceil_log2: int = int(np.ceil(np.log2(points_float)))
-
-    return points_int, points_floor_log2, points_ceil_log2
-
-
-def duration_ceil(sample_rate_hz: float, time_s: float) -> Tuple[int, int, float]:
-    """
-    Compute ceiling of the number of points, and convert to seconds
-    :param sample_rate_hz: sample rate in Hz
-    :param time_s: time scale, period or duration
-    :return: ceil of log 2 of number of points, power of two number of points, corresponding time in s
-    """
-    points_float: float = sample_rate_hz * time_s
-    points_ceil_log2: int = int(np.ceil(np.log2(points_float)))
-    points_ceil_pow2: int = 2**points_ceil_log2
-    time_ceil_pow2_s: float = points_ceil_pow2 / sample_rate_hz
-
-    return points_ceil_log2, points_ceil_pow2, time_ceil_pow2_s
-
-
-def duration_floor(sample_rate_hz: float, time_s: float) -> Tuple[int, int, float]:
-    """
-    Compute floor of the number of points, and convert to seconds
-    :param sample_rate_hz: sample rate in Hz
-    :param time_s: time scale, period or duration
-    :return: floor of log 2 of number of points, power of two number of points, corresponding time in s
-    """
-    points_float: float = sample_rate_hz * time_s
-    points_floor_log2: int = int(np.floor(np.log2(points_float)))
-    points_floor_pow2: int = 2**points_floor_log2
-    time_floor_pow2_s: float = points_floor_pow2 / sample_rate_hz
-
-    return points_floor_log2, points_floor_pow2, time_floor_pow2_s
-
-
-""" Sampling Utils """
-
-
-def resample_uneven_signal(sig_wf: np.ndarray,
-                           sig_epoch_s: np.ndarray,
-                           sample_rate_new_hz: float = None):
-    """
-
-    :param sig_wf:
-    :param sig_epoch_s:
-    :param sample_rate_new_hz:
-    :return:
-    """
-
-    if sample_rate_new_hz is None:
-        interval_from_epoch_s = np.mean(np.diff(sig_epoch_s))
-        # Round up
-        sample_rate_new_hz = np.ceil(1/interval_from_epoch_s)
-
-    interval_s = 1/sample_rate_new_hz
-    sig_new_epoch_s = np.arange(sig_epoch_s[0], sig_epoch_s[-1], interval_s)
-    f = interpolate.interp1d(sig_epoch_s, sig_wf)
-    sig_new_wf = f(sig_new_epoch_s)
-    return sig_new_wf, sig_new_epoch_s
-
-
-def upsample_fourier(sig_wf: np.ndarray,
-                     sig_sample_rate_hz: float,
-                     new_sample_rate_hz: float = 8000.) -> np.ndarray:
-    """
-    Upsample the Fourier way.
-
-    :param sig_wf: input signal waveform, reasonably well preprocessed
-    :param sig_sample_rate_hz: signal sample rate
-    :param new_sample_rate_hz: resampling sample rate
-    :return: resampled signal
-    """
-    sig_len = len(sig_wf)
-    new_len = int(sig_len * new_sample_rate_hz / sig_sample_rate_hz)
-    sig_resampled = signal.resample(x=sig_wf, num=new_len)
-    return sig_resampled
-
 
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
 
 
-# def taper_tukey_array(number_signals: int,
-#                       number_samples: int,
-#                       fraction_cosine: float = 0.1) -> np.ndarray:
-#     """
-#     Construct a teper matrix
-#     :param number_signals:
-#     :param number_samples:
-#     :param fraction_cosine:
-#     :return:
-#     """
-#     tukey_nsamples = signal.windows.tukey(M=number_samples, alpha=fraction_cosine, sym=True)
-#     tukey_array = just_tile(tukey_nsamples)
-
-
 def datetime_now_epoch_s() -> float:
     """
     Returns the invocation Unix time in seconds
 
     :return: The current epoch timestamp as seconds since the epoch UTC
     """
     return dt.datetime_to_epoch_seconds_utc(dt.now())
@@ -560,26 +448,7 @@
         raise TypeError('Cannot handle an array of shape {}.'.format(str(d1.shape)))
 
     if d1_matrix.shape == d2.shape:
         d1_x_d2 = d1_matrix * d2
     else:
         raise TypeError('Cannot handle an array of shape {}.'.format(str(d1.shape)))
     return d1_x_d2
-
-
-def decimate_array(sig_wf: np.array,
-                   downsampling_factor: int) -> np.ndarray:
-    """
-    Decimate data and timestamps for an individual station
-    All signals MUST have the same sample rate
-    :param sig_wf: signal waveform
-    :param downsampling_factor: the downsampling factor
-    :param filter_order: the order of the filter
-    :return: np.array decimated data
-    """
-    # decimate signal data
-    decimated_data = signal.decimate(x=sig_wf,
-                                    q=downsampling_factor,
-                                    axis=1,
-                                    zero_phase=True)
-
-    return decimated_data
```

