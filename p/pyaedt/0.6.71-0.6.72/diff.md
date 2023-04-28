# Comparing `tmp/pyaedt-0.6.71.tar.gz` & `tmp/pyaedt-0.6.72.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.71.tar", last modified: Fri Apr 14 08:21:39 2023, max compression
+gzip compressed data, was "pyaedt-0.6.72.tar", last modified: Fri Apr 28 08:03:00 2023, max compression
```

## Comparing `pyaedt-0.6.71.tar` & `pyaedt-0.6.72.tar`

### file list

```diff
@@ -1,249 +1,251 @@
--rw-r--r--   0        0        0     1111 2023-03-24 16:12:59.270687 pyaedt-0.6.71/LICENSE
--rw-r--r--   0        0        0     9857 2023-04-07 12:13:26.641029 pyaedt-0.6.71/README.rst
--rw-r--r--   0        0        0     2503 2023-04-14 08:04:16.194632 pyaedt-0.6.71/pyaedt/__init__.py
--rw-r--r--   0        0        0    26253 2023-03-24 16:13:01.176952 pyaedt-0.6.71/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-03-24 16:13:01.176952 pyaedt-0.6.71/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88739 2023-04-07 18:09:06.609599 pyaedt-0.6.71/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41260 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17009 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19795 2023-04-06 10:12:59.809616 pyaedt-0.6.71/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4374 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4539 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   126722 2023-03-27 07:03:01.756479 pyaedt-0.6.71/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    72583 2023-04-03 13:04:44.954527 pyaedt-0.6.71/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12433 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    37014 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    57605 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    57176 2023-04-13 13:45:42.136087 pyaedt-0.6.71/pyaedt/desktop.py
--rw-r--r--   0        0        0    23552 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0    23996 2023-03-24 16:13:01.192583 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   249856 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll
--rw-r--r--   0        0        0   481931 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.xml
--rw-r--r--   0        0        0   131072 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll
--rw-r--r--   0        0        0    85860 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.xml
--rw-r--r--   0        0        0    86016 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.dll
--rw-r--r--   0        0        0    51586 2023-03-24 16:13:01.208206 pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.RtfRendering-gdi.xml
--rw-r--r--   0        0        0   700336 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   707721 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0   585728 2023-03-24 16:13:01.223835 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll
--rw-r--r--   0        0        0  1164073 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.xml
--rw-r--r--   0        0        0    94208 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.dll
--rw-r--r--   0        0        0   129427 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp.Charting-gdi.xml
--rw-r--r--   0        0        0     9728 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.DocumentObjectModel-gdi.resources.dll
--rw-r--r--   0        0        0     7168 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.Rendering-gdi.resources.dll
--rw-r--r--   0        0        0     7168 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/MigraDoc.RtfRendering-gdi.resources.dll
--rw-r--r--   0        0        0     5120 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp-gdi.resources.dll
--rw-r--r--   0        0        0     4608 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/dlls/PDFReport/de/PdfSharp.Charting-gdi.resources.dll
--rw-r--r--   0        0        0    23488 2023-03-24 16:43:09.200130 pyaedt-0.6.71/pyaedt/downloads.py
--rw-r--r--   0        0        0   130992 2023-04-13 18:44:13.853500 pyaedt-0.6.71/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-04-06 16:52:05.688099 pyaedt-0.6.71/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    88157 2023-04-12 15:16:57.734625 pyaedt-0.6.71/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32856 2023-04-06 16:52:05.688099 pyaedt-0.6.71/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0      937 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0     1166 2023-03-24 16:13:01.239463 pyaedt-0.6.71/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    65580 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20305 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4724 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    58397 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32298 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    96895 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36296 2023-03-24 16:43:09.200130 pyaedt-0.6.71/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    31276 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-03-27 19:21:09.792652 pyaedt-0.6.71/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     2657 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    60230 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-03-24 16:13:01.255091 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7706 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4646 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11163 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-03-24 16:13:01.270714 pyaedt-0.6.71/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    48211 2023-04-03 15:08:34.103504 pyaedt-0.6.71/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33242 2023-04-07 12:13:26.672217 pyaedt-0.6.71/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43680 2023-04-07 07:07:57.602451 pyaedt-0.6.71/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46506 2023-04-06 10:00:43.540000 pyaedt-0.6.71/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57133 2023-04-06 16:52:05.703674 pyaedt-0.6.71/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   108085 2023-04-13 08:40:21.234448 pyaedt-0.6.71/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    10889 2023-03-31 19:32:16.029670 pyaedt-0.6.71/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3256 2023-03-31 19:32:16.029670 pyaedt-0.6.71/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0      448 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     6796 2023-04-10 16:06:04.843675 pyaedt-0.6.71/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    11153 2023-04-10 16:06:04.843675 pyaedt-0.6.71/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-03-27 11:43:10.713537 pyaedt-0.6.71/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3021 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83375 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    19616 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3416 2023-03-30 13:17:30.662219 pyaedt-0.6.71/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    62967 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    62296 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-03-24 16:13:01.286342 pyaedt-0.6.71/pyaedt/generic/process.py
--rw-r--r--   0        0        0    19736 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60355 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17088 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252857 2023-04-13 10:51:58.724974 pyaedt-0.6.71/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-04-06 10:12:59.840928 pyaedt-0.6.71/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   157774 2023-04-13 16:06:58.693317 pyaedt-0.6.71/pyaedt/icepak.py
--rw-r--r--   0        0        0   118317 2023-04-14 08:04:16.194632 pyaedt-0.6.71/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7816 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    23989 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-04-03 09:42:52.307879 pyaedt-0.6.71/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-04-03 09:42:52.307879 pyaedt-0.6.71/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0     8973 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-03-24 16:13:01.301964 pyaedt-0.6.71/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3507 2023-03-30 18:43:32.942201 pyaedt-0.6.71/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-03-24 16:13:01.317589 pyaedt-0.6.71/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-03-24 16:13:01.317589 pyaedt-0.6.71/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14076 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    19994 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18540 2023-03-24 16:13:01.333212 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16809 2023-04-07 12:58:12.911113 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120831 2023-04-05 05:51:01.697466 pyaedt-0.6.71/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194519 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   115251 2023-04-13 15:34:05.970087 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11332 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   119547 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    29079 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49002 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59392 2023-04-11 17:32:37.677113 pyaedt-0.6.71/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53056 2023-04-06 09:42:17.714071 pyaedt-0.6.71/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12588 2023-04-13 16:06:58.693317 pyaedt-0.6.71/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42008 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32175 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8157 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63043 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15094 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.348840 pyaedt-0.6.71/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    31983 2023-04-13 10:24:29.982183 pyaedt-0.6.71/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    67799 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6902 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    48446 2023-04-06 10:24:56.942325 pyaedt-0.6.71/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31270 2023-04-13 15:34:05.970087 pyaedt-0.6.71/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49786 2023-03-28 09:14:52.645654 pyaedt-0.6.71/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65526 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    21619 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30108 2023-03-31 13:49:23.220683 pyaedt-0.6.71/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   113864 2023-04-06 09:22:52.765550 pyaedt-0.6.71/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51910 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    39609 2023-04-13 15:34:05.985626 pyaedt-0.6.71/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82846 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28306 2023-03-24 16:43:09.215755 pyaedt-0.6.71/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53168 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11919 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26048 2023-03-31 13:49:23.236244 pyaedt-0.6.71/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-03-24 16:13:01.364468 pyaedt-0.6.71/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   172107 2023-04-13 10:24:29.997810 pyaedt-0.6.71/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   116130 2023-04-06 09:42:17.729701 pyaedt-0.6.71/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33226 2023-04-07 13:54:16.226712 pyaedt-0.6.71/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28652 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103276 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   124676 2023-04-07 09:25:28.374503 pyaedt-0.6.71/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95492 2023-04-13 10:24:29.997810 pyaedt-0.6.71/pyaedt/q3d.py
--rw-r--r--   0        0        0    10556 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-04-03 14:30:32.207324 pyaedt-0.6.71/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-03-24 16:13:01.380091 pyaedt-0.6.71/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-03-28 22:11:06.632650 pyaedt-0.6.71/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7601 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10373 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-03-24 16:13:01.395712 pyaedt-0.6.71/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4066 2023-04-12 13:46:49.217739 pyaedt-0.6.71/pyproject.toml
--rw-r--r--   0        0        0    14845 1970-01-01 00:00:00.000000 pyaedt-0.6.71/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-04-27 10:48:38.937375 pyaedt-0.6.72/LICENSE
+-rw-r--r--   0        0        0    10041 2023-04-27 10:48:38.937375 pyaedt-0.6.72/README.rst
+-rw-r--r--   0        0        0     2503 2023-04-28 07:45:45.191789 pyaedt-0.6.72/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26253 2023-04-27 10:48:40.495559 pyaedt-0.6.72/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-04-27 10:48:40.495559 pyaedt-0.6.72/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88739 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41260 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17009 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19795 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4374 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4539 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   127521 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75493 2023-04-27 13:08:15.716301 pyaedt-0.6.72/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12433 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    37014 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    57605 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    57382 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-04-27 10:48:40.511198 pyaedt-0.6.72/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-04-27 10:48:40.526826 pyaedt-0.6.72/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-04-27 10:48:40.526826 pyaedt-0.6.72/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-04-27 10:48:40.526826 pyaedt-0.6.72/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-04-27 10:48:40.526826 pyaedt-0.6.72/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-04-27 10:48:40.526826 pyaedt-0.6.72/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-04-27 10:48:40.542451 pyaedt-0.6.72/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-04-27 10:48:40.542451 pyaedt-0.6.72/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-04-27 10:48:40.542451 pyaedt-0.6.72/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-04-27 10:48:40.542451 pyaedt-0.6.72/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-04-27 10:48:40.558076 pyaedt-0.6.72/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-04-27 10:48:40.558076 pyaedt-0.6.72/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-04-27 10:48:40.589270 pyaedt-0.6.72/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-04-27 10:48:40.589270 pyaedt-0.6.72/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-04-27 10:48:40.589270 pyaedt-0.6.72/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-04-27 10:48:40.589270 pyaedt-0.6.72/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-04-27 10:48:40.589270 pyaedt-0.6.72/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/downloads.py
+-rw-r--r--   0        0        0   132415 2023-04-28 07:45:45.191789 pyaedt-0.6.72/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    87982 2023-04-27 15:58:46.158994 pyaedt-0.6.72/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32856 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0      937 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0     1166 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12081 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65580 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20305 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4724 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61111 2023-04-27 15:58:46.158994 pyaedt-0.6.72/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32298 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99826 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36282 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    31276 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    60863 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.604919 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7706 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4646 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-04-27 10:48:40.620538 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11163 2023-04-27 12:53:11.246332 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    47799 2023-04-27 15:58:46.158994 pyaedt-0.6.72/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33242 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43680 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    45432 2023-04-27 12:53:11.246332 pyaedt-0.6.72/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57133 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   108108 2023-04-28 07:45:45.191789 pyaedt-0.6.72/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11275 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0      791 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7546 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    11682 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3190 2023-04-27 10:48:40.636162 pyaedt-0.6.72/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83387 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    19616 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3416 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    63135 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9872 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62296 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    19736 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60355 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252855 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   154882 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118433 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-04-27 10:48:40.651785 pyaedt-0.6.72/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24259 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3829 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-04-27 10:48:40.667417 pyaedt-0.6.72/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14076 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    19994 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16809 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120831 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194519 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   115253 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11332 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   119788 2023-04-27 12:53:11.246332 pyaedt-0.6.72/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    29079 2023-04-27 10:48:40.683090 pyaedt-0.6.72/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49002 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59350 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53084 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12588 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42270 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32270 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8157 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63043 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15094 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    31983 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    67799 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6897 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52430 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31270 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49837 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65608 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    21640 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   113864 2023-04-27 10:48:40.698662 pyaedt-0.6.72/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51910 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40297 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82846 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28306 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53168 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11919 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26048 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   172808 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119128 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33226 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28652 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103276 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125048 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95482 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10556 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.714291 pyaedt-0.6.72/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7601 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10373 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4063 2023-04-27 10:48:40.729916 pyaedt-0.6.72/pyproject.toml
+-rw-r--r--   0        0        0    15020 1970-01-01 00:00:00.000000 pyaedt-0.6.72/PKG-INFO
```

### Comparing `pyaedt-0.6.71/LICENSE` & `pyaedt-0.6.72/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/README.rst` & `pyaedt-0.6.72/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -35,67 +35,69 @@
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyaedt/main.svg
    :target: https://results.pre-commit.ci/latest/github/pyansys/pyaedt/main
    :alt: pre-commit.ci status
 
 
 What is PyAEDT?
 ---------------
-PyAEDT is a Python library that interacts directly with the AEDT API
-to make scripting simpler for the end user. Its architecture
-can be reused for all AEDT 3D products (HFSS, Icepak, Maxwell 3D, and
-Q3D Extractor), 2D tools, and Ansys Mechanical. It also provides support for circuit
-tools like Nexxim and system simulation tools like Twin Builder. Finally it provides
-scripting capabilities in Ansys layout tools like HFSS 3D Layout and EDB. Its class
-and method structures simplify operation for the end user while reusing information
-as much as possible across the API.
+PyAEDT is a Python library that interacts directly with the API for
+Ansys Electronics Desktop (AEDT) to make scripting simpler. The architecture
+for PyAEDT can be reused for all AEDT 3D products (HFSS, Icepak, Maxwell 3D,
+and Q3D Extractor), 2D tools, and Ansys Mechanical. PyAEDT also provides
+support for circuit tools like Nexxim and system simulation tools like
+Twin Builder. Finally, PyAEDT provides scripting capabilities in Ansys layout
+tools like HFSS 3D Layout and EDB. The PyAEDT class and method structures
+simplify operation while reusing information as much as possible across
+the API.
 
 Install on CPython from PyPI
 ----------------------------
-You can install PyAEDT on CPython 3.7 through 3.10 from PyPI:
+You can install PyAEDT on CPython 3.7 through 3.10 from PyPI with this command:
 
 .. code:: python
 
     pip install pyaedt
 
-Install PyAEDT with all extra packages (matplotlib, numpy, pandas, pyvista):
+To install PyAEDT with all extra packages (Matplotlib, NumPy, Pandas, and PyVista),
+use this command:
 
 .. code:: python
 
     pip install pyaedt[full]
 
-You can also install PyAEDT from Conda-Forge:
+You can also install PyAEDT from Conda-Forge with this command:
 
 .. code:: python
 
     conda install -c conda-forge pyaedt
 
-PyAEDT remains compatible with Ironpython and can be still used in AEDT Framework.
+PyAEDT remains compatible with IronPython and can be still used in the AEDT Framework.
 
 About PyAnsys
 -------------
 
 PyAEDT is part of the larger `PyAnsys <https://docs.pyansys.com>`_
 effort to facilitate the use of Ansys technologies directly from Python.
 
 PyAEDT is intended to consolidate and extend all existing
-functionalities around scripting for Ansys Electronics Desktop (AEDT)
-to allow reuse of existing code, sharing of best practices, and increased
-collaboration.
+functionalities around scripting for AEDT to allow reuse of existing code,
+sharing of best practices, and increased collaboration.
 
 
 About AEDT
 ----------
 
-The Ansys Electronics Desktop (AEDT) is a platform that enables true electronics system design.
-`AEDT <https://www.ansys.com/products/electronics>`_ provides access to the Ansys gold-standard
-electro-magnetics simulation solutions such as Ansys HFSS,
-Ansys Maxwell, Ansys Q3D Extractor, Ansys Siwave, and Ansys Icepak using electrical CAD (ECAD) and
+`AEDT <https://www.ansys.com/products/electronics>`_ is a platform that enables true
+electronics system design. AEDT provides access to the Ansys gold-standard
+electro-magnetics simulation solutions, such as Ansys HFSS, Ansys Maxwell,
+Ansys Q3D Extractor, Ansys Siwave, and Ansys Icepak using electrical CAD (ECAD) and
 Mechanical CAD (MCAD) workflows.
-In addition, it includes direct links to the complete Ansys portfolio of thermal, fluid,
-and Mechanical solvers for comprehensive multiphysics analysis.
+
+In addition, AEDT includes direct links to the complete Ansys portfolio of thermal, fluid,
+and mechanical solvers for comprehensive multiphysics analysis.
 Tight integration among these solutions provides unprecedented ease of use for setup and
 faster resolution of complex simulations for design and optimization.
 
 .. image:: https://images.ansys.com/is/image/ansys/ansys-electronics-technology-collage?wid=941&op_usm=0.9,1.0,20,0&fit=constrain,0
   :width: 800
   :alt: AEDT Applications
   :target: https://www.ansys.com/products/electronics
@@ -114,50 +116,54 @@
 - Nexxim
 - EDB
 - Twin Builder
 
 
 Documentation and issues
 ------------------------
-In addition to installation and usage information, the PyAEDT
-documentation provides `API reference <https://aedt.docs.pyansys.com/release/0.6/API/index.html>`_,
-`Examples <https://aedt.docs.pyansys.com/release/0.6/examples/index.html>`_, and `Contribute 
-<https://aedt.docs.pyansys.com/release/0.6/Contributing.html>`_ sections.
+Documentation for the latest stable release of PyAEDT is hosted at
+`PyAEDT Documentation <https://aedt.docs.pyansys.com/version/stable/>`_.
+
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
 
 On the `PyAEDT Issues <https://github.com/pyansys/PyAEDT/issues>`_ page, you can
-create issues to submit questions, report bugs, and request new features. To reach
-the project support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+create issues to submit questions, report bugs, and request new features.
+
+To reach the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Dependencies
 ------------
-To run PyAEDT, you must have a local licenced copy of AEDT.
-PyAEDT supports AEDT versions 2022 R1 or newer.
+To run PyAEDT, you must have a local licensed copy of AEDT.
+PyAEDT supports AEDT versions 2022 R1 and later.
 
 Student version
 ---------------
 
-PyAEDT supports AEDT Student version 2022 R1 and later. For more information, see
-`Student Version page <https://www.ansys.com/academic/students/ansys-e
-lectronics-desktop-student>`_.
+PyAEDT supports AEDT Student versions 2022 R1 and later. For more information, see
+`Ansys Electronics Desktop Student  - Free Software Download <https://www.ansys.com/academic/students/ansys-e
+lectronics-desktop-student>`_ on the Ansys website.
 
 
 Why PyAEDT?
 -----------
 A quick and easy approach for automating a simple operation in the 
-AEDT UI is to record and reuse a script. However, disadvantages of 
-this approach are:
+AEDT UI is to record and reuse a script. However, here are some disadvantages of 
+this approach:
 
 - Recorded code is dirty and difficult to read and understand.
 - Recorded scripts are difficult to reuse and adapt.
 - Complex coding is required by many global users of AEDT.
 
-The main advantages of PyAEDT are:
+Here are the main advantages that PyAEDT provides:
 
 - Automatic initialization of all AEDT objects, such as desktop
-  objects like the editor, boundaries, and so on
+  objects like the editor, boundaries, and more
 - Error management
 - Log management
 - Variable management
 - Compatibility with IronPython and CPython
 - Simplification of complex API syntax using data objects while
   maintaining PEP8 compliance.
 - Code reusability across different solvers
@@ -167,17 +173,17 @@
 
 Example workflow
 -----------------
 1. Initialize the ``Desktop`` class with the version of AEDT to use.
 2. Initialize the application to use within AEDT.
 
 
-Connect to AEDT from Python IDE
--------------------------------
-PyAEDT works both inside AEDT and as a standalone application.
+Connect to AEDT from a Python IDE
+---------------------------------
+PyAEDT works both inside AEDT and as a standalone app.
 This Python library automatically detects whether it is running
 in an IronPython or CPython environment and initializes AEDT accordingly.
 PyAEDT also provides advanced error management. Usage examples follow.
 
 Explicit AEDT declaration and error management
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -215,15 +221,15 @@
 
 
 Remote application call
 ~~~~~~~~~~~~~~~~~~~~~~~
 You can make a remote application call on a CPython server
 or any Windows client machine.
 
-On a CPython Server:
+On a CPython server:
 
 .. code:: python
 
     # Launch PyAEDT remote server on CPython
 
     from pyaedt.common_rpc import pyaedt_service_manager
     pyaedt_service_manager()
@@ -268,9 +274,9 @@
 
 This module makes no commercial claim over Ansys whatsoever.
 PyAEDT extends the functionality of AEDT by adding
 an additional Python interface to AEDT without changing the core
 behavior or license of the original software. The use of the
 interactive control of PyAEDT requires a legally licensed
 local copy of AEDT. For more information about AEDT, 
-visit the `AEDT page <https://www.ansys.com/products/electronics>`_ 
-on the Ansys website.
+see the `Ansys Electronics <https://www.ansys.com/products/electronics>`_ 
+page on the Ansys website.
```

### Comparing `pyaedt-0.6.71/pyaedt/__init__.py` & `pyaedt-0.6.72/pyaedt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 os.environ["ANSYSEM_FEATURE_SF6694_NON_GRAPHICAL_COMMAND_EXECUTION_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.71"
+__version__ = "0.6.72"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
 from pyaedt.generic.general_methods import _pythonver
```

### Comparing `pyaedt-0.6.71/pyaedt/aedt_logger.py` & `pyaedt-0.6.72/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.72/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/Analysis.py` & `pyaedt-0.6.72/pyaedt/application/Analysis.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.72/pyaedt/application/Analysis3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.72/pyaedt/application/Analysis3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.72/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.72/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.72/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.72/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/Design.py` & `pyaedt-0.6.72/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,18 +207,15 @@
 
         self.student_version = main_module.student_version
         if self.student_version:
             settings.disable_bounding_box_sat = True
         self._mttime = None
         self._design_type = design_type
         self._desktop = main_module.oDesktop
-        try:
-            settings.enable_desktop_logs = not main_module.oDesktop.GetIsNonGraphical()
-        except AttributeError:
-            settings.enable_desktop_logs = not non_graphical
+
         self._desktop_install_dir = main_module.sDesktopinstallDirectory
         self._odesign = None
         self._oproject = None
         self._design_type = design_type
         if design_type == "HFSS":
             self.design_solutions = HFSSDesignSolution(None, design_type, self._aedt_version)
         elif design_type == "Icepak":
@@ -1911,22 +1908,41 @@
         >>> oDesign.ChangeProperty
 
         Examples
         --------
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> hfss["my_hidden_leaf"] = "15mm"
-        >>> hfss.make_hidden_variable("my_hidden_leaf")
+        >>> hfss.hidden_variable("my_hidden_leaf", True)
 
         """
-        if not isinstance(variable_name, list):
-            variable_name = [variable_name]
 
-        for var in variable_name:
-            self.variable_manager[var].hidden = value
+        if not isinstance(variable_name, list):
+            self.variable_manager[variable_name].hidden = value
+        else:
+            design_variables = ["NAME:ChangedProps"]
+            project_variables = ["NAME:ChangedProps"]
+            for name in variable_name:
+                if name in self.variable_manager.design_variable_names:
+                    design_variables.append(["NAME:" + name, "Hidden:=", value])
+                elif name in self.variable_manager.project_variable_names:
+                    project_variables.append(["NAME:" + name, "Hidden:=", value])
+
+            if len(design_variables) > 1:
+                command = [
+                    "NAME:AllTabs",
+                    ["NAME:LocalVariableTab", ["NAME:PropServers", "LocalVariables"], design_variables],
+                ]
+                self.odesign.ChangeProperty(command)
+            if len(project_variables) > 1:
+                command = [
+                    "NAME:AllTabs",
+                    ["NAME:ProjectVariableTab", ["NAME:PropServers", "ProjectVariables"], project_variables],
+                ]
+                self.oproject.ChangeProperty(command)
         return True
 
     @pyaedt_function_handler
     def read_only_variable(self, variable_name, value=True):
         """Set the variable to a read-only or not read-only variable.
 
         Parameters
```

### Comparing `pyaedt-0.6.71/pyaedt/application/JobManager.py` & `pyaedt-0.6.72/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/Variables.py` & `pyaedt-0.6.72/pyaedt/application/Variables.py`

 * *Files 3% similar despite different names*

```diff
@@ -575,54 +575,89 @@
         >>> oDesign.GetVariables
         >>> oProject.GetChildObject("Variables").GetChildNames
         >>> oDesign.GetChildObject("Variables").GetChildNames
         """
         return self._variable_dict([self._odesign, self._oproject], independent=False)
 
     @property
-    def variable_names(self):
-        """List of variables."""
-        return [var_name for var_name in self.variables]
+    def dependent_project_variables(self):
+        """Dependent project variables.
 
-    @property
-    def project_variable_names(self):
-        """List of project variables.
+        Returns
+        -------
+        dict
+            Dictionary of the dependent project variables available to the design.
 
         References
         ----------
 
         >>> oProject.GetVariables
         >>> oProject.GetChildObject("Variables").GetChildNames
         """
-        return [var_name for var_name in self.project_variables]
+        return self._variable_dict([self._oproject], independent=False)
 
     @property
-    def independent_project_variable_names(self):
-        """List of independent project variables.
+    def dependent_design_variables(self):
+        """Dependent design variables.
+
+        Returns
+        -------
+        dict
+            Dictionary of the dependent design properties (local
+            variables) available to the design.
+
+        References
+        ----------
+
+        >>> oDesign.GetVariables
+        >>> oDesign.GetChildObject("Variables").GetChildNames
+        """
+        return self._variable_dict([self._odesign], independent=False)
+
+    @property
+    def variable_names(self):
+        """List of variables."""
+        return [var_name for var_name in self.variables]
+
+    @property
+    def project_variable_names(self):
+        """List of project variables.
 
         References
         ----------
 
         >>> oProject.GetVariables
         >>> oProject.GetChildObject("Variables").GetChildNames
         """
-        return [var_name for var_name in self.independent_project_variables]
+        return [var_name for var_name in self.project_variables]
 
     @property
     def design_variable_names(self):
         """List of design variables.
 
         References
         ----------
 
         >>> oDesign.GetVariables
         >>> oDesign.GetChildObject("Variables").GetChildNames"""
         return [var_name for var_name in self.design_variables]
 
     @property
+    def independent_project_variable_names(self):
+        """List of independent project variables.
+
+        References
+        ----------
+
+        >>> oProject.GetVariables
+        >>> oProject.GetChildObject("Variables").GetChildNames
+        """
+        return [var_name for var_name in self.independent_project_variables]
+
+    @property
     def independent_design_variable_names(self):
         """List of independent design variables.
 
         References
         ----------
 
         >>> oDesign.GetVariables
@@ -639,14 +674,37 @@
         >>> oProject.GetVariables
         >>> oDesign.GetVariables
         >>> oProject.GetChildObject("Variables").GetChildNames
         >>> oDesign.GetChildObject("Variables").GetChildNames"""
         return [var_name for var_name in self.independent_variables]
 
     @property
+    def dependent_project_variable_names(self):
+        """List of dependent project variables.
+
+        References
+        ----------
+
+        >>> oProject.GetVariables
+        >>> oProject.GetChildObject("Variables").GetChildNames
+        """
+        return [var_name for var_name in self.dependent_project_variables]
+
+    @property
+    def dependent_design_variable_names(self):
+        """List of dependent design variables.
+
+        References
+        ----------
+
+        >>> oDesign.GetVariables
+        >>> oDesign.GetChildObject("Variables").GetChildNames"""
+        return [var_name for var_name in self.dependent_design_variables]
+
+    @property
     def dependent_variable_names(self):
         """List of dependent variables.
 
         References
         ----------
 
         >>> oProject.GetVariables
@@ -669,36 +727,71 @@
     def _logger(self):
         """Logger."""
         return self._app.logger
 
     def __init__(self, app):
         # Global Desktop Environment
         self._app = app
-        self._independent_variables = {}
-        self._dependent_variables = {}
+        self._independent_design_variables = {}
+        self._independent_project_variables = {}
+        self._dependent_design_variables = {}
+        self._dependent_project_variables = {}
+
+    @property
+    def _independent_variables(self):
+        all = {}
+        all.update(self._independent_project_variables)
+        all.update(self._independent_design_variables)
+        return all
+
+    @property
+    def _dependent_variables(self):
+        all = {}
+        for k, v in self._dependent_project_variables.items():
+            all[k] = v
+        for k, v in self._dependent_design_variables.items():
+            all[k] = v
+        return all
+
+    @property
+    def _all_variables(self):
+        all = {}
+        all.update(self._independent_variables)
+        all.update(self._dependent_variables)
+        return all
 
     @pyaedt_function_handler()
     def __delitem__(self, key):
         """Implement del with array name or index."""
         self.delete_variable(key)
-        if key in self._independent_variables:
-            del self._independent_variables[key]
-        if key in self._dependent_variables:
-            del self._dependent_variables[key]
 
     @pyaedt_function_handler()
     def __getitem__(self, variable_name):
         return self.variables[variable_name]
 
     @pyaedt_function_handler()
     def __setitem__(self, variable, value):
         self.set_variable(variable, value)
         return True
 
     @pyaedt_function_handler()
+    def _cleanup_variables(self):
+        variables = self._get_var_list_from_aedt(self._app.odesign) + self._get_var_list_from_aedt(self._app.oproject)
+        all_dicts = [
+            self._independent_project_variables,
+            self._independent_design_variables,
+            self._dependent_project_variables,
+            self._dependent_design_variables,
+        ]
+        for dict_var in all_dicts:
+            for var_name in list(dict_var.keys()):
+                if var_name not in variables:
+                    del dict_var[var_name]
+
+    @pyaedt_function_handler()
     def _variable_dict(self, object_list, dependent=True, independent=True):
         """Retrieve the variable dictionary.
 
         Parameters
         ----------
         object_list : list
             List of objects.
@@ -711,49 +804,47 @@
         -------
         dict
             Dictionary of the specified variables.
 
         """
         all_names = {}
         for obj in object_list:
-            variables = self._get_var_list_from_aedt(obj)
+            variables = [i for i in self._get_var_list_from_aedt(obj) if i not in list(self._all_variables.keys())]
             for variable_name in variables:
-                if independent and variable_name not in self._independent_variables:
-                    if self.get_expression(variable_name):
-                        variable_expression = self.get_expression(variable_name)
-                        all_names[variable_name] = variable_expression
-                        si_value = self._app.get_evaluated_value(variable_name)
-                        value = Variable(
-                            variable_expression, None, si_value, all_names, name=variable_name, app=self._app
-                        )
-                        is_number_flag = is_number(value._calculated_value)
-                        if is_number_flag:
-                            self._independent_variables[variable_name] = value
-
-                        elif dependent and not is_number_flag:
-                            self._dependent_variables[variable_name] = value
-                elif dependent and variable_name not in self._dependent_variables:
-                    if self.get_expression(variable_name):
-                        variable_expression = self.get_expression(variable_name)
-                        all_names[variable_name] = variable_expression
-                        si_value = self._app.get_evaluated_value(variable_name)
-                        value = Variable(
-                            variable_expression, None, si_value, all_names, name=variable_name, app=self._app
-                        )
-                        is_number_flag = is_number(value._calculated_value)
-                        if not is_number_flag:
-                            self._dependent_variables[variable_name] = value
+                variable_expression = self.get_expression(variable_name)
+                if variable_expression:
+                    all_names[variable_name] = variable_expression
+                    si_value = self._app.get_evaluated_value(variable_name)
+                    value = Variable(variable_expression, None, si_value, all_names, name=variable_name, app=self._app)
+                    is_number_flag = is_number(value._calculated_value)
+                    if variable_name.startswith("$") and is_number_flag:
+                        self._independent_project_variables[variable_name] = value
+                    elif variable_name.startswith("$"):
+                        self._dependent_project_variables[variable_name] = value
+                    elif is_number_flag:
+                        self._independent_design_variables[variable_name] = value
+                    else:
+                        self._dependent_design_variables[variable_name] = value
+        self._cleanup_variables()
+        vars_to_output = {}
+        dicts_to_add = []
         if independent:
-            vars = self._independent_variables.copy()
-        else:
-            vars = {}
+            if self._app.odesign in object_list:
+                dicts_to_add.append(self._independent_design_variables)
+            if self._app.oproject in object_list:
+                dicts_to_add.append(self._independent_project_variables)
         if dependent:
-            for k, v in self._dependent_variables.items():
-                vars[k] = v
-        return vars
+            if self._app.odesign in object_list:
+                dicts_to_add.append(self._dependent_design_variables)
+            if self._app.oproject in object_list:
+                dicts_to_add.append(self._dependent_project_variables)
+        for dict_var in dicts_to_add:
+            for k, v in dict_var.items():
+                vars_to_output[k] = v
+        return vars_to_output
 
     @pyaedt_function_handler()
     def get_expression(self, variable_name):  # TODO: Should be renamed to "evaluate"
         """Retrieve the variable value of a project or design variable as a string.
 
         References
         ----------
@@ -861,16 +952,24 @@
         creating the variable if it does not exist.
 
         >>> aedtapp.variable_manager.set_variable["$p1"] == "30mm"
 
         """
         if variable_name in self._independent_variables:
             del self._independent_variables[variable_name]
+            if variable_name in self._independent_design_variables:
+                del self._independent_design_variables[variable_name]
+            elif variable_name in self._independent_project_variables:
+                del self._independent_project_variables[variable_name]
         elif variable_name in self._dependent_variables:
             del self._dependent_variables[variable_name]
+            if variable_name in self._dependent_design_variables:
+                del self._dependent_design_variables[variable_name]
+            elif variable_name in self._dependent_project_variables:
+                del self._dependent_project_variables[variable_name]
         if not description:
             description = ""
 
         desktop_object = self.aedt_object(variable_name)
         if variable_name.startswith("$"):
             tab_name = "ProjectVariableTab"
             prop_server = "ProjectVariables"
@@ -994,15 +1093,15 @@
                                 "Hidden:=",
                                 hidden,
                             ],
                         ],
                     ],
                 ]
             )
-            self._clean_variable_from_dicts(variable_name)
+            self._cleanup_variables()
         var_list = self._get_var_list_from_aedt(desktop_object)
         lower_case_vars = [var_name.lower() for var_name in var_list]
         if variable_name.lower() not in lower_case_vars:
             return False
         return True
 
     @pyaedt_function_handler()
@@ -1082,26 +1181,19 @@
                             ["NAME:DeletedProps", var_name],
                         ],
                     ]
                 )
             except:  # pragma: no cover
                 pass
             else:
-                self._clean_variable_from_dicts(var_name)
+                self._cleanup_variables()
                 return True
         return False
 
     @pyaedt_function_handler()
-    def _clean_variable_from_dicts(self, variable_name):
-        if variable_name in self._dependent_variables:
-            del self._dependent_variables[variable_name]
-        if variable_name in self._independent_variables:
-            del self._independent_variables[variable_name]
-
-    @pyaedt_function_handler()
     def _get_var_list_from_aedt(self, desktop_object):
         var_list = []
         if self._app._is_object_oriented_enabled() and self._app.design_type != "Maxwell Circuit":
             # To retrieve local variables
             var_list += list(self._app.get_oo_object(self._app.odesign, "LocalVariables").GetPropNames())
         if self._app._is_object_oriented_enabled() and self._app.design_type in [
             "Circuit Design",
```

### Comparing `pyaedt-0.6.71/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.72/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/application/design_solutions.py` & `pyaedt-0.6.72/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/circuit.py` & `pyaedt-0.6.72/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/common_rpc.py` & `pyaedt-0.6.72/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/desktop.py` & `pyaedt-0.6.72/pyaedt/desktop.py`

 * *Files 1% similar despite different names*

```diff
@@ -569,14 +569,15 @@
         if not settings.remote_api:
             self._logger.info("Python version %s", sys.version)
         self.odesktop = self._main.oDesktop
         settings.aedt_version = self.odesktop.GetVersion()[0:6]
         settings.machine = self.machine
         settings.port = self.port
         self.aedt_process_id = self.odesktop.GetProcessID()  # bit of cleanup for consistency if used in future
+        self._logger.info("AEDT %s Build Date %s", self.odesktop.GetVersion(), self.odesktop.GetBuildDateTimeString())
 
         if _com == "ironpython":
             sys.path.append(
                 os.path.join(self._main.sDesktopinstallDirectory, "common", "commonfiles", "IronPython", "DLLs")
             )
 
     def __enter__(self):
@@ -686,18 +687,19 @@
         return ""
 
     def _init_desktop(self, non_graphical):
         self._main.AEDTVersion = self._main.oDesktop.GetVersion()[0:6]
         self._main.oDesktop.RestoreWindow()
         self._main.sDesktopinstallDirectory = self._main.oDesktop.GetExeDir()
         self._main.pyaedt_initialized = True
-        try:
-            settings.enable_desktop_logs = not self._main.oDesktop.GetIsNonGraphical()
-        except AttributeError:
-            settings.enable_desktop_logs = not non_graphical
+        if non_graphical or self._main.oDesktop.GetIsNonGraphical():
+            try:
+                settings.enable_desktop_logs = not self._main.oDesktop.GetIsNonGraphical()
+            except AttributeError:
+                settings.enable_desktop_logs = not non_graphical
 
     def _set_version(self, specified_version, student_version):
         student_version_flag = False
         if specified_version:
             if float(specified_version) < 2021:
                 if float(specified_version) < 2019:
                     raise ValueError("PyAEDT supports AEDT version 2021 R1 and later.")
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files 18% similar despite different names*

#### pedump {}

```diff
@@ -1,38 +1,38 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xdbb7c852
+	             Time stamp: 0xc47ba9d4
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
 	              Code Size: 0x00005400
 	  Initialized Data Size: 0x00000600
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x00007332
+	        Entry Point RVA: 0x0000730a
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x00008000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
-	  	Subsys major (4): 0x0006
+	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x0000c000
 	 	     Header Size: 0x00000200
 	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
@@ -41,42 +41,42 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000072df [0x0000004f]
-	   Resource Table: 0x00008000 [0x00000388]
+	     Import Table: 0x000072b5 [0x0000004f]
+	   Resource Table: 0x00008000 [0x00000330]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0000a000 [0x0000000c]
-	            Debug: 0x00007250 [0x00000038]
+	            Debug: 0x000071c8 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x00005338
+	   Virtual Size: 0x00005310
 	Virtual Address: 0x00002000
 	  Raw Data Size: 0x00005400
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x00000388
+	   Virtual Size: 0x00000330
 	Virtual Address: 0x00008000
 	  Raw Data Size: 0x00000400
 	   Raw Data Ptr: 0x00005600
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
@@ -92,15 +92,15 @@
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x000040c8 [0x00003188]
+	         Metadata: 0x00003fb0 [0x00003218]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
@@ -109,31 +109,31 @@
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x000012d4 [4712 == 0x00001268]
-	    Strings: 0x000012d4 - 0x00002758 [5252 == 0x00001484]
-	       Blob: 0x00002b54 - 0x00003188 [1588 == 0x00000634]
-	User string: 0x00002758 - 0x00002b44 [1004 == 0x000003ec]
-	       GUID: 0x00002b44 - 0x00002b54 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00001330 [4804 == 0x000012c4]
+	    Strings: 0x00001330 - 0x00002864 [5428 == 0x00001534]
+	       Blob: 0x00002c30 - 0x00003218 [1512 == 0x000005e8]
+	User string: 0x00002864 - 0x00002c20 [956 == 0x000003bc]
+	       GUID: 0x00002c20 - 0x00002c30 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at 2394)
-Table TypeRef: 111 records (6 bytes, at 239e)
-Table TypeDef: 6 records (14 bytes, at 2638)
-Table Field: 65 records (6 bytes, at 268c)
-Table Method: 60 records (14 bytes, at 2812)
-Table Param: 83 records (6 bytes, at 2b5a)
-Table MemberRef: 215 records (6 bytes, at 2d4c)
-Table Constant: 26 records (6 bytes, at 3256)
-Table CustomAttribute: 42 records (6 bytes, at 32f2)
-Table StandaloneSig: 17 records (2 bytes, at 33ee)
-Table PropertyMap: 3 records (4 bytes, at 3410)
-Table Property: 10 records (6 bytes, at 341c)
-Table MethodSemantics: 20 records (6 bytes, at 3458)
-Table TypeSpec: 11 records (2 bytes, at 34d0)
-Table Assembly: 1 records (22 bytes, at 34e6)
-Table AssemblyRef: 7 records (20 bytes, at 34fc)
-Table NestedClass: 1 records (4 bytes, at 3588)
-Table MethodSpec: 3 records (4 bytes, at 358c)
+Table Module: 1 records (10 bytes, at 227c)
+Table TypeRef: 112 records (6 bytes, at 2286)
+Table TypeDef: 6 records (14 bytes, at 2526)
+Table Field: 66 records (6 bytes, at 257a)
+Table Method: 59 records (14 bytes, at 2706)
+Table Param: 75 records (6 bytes, at 2a40)
+Table MemberRef: 213 records (6 bytes, at 2c02)
+Table Constant: 24 records (6 bytes, at 3100)
+Table CustomAttribute: 44 records (6 bytes, at 3190)
+Table StandaloneSig: 14 records (2 bytes, at 3298)
+Table PropertyMap: 3 records (4 bytes, at 32b4)
+Table Property: 12 records (6 bytes, at 32c0)
+Table MethodSemantics: 24 records (6 bytes, at 3308)
+Table TypeSpec: 13 records (2 bytes, at 3398)
+Table Assembly: 1 records (22 bytes, at 33b2)
+Table AssemblyRef: 13 records (20 bytes, at 33c8)
+Table NestedClass: 1 records (4 bytes, at 34cc)
+Table MethodSpec: 3 records (4 bytes, at 34d0)
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9868421052631579%*

 * *Differences: {"'BottomMarginCover'": '1.9'}*

```diff
@@ -1,10 +1,10 @@
 {
     "BottomMargin": 2.0,
-    "BottomMarginCover": 2.0,
+    "BottomMarginCover": 1.9,
     "CaptionFontSize": 9,
     "ChartHeight": 12,
     "ChartWidth": 16,
     "CoverSpaceAfter": 0.5,
     "CoverSubTitleFontSize": 24,
     "CoverSubTitleSpaceAfter": 0.3,
     "CoverTitleFontSize": 28,
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.DocumentObjectModel-gdi.dll` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files 17% similar despite different names*

#### pedump {}

```diff
@@ -1,162 +1,142 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x5c583c6f
+	             Time stamp: 0x8b85be39
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x0003a000
-	  Initialized Data Size: 0x00002000
+	              Code Size: 0x00039a00
+	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0003b5be
+	        Entry Point RVA: 0x0003b9ce
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x0003c000
 
 
 NT Header:
-	   Image Base (0x400000): 0x11000000
+	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
-	   File Align (512/4096): 0x00001000
+	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x00040000
-	 	     Header Size: 0x00001000
-	            Checksum (0): 0x00045950
+	 	     Header Size: 0x00000200
+	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
-	           DLL Flags (0): 0x8540
+	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0003b56c [0x0000004f]
-	   Resource Table: 0x0003c000 [0x000004d4]
+	     Import Table: 0x0003b97b [0x0000004f]
+	   Resource Table: 0x0003c000 [0x00000588]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x0003e000 [0x0000000c]
-	            Debug: 0x00000000 [0x00000000]
+	            Debug: 0x0003b86c [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000395c4
+	   Virtual Size: 0x000399d4
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x0003a000
-	   Raw Data Ptr: 0x00001000
+	  Raw Data Size: 0x00039a00
+	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004d4
+	   Virtual Size: 0x00000588
 	Virtual Address: 0x0003c000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0003b000
+	  Raw Data Size: 0x00000600
+	   Raw Data Ptr: 0x00039c00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x0003e000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0003c000
+	  Raw Data Size: 0x00000200
+	   Raw Data Ptr: 0x0003a200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
-                    Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x0001c624 [0x0001db70]
+                    Flags: ilonly, 32/64, no-trackdebug, notsigned
+	         Metadata: 0x0001cc8c [0x0001d820]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0003a194 [0x00001358]
-	   Strong Name at: 0x0003b4ec [0x00000080]
+	     Resources at: 0x0003a4ac [0x000013c0]
+	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
-Strong name:
-	 DF 6D 5C DB FF 3E A3 A3 E3 6F 47 2D 7C 32 36 DC
-	 E8 46 8A 86 E6 FB 54 B4 67 3C 6B D9 FD 57 80 D0
-	 C4 3A AC EA 85 3A 19 7B E4 69 4B 7A 24 89 16 1A
-	 E5 57 0D 05 64 14 CB 34 D1 91 FE 98 A7 DA 16 3A
-	 B4 56 5C 7B 29 8E 51 87 4E 39 80 6D 2C 90 8E 36
-	 BB 20 6C 04 BD E0 10 6C 1E 70 E9 82 B5 36 36 F8
-	 FA C3 28 E7 D6 3A B9 A0 37 4F 49 30 D9 04 A9 F1
-	 61 49 11 75 B6 0D A4 72 82 1A 6F BD B1 3D 25 66
-
-Public key:
-	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
-	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
-	 87 94 E8 03 E5 66 EC CC 3C 91 81 F5 2C 4F 70 44
-	 E5 44 2C C2 CE 3C BB A9 FC 11 BC 41 86 BA 2E 44
-	 6C D3 1D EE A2 0C 1A 8F 49 9E 97 84 17 FA D2 BC
-	 74 14 3A 4F 83 98 F7 CF 5C 5C 02 71 B0 F7 FE 90
-	 7C 53 7C FF 28 B9 D5 82 DA 41 28 9D 1D AE 90 16
-	 8A 3D A2 A5 ED 11 15 21 0A 18 FD AE 83 24 79 D3
-	 E6 39 CA 40 03 28 6B A8 B9 8D C9 14 46 15 C0 40
-	 ED 83 89 81 AC 81 61 12 DF 3B 5A 9E 7C AB 4F BB
+Strong name: none
+
+Public key: none
 
 Metadata header:
            Version: 1.1
-    Version string: v2.0.50727
+    Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00010bac [68416 == 0x00010b40]
-	    Strings: 0x00010bac - 0x00016bdc [24624 == 0x00006030]
-	       Blob: 0x00019684 - 0x0001db70 [17644 == 0x000044ec]
-	User string: 0x00016bdc - 0x00019674 [10904 == 0x00002a98]
-	       GUID: 0x00019674 - 0x00019684 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00010f44 [69336 == 0x00010ed8]
+	    Strings: 0x00010f44 - 0x00017064 [24864 == 0x00006120]
+	       Blob: 0x0001a234 - 0x0001d820 [13804 == 0x000035ec]
+	User string: 0x00017064 - 0x0001a224 [12736 == 0x000031c0]
+	       GUID: 0x0001a224 - 0x0001a234 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at 1b704)
-Table TypeRef: 90 records (6 bytes, at 1b70e)
-Table TypeDef: 170 records (14 bytes, at 1b92a)
-Table Field: 1361 records (6 bytes, at 1c276)
-Table Method: 2111 records (14 bytes, at 1e25c)
-Table Param: 1515 records (6 bytes, at 255ce)
-Table InterfaceImpl: 41 records (4 bytes, at 27950)
-Table MemberRef: 248 records (6 bytes, at 279f4)
-Table Constant: 654 records (6 bytes, at 27fc4)
-Table CustomAttribute: 386 records (8 bytes, at 28f18)
-Table StandaloneSig: 219 records (2 bytes, at 29b28)
-Table PropertyMap: 94 records (4 bytes, at 29cde)
-Table Property: 542 records (6 bytes, at 29e56)
-Table MethodSemantics: 886 records (6 bytes, at 2ab0a)
-Table MethodImpl: 63 records (6 bytes, at 2bfce)
-Table TypeSpec: 21 records (2 bytes, at 2c148)
-Table Assembly: 1 records (22 bytes, at 2c172)
-Table AssemblyRef: 1 records (20 bytes, at 2c188)
-Table ManifestResource: 1 records (12 bytes, at 2c19c)
-Table NestedClass: 2 records (4 bytes, at 2c1a8)
-Table GenericParam: 1 records (8 bytes, at 2c1b0)
-Table MethodSpec: 4 records (4 bytes, at 2c1b8)
-Table GenericParamConstraint: 1 records (4 bytes, at 2c1c8)
+Table Module: 1 records (10 bytes, at 1af64)
+Table TypeRef: 109 records (6 bytes, at 1af6e)
+Table TypeDef: 171 records (14 bytes, at 1b1fc)
+Table Field: 1349 records (6 bytes, at 1bb56)
+Table Method: 2151 records (14 bytes, at 1daf4)
+Table Param: 1479 records (6 bytes, at 25096)
+Table InterfaceImpl: 43 records (4 bytes, at 27340)
+Table MemberRef: 254 records (6 bytes, at 273ec)
+Table Constant: 638 records (6 bytes, at 279e0)
+Table CustomAttribute: 383 records (8 bytes, at 288d4)
+Table StandaloneSig: 207 records (2 bytes, at 294cc)
+Table PropertyMap: 96 records (4 bytes, at 2966a)
+Table Property: 594 records (6 bytes, at 297ea)
+Table MethodSemantics: 937 records (6 bytes, at 2a5d6)
+Table MethodImpl: 64 records (6 bytes, at 2bbcc)
+Table TypeSpec: 8 records (2 bytes, at 2bd4c)
+Table Assembly: 1 records (22 bytes, at 2bd5c)
+Table AssemblyRef: 2 records (20 bytes, at 2bd72)
+Table ManifestResource: 1 records (12 bytes, at 2bd9a)
+Table NestedClass: 4 records (4 bytes, at 2bda6)
+Table MethodSpec: 6 records (4 bytes, at 2bdb6)
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/MigraDoc.Rendering-gdi.dll` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files 20% similar despite different names*

#### pedump {}

```diff
@@ -1,164 +1,146 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x5c583c72
+	             Time stamp: 0xbc36bcfe
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x0001d000
-	  Initialized Data Size: 0x00002000
+	              Code Size: 0x0001ba00
+	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0001ec76
+	        Entry Point RVA: 0x0001d82e
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x00020000
+		  Data Base RVA: 0x0001e000
 
 
 NT Header:
-	   Image Base (0x400000): 0x11000000
+	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
-	   File Align (512/4096): 0x00001000
+	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x00024000
-	 	     Header Size: 0x00001000
-	            Checksum (0): 0x0002a4f7
+	 	      Image Size: 0x00022000
+	 	     Header Size: 0x00000200
+	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
-	           DLL Flags (0): 0x8540
+	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0001ec24 [0x0000004f]
-	   Resource Table: 0x00020000 [0x00000498]
+	     Import Table: 0x0001d7da [0x0000004f]
+	   Resource Table: 0x0001e000 [0x00000510]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x00022000 [0x0000000c]
-	            Debug: 0x00000000 [0x00000000]
+	      Reloc Table: 0x00020000 [0x0000000c]
+	            Debug: 0x0001d6e0 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x0001cd14
+	   Virtual Size: 0x0001b86c
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x0001d000
-	   Raw Data Ptr: 0x00001000
+	  Raw Data Size: 0x0001ba00
+	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x00000498
-	Virtual Address: 0x00020000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0001e000
+	   Virtual Size: 0x00000510
+	Virtual Address: 0x0001e000
+	  Raw Data Size: 0x00000600
+	   Raw Data Ptr: 0x0001bc00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x00022000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0001f000
+	Virtual Address: 0x00020000
+	  Raw Data Size: 0x00000200
+	   Raw Data Ptr: 0x0001c200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
-                    Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x0001055c [0x0000daf0]
+                    Flags: ilonly, 32/64, no-trackdebug, notsigned
+	         Metadata: 0x000100dc [0x0000d0ac]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0001e04c [0x00000b58]
-	   Strong Name at: 0x0001eba4 [0x00000080]
+	     Resources at: 0x0001d188 [0x00000558]
+	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
-Strong name:
-	 54 D4 A4 F0 0C 07 92 6A 23 C5 93 A3 A5 56 92 B7
-	 86 3B B1 3B 3D DF 1E 25 5A 44 39 7E 46 A1 B0 6A
-	 F0 6A 39 3B EA E2 70 73 0C C1 DC 9A 4A 07 52 E7
-	 72 CC CB 02 D9 DD 84 BE 7A 7E 08 F7 81 7E 76 DF
-	 1D A7 D9 AA CF EE D1 5F 15 48 10 5B D0 04 8D B2
-	 D7 DD 8B BE FA 29 6F 8B F6 97 F5 35 C1 C7 C8 89
-	 16 D1 CD D5 59 CA 4A D9 C5 C8 FD 4C F0 CA 5C 0E
-	 BF 37 95 99 2A F5 58 D7 E2 16 1F EA 27 2F E2 18
-
-Public key:
-	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
-	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
-	 87 94 E8 03 E5 66 EC CC 3C 91 81 F5 2C 4F 70 44
-	 E5 44 2C C2 CE 3C BB A9 FC 11 BC 41 86 BA 2E 44
-	 6C D3 1D EE A2 0C 1A 8F 49 9E 97 84 17 FA D2 BC
-	 74 14 3A 4F 83 98 F7 CF 5C 5C 02 71 B0 F7 FE 90
-	 7C 53 7C FF 28 B9 D5 82 DA 41 28 9D 1D AE 90 16
-	 8A 3D A2 A5 ED 11 15 21 0A 18 FD AE 83 24 79 D3
-	 E6 39 CA 40 03 28 6B A8 B9 8D C9 14 46 15 C0 40
-	 ED 83 89 81 AC 81 61 12 DF 3B 5A 9E 7C AB 4F BB
+Strong name: none
+
+Public key: none
 
 Metadata header:
            Version: 1.1
-    Version string: v2.0.50727
+    Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x000066d4 [26216 == 0x00006668]
-	    Strings: 0x000066d4 - 0x0000b28c [19384 == 0x00004bb8]
-	       Blob: 0x0000bb18 - 0x0000daf0 [8152 == 0x00001fd8]
-	User string: 0x0000b28c - 0x0000bb08 [2172 == 0x0000087c]
-	       GUID: 0x0000bb08 - 0x0000bb18 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00005e4c [24032 == 0x00005de0]
+	    Strings: 0x00005e4c - 0x0000a728 [18652 == 0x000048dc]
+	       Blob: 0x0000b614 - 0x0000d0ac [6808 == 0x00001a98]
+	User string: 0x0000a728 - 0x0000b604 [3804 == 0x00000edc]
+	       GUID: 0x0000b604 - 0x0000b614 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at f644)
-Table TypeRef: 261 records (6 bytes, at f64e)
-Table TypeDef: 82 records (14 bytes, at fc6c)
-Table Field: 346 records (6 bytes, at 100e8)
-Table Method: 675 records (14 bytes, at 10904)
-Table Param: 588 records (6 bytes, at 12dee)
-Table InterfaceImpl: 5 records (4 bytes, at 13bb6)
-Table MemberRef: 707 records (6 bytes, at 13bca)
-Table Constant: 77 records (6 bytes, at 14c5c)
-Table CustomAttribute: 49 records (6 bytes, at 14e2a)
-Table ClassLayout: 2 records (8 bytes, at 14f50)
-Table StandaloneSig: 195 records (2 bytes, at 14f60)
-Table EventMap: 2 records (4 bytes, at 150e6)
-Table Event: 3 records (6 bytes, at 150ee)
-Table PropertyMap: 35 records (4 bytes, at 15100)
-Table Property: 153 records (6 bytes, at 1518c)
-Table MethodSemantics: 216 records (6 bytes, at 15522)
-Table MethodImpl: 35 records (6 bytes, at 15a32)
-Table TypeSpec: 20 records (2 bytes, at 15b04)
-Table FieldRVA: 2 records (6 bytes, at 15b2c)
-Table Assembly: 1 records (22 bytes, at 15b38)
-Table AssemblyRef: 7 records (20 bytes, at 15b4e)
-Table ManifestResource: 3 records (12 bytes, at 15bda)
-Table NestedClass: 10 records (4 bytes, at 15bfe)
-Table MethodSpec: 2 records (4 bytes, at 15c26)
+Table Module: 1 records (10 bytes, at e3c4)
+Table TypeRef: 246 records (6 bytes, at e3ce)
+Table TypeDef: 81 records (14 bytes, at e992)
+Table Field: 294 records (6 bytes, at ee00)
+Table Method: 637 records (14 bytes, at f4e4)
+Table Param: 538 records (6 bytes, at 117ba)
+Table InterfaceImpl: 5 records (4 bytes, at 12456)
+Table MemberRef: 643 records (6 bytes, at 1246a)
+Table Constant: 39 records (6 bytes, at 1337c)
+Table CustomAttribute: 29 records (6 bytes, at 13466)
+Table ClassLayout: 1 records (8 bytes, at 13514)
+Table StandaloneSig: 186 records (2 bytes, at 1351c)
+Table EventMap: 1 records (4 bytes, at 13690)
+Table Event: 1 records (6 bytes, at 13694)
+Table PropertyMap: 35 records (4 bytes, at 1369a)
+Table Property: 150 records (6 bytes, at 13726)
+Table MethodSemantics: 190 records (6 bytes, at 13aaa)
+Table MethodImpl: 35 records (6 bytes, at 13f1e)
+Table TypeSpec: 7 records (2 bytes, at 13ff0)
+Table FieldRVA: 1 records (6 bytes, at 13ffe)
+Table Assembly: 1 records (22 bytes, at 14004)
+Table AssemblyRef: 11 records (20 bytes, at 1401a)
+Table ManifestResource: 1 records (12 bytes, at 140f6)
+Table NestedClass: 8 records (4 bytes, at 14102)
+Table MethodSpec: 1 records (4 bytes, at 14122)
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files 12% similar despite different names*

#### pedump {}

```diff
@@ -1,122 +1,122 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0xdff1c7f1
+	             Time stamp: 0x8be79041
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x000a8600
+	              Code Size: 0x000a8a00
 	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000aa1de
+	        Entry Point RVA: 0x000aa672
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x000ac000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
 	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
-	  	Subsys major (4): 0x0006
+	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
 	 	      Image Size: 0x000b0000
 	 	     Header Size: 0x00000200
-	            Checksum (0): 0x000b2a66
+	            Checksum (0): 0x000b91f9
 	               Subsystem: 0x0003
 	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000aa18c [0x0000004f]
-	   Resource Table: 0x000ac000 [0x000004a4]
+	     Import Table: 0x000aa61d [0x0000004f]
+	   Resource Table: 0x000ac000 [0x000004c8]
 	  Exception Table: 0x00000000 [0x00000000]
-	Certificate Table: 0x000a9000 [0x00001fb0]
+	Certificate Table: 0x000a9400 [0x00002f10]
 	      Reloc Table: 0x000ae000 [0x0000000c]
-	            Debug: 0x000aa0bc [0x00000054]
+	            Debug: 0x000aa544 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000a84ac
+	   Virtual Size: 0x000a8940
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x000a8600
+	  Raw Data Size: 0x000a8a00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x000004a4
+	   Virtual Size: 0x000004c8
 	Virtual Address: 0x000ac000
 	  Raw Data Size: 0x00000600
-	   Raw Data Ptr: 0x000a8800
+	   Raw Data Ptr: 0x000a8c00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x000ae000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x000a8e00
+	   Raw Data Ptr: 0x000a9200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x00047a00 [0x0006263c]
+	         Metadata: 0x000479c0 [0x00062b04]
 	Entry Point Token: 0x00000000
 	     Resources at: 0x00000000 [0x00000000]
-	   Strong Name at: 0x000aa03c [0x00000080]
+	   Strong Name at: 0x000aa4c4 [0x00000080]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name:
-	 7F F4 85 D3 8D F8 DA 29 5A F4 F9 18 84 56 FC 62
-	 D1 65 00 D6 71 B3 3A 72 BE BB 6A 00 FC 18 E9 E2
-	 07 91 D2 A6 10 2D 69 6F 0A E1 FA 27 E6 A7 D1 72
-	 5E DE 0F 6F 44 3D 8E 88 44 4A 20 4C F4 D2 6D 01
-	 5C E5 79 E8 1E 7D 3D 01 85 5A 27 8C E2 0C F2 4F
-	 B8 95 8D 6D 28 A1 1B A9 81 D7 B8 F1 A9 7B 9F CD
-	 16 36 C9 50 FB 02 52 5F C5 EE 59 3C 51 2D 8A C5
-	 A1 3B 46 7A 29 78 85 1F D0 45 2B C4 A0 C0 F1 97
+	 7C 63 D9 BA 6D D9 4E 50 D1 39 3F C7 B5 CC 62 DD
+	 79 87 5B BC 9C 61 B6 A6 FF BE CD 4D CE 07 FF 6D
+	 92 FF B3 EE 8F B5 85 6E 72 7A 40 C0 1F 4A D7 E8
+	 6B A0 A5 19 E8 9F 8D 66 0B 97 9D D2 7A 0A 91 6C
+	 39 1C B3 BB 58 E6 DA 61 96 FD 01 54 E7 95 77 E9
+	 8B B2 54 D1 8C 67 8C 07 F2 2A E3 87 39 17 71 43
+	 AE 35 0B 4F CC E4 27 22 49 88 F6 2E 55 8E F1 83
+	 A2 95 C3 22 75 3D DD 92 8D F8 39 F7 90 BA 6D 4C
 
 Public key:
 	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
 	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
 	 F5 61 DF 27 7C 6C 0B 49 7D 62 90 32 B4 10 CD CF
 	 28 6E 53 7C 05 47 24 F7 FF A0 16 43 45 F6 2B 3E
 	 64 20 29 D7 A8 0C C3 51 91 89 55 32 8C 4A DC 8A
@@ -127,39 +127,39 @@
 	 93 0F 32 10 3F BE 1D 29 11 42 5B C5 74 40 02 C7
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x00033eec [212608 == 0x00033e80]
-	    Strings: 0x00033eec - 0x000468ac [76224 == 0x000129c0]
-	       Blob: 0x000546b0 - 0x0006263c [57228 == 0x0000df8c]
-	User string: 0x000468ac - 0x000546a0 [56820 == 0x0000ddf4]
-	       GUID: 0x000546a0 - 0x000546b0 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00034228 [213436 == 0x000341bc]
+	    Strings: 0x00034228 - 0x00046d8c [76644 == 0x00012b64]
+	       Blob: 0x00054c88 - 0x00062b04 [56956 == 0x0000de7c]
+	User string: 0x00046d8c - 0x00054c78 [57068 == 0x0000deec]
+	       GUID: 0x00054c78 - 0x00054c88 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 45cec)
-Table TypeRef: 352 records (10 bytes, at 45cf8)
-Table TypeDef: 496 records (18 bytes, at 46ab8)
-Table Field: 2160 records (8 bytes, at 48d98)
-Table Method: 4176 records (16 bytes, at 4d118)
-Table Param: 4761 records (8 bytes, at 5d618)
-Table InterfaceImpl: 291 records (4 bytes, at 66ae0)
-Table MemberRef: 2119 records (8 bytes, at 66f6c)
-Table Constant: 565 records (6 bytes, at 6b1a4)
-Table CustomAttribute: 4208 records (8 bytes, at 6bee2)
-Table ClassLayout: 10 records (8 bytes, at 74262)
-Table StandaloneSig: 751 records (2 bytes, at 742b2)
-Table EventMap: 5 records (4 bytes, at 74890)
-Table Event: 8 records (8 bytes, at 748a4)
-Table PropertyMap: 145 records (4 bytes, at 748e4)
-Table Property: 703 records (8 bytes, at 74b28)
-Table MethodSemantics: 1098 records (6 bytes, at 76120)
-Table MethodImpl: 438 records (6 bytes, at 77adc)
-Table TypeSpec: 482 records (2 bytes, at 78520)
-Table FieldRVA: 22 records (6 bytes, at 788e4)
-Table Assembly: 1 records (26 bytes, at 78968)
-Table AssemblyRef: 8 records (24 bytes, at 78982)
-Table NestedClass: 222 records (4 bytes, at 78a42)
-Table GenericParam: 158 records (10 bytes, at 78dba)
-Table MethodSpec: 418 records (4 bytes, at 793e6)
-Table GenericParamConstraint: 31 records (4 bytes, at 79a6e)
+Table Module: 1 records (12 bytes, at 45cac)
+Table TypeRef: 342 records (10 bytes, at 45cb8)
+Table TypeDef: 496 records (18 bytes, at 46a14)
+Table Field: 2196 records (8 bytes, at 48cf4)
+Table Method: 4185 records (16 bytes, at 4d194)
+Table Param: 4778 records (8 bytes, at 5d724)
+Table InterfaceImpl: 291 records (4 bytes, at 66c74)
+Table MemberRef: 2068 records (8 bytes, at 67100)
+Table Constant: 568 records (6 bytes, at 6b1a0)
+Table CustomAttribute: 4316 records (8 bytes, at 6bef0)
+Table ClassLayout: 10 records (8 bytes, at 745d0)
+Table StandaloneSig: 753 records (2 bytes, at 74620)
+Table EventMap: 5 records (4 bytes, at 74c02)
+Table Event: 8 records (8 bytes, at 74c16)
+Table PropertyMap: 147 records (4 bytes, at 74c56)
+Table Property: 706 records (8 bytes, at 74ea2)
+Table MethodSemantics: 1105 records (6 bytes, at 764b2)
+Table MethodImpl: 440 records (6 bytes, at 77e98)
+Table TypeSpec: 480 records (2 bytes, at 788e8)
+Table FieldRVA: 22 records (6 bytes, at 78ca8)
+Table Assembly: 1 records (26 bytes, at 78d2c)
+Table AssemblyRef: 1 records (24 bytes, at 78d46)
+Table NestedClass: 222 records (4 bytes, at 78d5e)
+Table GenericParam: 151 records (10 bytes, at 790d6)
+Table MethodSpec: 427 records (4 bytes, at 796bc)
+Table GenericParamConstraint: 31 records (4 bytes, at 79d68)
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files 1% similar despite different names*

#### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

```diff
@@ -1239,14 +1239,50 @@
     <member name="T:Newtonsoft.Json.Converters.UnixDateTimeConverter">
       <summary>
         Converts a
         <see cref="T:System.DateTime"/>
         to and from Unix epoch time
       </summary>
     </member>
+    <member name="P:Newtonsoft.Json.Converters.UnixDateTimeConverter.AllowPreEpoch">
+      <summary>Gets or sets a value indicating whether the dates before Unix epoch
+            should converted to and from JSON.</summary>
+      <value>
+        <c>true</c>
+        to allow converting dates before Unix epoch to and from JSON;
+        <c>false</c>
+        to throw an exception when a date being converted to or from JSON
+            occurred before Unix epoch. The default value is
+        <c>false</c>
+        .
+      </value>
+    </member>
+    <member name="M:Newtonsoft.Json.Converters.UnixDateTimeConverter.#ctor">
+      <summary>
+        Initializes a new instance of the
+        <see cref="T:Newtonsoft.Json.Converters.UnixDateTimeConverter"/>
+        class.
+      </summary>
+    </member>
+    <member name="M:Newtonsoft.Json.Converters.UnixDateTimeConverter.#ctor(System.Boolean)">
+      <summary>
+        Initializes a new instance of the
+        <see cref="T:Newtonsoft.Json.Converters.UnixDateTimeConverter"/>
+        class.
+      </summary>
+      <param name="allowPreEpoch">
+        <c>true</c>
+        to allow converting dates before Unix epoch to and from JSON;
+        <c>false</c>
+        to throw an exception when a date being converted to or from JSON
+            occurred before Unix epoch. The default value is
+        <c>false</c>
+        .
+      </param>
+    </member>
     <member name="M:Newtonsoft.Json.Converters.UnixDateTimeConverter.WriteJson(Newtonsoft.Json.JsonWriter,System.Object,Newtonsoft.Json.JsonSerializer)">
       <summary>Writes the JSON representation of the object.</summary>
       <param name="writer">
         The
         <see cref="T:Newtonsoft.Json.JsonWriter"/>
         to write to.
       </param>
@@ -3650,14 +3686,18 @@
       <summary>Gets or sets how custom date formatted strings are parsed when reading JSON.</summary>
     </member>
     <member name="P:Newtonsoft.Json.JsonReader.MaxDepth">
       <summary>
         Gets or sets the maximum depth allowed when reading JSON. Reading past this depth will throw a
         <see cref="T:Newtonsoft.Json.JsonReaderException"/>
         .
+            A null value means there is no maximum. 
+            The default value is
+        <c>64</c>
+        .
       </summary>
     </member>
     <member name="P:Newtonsoft.Json.JsonReader.TokenType">
       <summary>Gets the type of the current JSON token.</summary>
     </member>
     <member name="P:Newtonsoft.Json.JsonReader.Value">
       <summary>Gets the text value of the current JSON token.</summary>
@@ -4335,15 +4375,15 @@
     <member name="P:Newtonsoft.Json.JsonSerializer.MaxDepth">
       <summary>
         Gets or sets the maximum depth allowed when reading JSON. Reading past this depth will throw a
         <see cref="T:Newtonsoft.Json.JsonReaderException"/>
         .
             A null value means there is no maximum.
             The default value is
-        <c>null</c>
+        <c>64</c>
         .
       </summary>
     </member>
     <member name="P:Newtonsoft.Json.JsonSerializer.CheckAdditionalContent">
       <summary>
         Gets a value indicating whether there will be a check for additional JSON content after deserializing an object.
             The default value is
@@ -4879,15 +4919,15 @@
     <member name="P:Newtonsoft.Json.JsonSerializerSettings.MaxDepth">
       <summary>
         Gets or sets the maximum depth allowed when reading JSON. Reading past this depth will throw a
         <see cref="T:Newtonsoft.Json.JsonReaderException"/>
         .
             A null value means there is no maximum.
             The default value is
-        <c>null</c>
+        <c>64</c>
         .
       </summary>
     </member>
     <member name="P:Newtonsoft.Json.JsonSerializerSettings.Formatting">
       <summary>
         Indicates how JSON text output is formatted.
             The default value is
@@ -4981,14 +5021,24 @@
     <member name="M:Newtonsoft.Json.JsonSerializerSettings.#ctor">
       <summary>
         Initializes a new instance of the
         <see cref="T:Newtonsoft.Json.JsonSerializerSettings"/>
         class.
       </summary>
     </member>
+    <member name="M:Newtonsoft.Json.JsonSerializerSettings.#ctor(Newtonsoft.Json.JsonSerializerSettings)">
+      <summary>
+        Initializes a new instance of the
+        <see cref="T:Newtonsoft.Json.JsonSerializerSettings"/>
+        class
+            using values copied from the passed in
+        <see cref="T:Newtonsoft.Json.JsonSerializerSettings"/>
+        .
+      </summary>
+    </member>
     <member name="T:Newtonsoft.Json.JsonTextReader">
       <summary>Represents a reader that provides fast, non-cached, forward-only access to JSON text data.</summary>
     </member>
     <member name="M:Newtonsoft.Json.JsonTextReader.ReadAsync(System.Threading.CancellationToken)">
       <summary>Asynchronously reads the next JSON token from the source.</summary>
       <param name="cancellationToken">
         The token to monitor for cancellation requests. The default value is
@@ -12049,14 +12099,39 @@
       <param name="reader">The reader.</param>
       <returns>
         An instance of
         <see cref="T:Newtonsoft.Json.Linq.JRaw"/>
         with the content of the reader's current token.
       </returns>
     </member>
+    <member name="T:Newtonsoft.Json.Linq.JsonCloneSettings">
+      <summary>Specifies the settings used when cloning JSON.</summary>
+    </member>
+    <member name="M:Newtonsoft.Json.Linq.JsonCloneSettings.#ctor">
+      <summary>
+        Initializes a new instance of the
+        <see cref="T:Newtonsoft.Json.Linq.JsonCloneSettings"/>
+        class.
+      </summary>
+    </member>
+    <member name="P:Newtonsoft.Json.Linq.JsonCloneSettings.CopyAnnotations">
+      <summary>
+        Gets or sets a flag that indicates whether to copy annotations when cloning a
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        .
+            The default value is
+        <c>true</c>
+        .
+      </summary>
+      <value>
+        A flag that indicates whether to copy annotations when cloning a
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        .
+      </value>
+    </member>
     <member name="T:Newtonsoft.Json.Linq.JsonLoadSettings">
       <summary>Specifies the settings used when loading JSON.</summary>
     </member>
     <member name="M:Newtonsoft.Json.Linq.JsonLoadSettings.#ctor">
       <summary>
         Initializes a new instance of the
         <see cref="T:Newtonsoft.Json.Linq.JsonLoadSettings"/>
@@ -12114,14 +12189,27 @@
             The exact property name will be searched for first and if no matching property is found then
             the
         <see cref="T:System.StringComparison"/>
         will be used to match a property.
       </summary>
       <value>The comparison used to match property names while merging.</value>
     </member>
+    <member name="T:Newtonsoft.Json.Linq.JsonSelectSettings">
+      <summary>Specifies the settings used when selecting JSON.</summary>
+    </member>
+    <member name="P:Newtonsoft.Json.Linq.JsonSelectSettings.RegexMatchTimeout">
+      <summary>Gets or sets a timeout that will be used when executing regular expressions.</summary>
+      <value>The timeout that will be used when executing regular expressions.</value>
+    </member>
+    <member name="P:Newtonsoft.Json.Linq.JsonSelectSettings.ErrorWhenNoMatch">
+      <summary>Gets or sets a flag that indicates whether an error should be thrown if
+            no tokens are found when evaluating part of the expression.</summary>
+      <value>A flag that indicates whether an error should be thrown if
+            no tokens are found when evaluating part of the expression.</value>
+    </member>
     <member name="T:Newtonsoft.Json.Linq.JToken">
       <summary>Represents an abstract JSON token.</summary>
     </member>
     <member name="M:Newtonsoft.Json.Linq.JToken.WriteToAsync(Newtonsoft.Json.JsonWriter,System.Threading.CancellationToken,Newtonsoft.Json.JsonConverter[])">
       <summary>
         Writes this token to a
         <see cref="T:Newtonsoft.Json.JsonWriter"/>
@@ -13972,14 +14060,36 @@
       <param name="errorWhenNoMatch">A flag to indicate whether an error should be thrown if no tokens are found when evaluating part of the expression.</param>
       <returns>
         A
         <see cref="T:Newtonsoft.Json.Linq.JToken"/>
         .
       </returns>
     </member>
+    <member name="M:Newtonsoft.Json.Linq.JToken.SelectToken(System.String,Newtonsoft.Json.Linq.JsonSelectSettings)">
+      <summary>
+        Selects a
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        using a JSONPath expression. Selects the token that matches the object path.
+      </summary>
+      <param name="path">
+        A
+        <see cref="T:System.String"/>
+        that contains a JSONPath expression.
+      </param>
+      <param name="settings">
+        The
+        <see cref="T:Newtonsoft.Json.Linq.JsonSelectSettings"/>
+        used to select tokens.
+      </param>
+      <returns>
+        A
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        .
+      </returns>
+    </member>
     <member name="M:Newtonsoft.Json.Linq.JToken.SelectTokens(System.String)">
       <summary>Selects a collection of elements using a JSONPath expression.</summary>
       <param name="path">
         A
         <see cref="T:System.String"/>
         that contains a JSONPath expression.
       </param>
@@ -14003,14 +14113,34 @@
         An
         <see cref="T:System.Collections.Generic.IEnumerable`1"/>
         of
         <see cref="T:Newtonsoft.Json.Linq.JToken"/>
         that contains the selected elements.
       </returns>
     </member>
+    <member name="M:Newtonsoft.Json.Linq.JToken.SelectTokens(System.String,Newtonsoft.Json.Linq.JsonSelectSettings)">
+      <summary>Selects a collection of elements using a JSONPath expression.</summary>
+      <param name="path">
+        A
+        <see cref="T:System.String"/>
+        that contains a JSONPath expression.
+      </param>
+      <param name="settings">
+        The
+        <see cref="T:Newtonsoft.Json.Linq.JsonSelectSettings"/>
+        used to select tokens.
+      </param>
+      <returns>
+        An
+        <see cref="T:System.Collections.Generic.IEnumerable`1"/>
+        of
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        that contains the selected elements.
+      </returns>
+    </member>
     <member name="M:Newtonsoft.Json.Linq.JToken.GetMetaObject(System.Linq.Expressions.Expression)">
       <summary>
         Returns the
         <see cref="T:System.Dynamic.DynamicMetaObject"/>
         responsible for binding operations performed on this object.
       </summary>
       <param name="parameter">The expression tree representation of the runtime value.</param>
@@ -14041,14 +14171,31 @@
       </summary>
       <returns>
         A new instance of the
         <see cref="T:Newtonsoft.Json.Linq.JToken"/>
         .
       </returns>
     </member>
+    <member name="M:Newtonsoft.Json.Linq.JToken.DeepClone(Newtonsoft.Json.Linq.JsonCloneSettings)">
+      <summary>
+        Creates a new instance of the
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        . All child tokens are recursively cloned.
+      </summary>
+      <param name="settings">
+        A
+        <see cref="T:Newtonsoft.Json.Linq.JsonCloneSettings"/>
+        object to configure cloning settings.
+      </param>
+      <returns>
+        A new instance of the
+        <see cref="T:Newtonsoft.Json.Linq.JToken"/>
+        .
+      </returns>
+    </member>
     <member name="M:Newtonsoft.Json.Linq.JToken.AddAnnotation(System.Object)">
       <summary>
         Adds an object to the annotation list of this
         <see cref="T:Newtonsoft.Json.Linq.JToken"/>
         .
       </summary>
       <param name="annotation">The annotation to add.</param>
@@ -16491,39 +16638,14 @@
         The
         <see cref="T:System.Diagnostics.TraceLevel"/>
         at which to write this trace.
       </param>
       <param name="message">The trace message.</param>
       <param name="ex">The trace exception. This parameter is optional.</param>
     </member>
-    <member name="T:Newtonsoft.Json.Serialization.DynamicValueProvider">
-      <summary>
-        Get and set values for a
-        <see cref="T:System.Reflection.MemberInfo"/>
-        using dynamic methods.
-      </summary>
-    </member>
-    <member name="M:Newtonsoft.Json.Serialization.DynamicValueProvider.#ctor(System.Reflection.MemberInfo)">
-      <summary>
-        Initializes a new instance of the
-        <see cref="T:Newtonsoft.Json.Serialization.DynamicValueProvider"/>
-        class.
-      </summary>
-      <param name="memberInfo">The member info.</param>
-    </member>
-    <member name="M:Newtonsoft.Json.Serialization.DynamicValueProvider.SetValue(System.Object,System.Object)">
-      <summary>Sets the value.</summary>
-      <param name="target">The target to set the value on.</param>
-      <param name="value">The value to set on the target.</param>
-    </member>
-    <member name="M:Newtonsoft.Json.Serialization.DynamicValueProvider.GetValue(System.Object)">
-      <summary>Gets the value.</summary>
-      <param name="target">The target to get the value from.</param>
-      <returns>The value.</returns>
-    </member>
     <member name="T:Newtonsoft.Json.Serialization.ErrorContext">
       <summary>Provides information surrounding an error.</summary>
     </member>
     <member name="P:Newtonsoft.Json.Serialization.ErrorContext.Error">
       <summary>Gets the error.</summary>
       <value>The error.</value>
     </member>
```

### Comparing `pyaedt-0.6.71/pyaedt/dlls/PDFReport/PdfSharp-gdi.dll` & `pyaedt-0.6.72/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files 20% similar despite different names*

#### pedump {}

```diff
@@ -1,170 +1,150 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x5c583c6e
+	             Time stamp: 0xffa45f76
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x0008c000
-	  Initialized Data Size: 0x00002000
+	              Code Size: 0x00084e00
+	  Initialized Data Size: 0x00000800
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x0008bdb2
+	        Entry Point RVA: 0x00084d82
 	 	  Code Base RVA: 0x00002000
-		  Data Base RVA: 0x0008e000
+		  Data Base RVA: 0x00088000
 
 
 NT Header:
-	   Image Base (0x400000): 0x11000000
+	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
-	   File Align (512/4096): 0x00001000
+	   File Align (512/4096): 0x00000200
 	            OS Major (4): 0x0004
 	            OS Minor (0): 0x0000
 	  	  User Major (0): 0x0000
 	  	  User Minor (0): 0x0000
 	  	Subsys major (4): 0x0004
 	  	Subsys minor (0): 0x0000
 	 	       Reserverd: 0x00000000
-	 	      Image Size: 0x00092000
-	 	     Header Size: 0x00001000
-	            Checksum (0): 0x00091e3a
+	 	      Image Size: 0x0008c000
+	 	     Header Size: 0x00000200
+	            Checksum (0): 0x00000000
 	               Subsystem: 0x0003
-	           DLL Flags (0): 0x8540
+	           DLL Flags (0): 0x8560
 	 Stack Reserve Size (1M): 0x00100000
 	Stack commit Size (4096): 0x00001000
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x0008bd60 [0x0000004f]
-	   Resource Table: 0x0008e000 [0x00000480]
+	     Import Table: 0x00084d2e [0x0000004f]
+	   Resource Table: 0x00088000 [0x000005fc]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
-	      Reloc Table: 0x00090000 [0x0000000c]
-	            Debug: 0x00000000 [0x00000000]
+	      Reloc Table: 0x0008a000 [0x0000000c]
+	            Debug: 0x00084c48 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x0008be30
+	   Virtual Size: 0x00084df8
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x0008c000
-	   Raw Data Ptr: 0x00001000
+	  Raw Data Size: 0x00084e00
+	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
-	   Virtual Size: 0x00000480
-	Virtual Address: 0x0008e000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0008d000
+	   Virtual Size: 0x000005fc
+	Virtual Address: 0x00088000
+	  Raw Data Size: 0x00000600
+	   Raw Data Ptr: 0x00085000
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
-	Virtual Address: 0x00090000
-	  Raw Data Size: 0x00001000
-	   Raw Data Ptr: 0x0008e000
+	Virtual Address: 0x0008a000
+	  Raw Data Size: 0x00000200
+	   Raw Data Ptr: 0x00085600
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
-                    Flags: ilonly, 32/64, no-trackdebug, strongnamesigned
-	         Metadata: 0x00040c1c [0x0004a184]
+                    Flags: ilonly, 32/64, no-trackdebug, notsigned
+	         Metadata: 0x0003c7fc [0x00048144]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x0008ada0 [0x00000f40]
-	   Strong Name at: 0x0008bce0 [0x00000080]
+	     Resources at: 0x00084940 [0x00000308]
+	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
-Strong name:
-	 5D 55 A9 81 32 62 11 1D 2A 20 B5 00 41 14 B2 23
-	 6B 56 34 B5 36 26 CD A1 21 29 FF DD 94 1F AF 77
-	 CC B1 15 7C F1 F8 22 B1 02 B9 78 9D BC 41 9E B1
-	 8B 02 11 A9 55 9B 9C FE 81 6C CF AA D9 E4 57 9F
-	 C9 F4 EF C9 25 D6 F8 4E 80 1B 2F 59 9F 47 60 F8
-	 A6 92 CF 77 6B 3E 1A 1E E0 92 44 8D 39 D8 A0 54
-	 26 DE E4 72 56 72 83 88 B8 F0 8A 7F 2A E5 CD E4
-	 D1 37 DA F5 FB 56 E0 F7 6A E1 AF DC 48 31 A7 2D
-
-Public key:
-	 00 24 00 00 04 80 00 00 94 00 00 00 06 02 00 00
-	 00 24 00 00 52 53 41 31 00 04 00 00 01 00 01 00
-	 87 94 E8 03 E5 66 EC CC 3C 91 81 F5 2C 4F 70 44
-	 E5 44 2C C2 CE 3C BB A9 FC 11 BC 41 86 BA 2E 44
-	 6C D3 1D EE A2 0C 1A 8F 49 9E 97 84 17 FA D2 BC
-	 74 14 3A 4F 83 98 F7 CF 5C 5C 02 71 B0 F7 FE 90
-	 7C 53 7C FF 28 B9 D5 82 DA 41 28 9D 1D AE 90 16
-	 8A 3D A2 A5 ED 11 15 21 0A 18 FD AE 83 24 79 D3
-	 E6 39 CA 40 03 28 6B A8 B9 8D C9 14 46 15 C0 40
-	 ED 83 89 81 AC 81 61 12 DF 3B 5A 9E 7C AB 4F BB
+Strong name: none
+
+Public key: none
 
 Metadata header:
            Version: 1.1
-    Version string: v2.0.50727
+    Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0002562c [153024 == 0x000255c0]
-	    Strings: 0x0002562c - 0x000344cc [61088 == 0x0000eea0]
-	       Blob: 0x00040e38 - 0x0004a184 [37708 == 0x0000934c]
-	User string: 0x000344cc - 0x00040e28 [51548 == 0x0000c95c]
-	       GUID: 0x00040e28 - 0x00040e38 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x00024800 [149396 == 0x00024794]
+	    Strings: 0x00024800 - 0x00033f9c [63388 == 0x0000f79c]
+	       Blob: 0x00040260 - 0x00048144 [32484 == 0x00007ee4]
+	User string: 0x00033f9c - 0x00040250 [49844 == 0x0000c2b4]
+	       GUID: 0x00040250 - 0x00040260 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (10 bytes, at 3fd1c)
-Table TypeRef: 216 records (6 bytes, at 3fd26)
-Table TypeDef: 508 records (14 bytes, at 40236)
-Table Field: 2846 records (6 bytes, at 41dfe)
-Table Method: 4353 records (14 bytes, at 460b2)
-Table Param: 4258 records (6 bytes, at 54ec0)
-Table InterfaceImpl: 60 records (4 bytes, at 5b28c)
-Table MemberRef: 919 records (6 bytes, at 5b37c)
-Table Constant: 1410 records (6 bytes, at 5c906)
-Table CustomAttribute: 546 records (8 bytes, at 5ea12)
-Table FieldMarshal: 1 records (4 bytes, at 5fb22)
-Table ClassLayout: 17 records (8 bytes, at 5fb26)
-Table FieldLayoutt: 2 records (6 bytes, at 5fbae)
-Table StandaloneSig: 486 records (2 bytes, at 5fbba)
-Table EventMap: 1 records (4 bytes, at 5ff86)
-Table Event: 1 records (6 bytes, at 5ff8a)
-Table PropertyMap: 237 records (4 bytes, at 5ff90)
-Table Property: 1367 records (6 bytes, at 60344)
-Table MethodSemantics: 1706 records (6 bytes, at 6234e)
-Table MethodImpl: 70 records (6 bytes, at 64b4a)
-Table Moduleref: 2 records (2 bytes, at 64cee)
-Table TypeSpec: 108 records (2 bytes, at 64cf2)
-Table ImplMap: 10 records (8 bytes, at 64dca)
-Table FieldRVA: 76 records (6 bytes, at 64e1a)
-Table Assembly: 1 records (22 bytes, at 64fe2)
-Table AssemblyRef: 4 records (20 bytes, at 64ff8)
-Table ManifestResource: 3 records (12 bytes, at 65048)
-Table NestedClass: 108 records (4 bytes, at 6506c)
-Table GenericParam: 1 records (8 bytes, at 6521c)
-Table MethodSpec: 7 records (4 bytes, at 65224)
-Table GenericParamConstraint: 1 records (4 bytes, at 65240)
+Table Module: 1 records (10 bytes, at 3aaf4)
+Table TypeRef: 174 records (6 bytes, at 3aafe)
+Table TypeDef: 532 records (14 bytes, at 3af12)
+Table Field: 2809 records (6 bytes, at 3cc2a)
+Table Method: 4243 records (14 bytes, at 40e00)
+Table Param: 3922 records (6 bytes, at 4f60a)
+Table InterfaceImpl: 67 records (4 bytes, at 551f6)
+Table MemberRef: 764 records (6 bytes, at 55302)
+Table Constant: 1392 records (6 bytes, at 564ea)
+Table CustomAttribute: 588 records (8 bytes, at 5858a)
+Table FieldMarshal: 2 records (4 bytes, at 597ea)
+Table ClassLayout: 17 records (8 bytes, at 597f2)
+Table FieldLayoutt: 2 records (6 bytes, at 5987a)
+Table StandaloneSig: 451 records (2 bytes, at 59886)
+Table PropertyMap: 248 records (4 bytes, at 59c0c)
+Table Property: 1379 records (6 bytes, at 59fec)
+Table MethodSemantics: 1734 records (6 bytes, at 5c03e)
+Table MethodImpl: 77 records (6 bytes, at 5e8e2)
+Table Moduleref: 1 records (2 bytes, at 5eab0)
+Table TypeSpec: 149 records (2 bytes, at 5eab2)
+Table ImplMap: 9 records (8 bytes, at 5ebdc)
+Table FieldRVA: 76 records (6 bytes, at 5ec24)
+Table Assembly: 1 records (22 bytes, at 5edec)
+Table AssemblyRef: 17 records (20 bytes, at 5ee02)
+Table ManifestResource: 1 records (12 bytes, at 5ef56)
+Table NestedClass: 120 records (4 bytes, at 5ef62)
+Table GenericParam: 4 records (8 bytes, at 5f142)
+Table MethodSpec: 31 records (4 bytes, at 5f162)
+Table GenericParamConstraint: 7 records (4 bytes, at 5f1de)
```

### Comparing `pyaedt-0.6.71/pyaedt/downloads.py` & `pyaedt-0.6.72/pyaedt/downloads.py`

 * *Files 5% similar despite different names*

```diff
@@ -155,16 +155,16 @@
     -------
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_aedb()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_aedb()
     >>> path
     'C:/Users/user/AppData/local/temp/Galileo.aedb'
     """
     _download_file("edb/Galileo.aedb", "GRM32ER72A225KA35_25C_0V.sp", destination)
 
     return _download_file("edb/Galileo.aedb", "edb.def", destination)
 
@@ -186,16 +186,16 @@
     -------
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_edb_merge_utility(force_download=True)
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_edb_merge_utility(force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/wpf_edb_merge/merge_wizard.py'
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "wpf_edb_merge")
@@ -223,16 +223,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_netlist()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_netlist()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/netlist_small.cir'
     """
 
     return _download_file("netlist", "netlist_small.cir", destination)
 
 
@@ -253,16 +253,16 @@
         Path to the example file.
 
     Examples
     --------
 
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_antenna_array()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_antenna_array()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/FiniteArray_Radome_77GHz_3D_CADDM.aedt'
     """
 
     return _download_file("array_antenna", "FiniteArray_Radome_77GHz_3D_CADDM.aedt", destination)
 
 
@@ -282,16 +282,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_antenna_array()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_antenna_array()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/FiniteArray_Radome_77GHz_3D_CADDM.aedt'
     """
 
     return _download_file("sbr", "Cassegrain.aedt", destination)
 
 
@@ -311,16 +311,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_sbr_time()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_sbr_time()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/sbr/poc_scat_small.aedt'
     """
 
     return _download_file("sbr", "poc_scat_small.aedt", destination)
 
 
@@ -340,16 +340,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_icepak()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_icepak()
     >>> pathavoid
     'C:/Users/user/AppData/local/temp/pyaedtexamples/Graphic_Card.aedt'
     """
 
     return _download_file("icepak", "Graphics_card.aedt", destination)
 
 
@@ -371,16 +371,16 @@
     str
         Path to QFP2 the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path1, path2 = examples.download_icepak_3d_component()
+    >>> import pyaedt
+    >>> path1, path2 = pyaedt.downloads.download_icepak_3d_component()
     >>> path1
     'C:/Users/user/AppData/local/temp/pyaedtexamples/PCBAssembly.aedt',
     """
     _download_file("icepak_3dcomp//PCBAssembly.aedb", destination=destination)
     return _download_file("icepak_3dcomp", "PCBAssembly.aedt", destination), _download_file(
         "icepak_3dcomp", "QFP2.aedt", destination
     )
@@ -402,16 +402,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_via_wizard()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_via_wizard()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/Graphic_Card.aedt'
     """
 
     return _download_file("via_wizard", "viawizard_vacuum_FR4.aedt", destination)
 
 
@@ -430,16 +430,16 @@
     -------
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_touchstone()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_touchstone()
     >>> path
     'C:/Users/user/AppData/local/temp/pyaedtexamples/ssn_ssn.s6p'
     """
     return _download_file("touchstone", "SSN_ssn.s6p", destination)
 
 
 def download_sherlock(destination=None):
@@ -458,16 +458,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_sherlock()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_sherlock()
     >>> path
     'C:/Users/user/AppData/local/temp/Galileo.aedb'
     """
     if not destination:
         destination = EXAMPLES_PATH
     _download_file("sherlock", "MaterialExport.csv", destination)
     _download_file("sherlock", "TutorialBoardPartsList.csv", destination)
@@ -494,16 +494,16 @@
     (str, str)
         Path to the 30DH_20C_smooth and BH_Arnold_Magnetics_N30UH_80C tabular material data file file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_leaf(r"c:\temp")
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_leaf(r"c:\temp")
     >>> path
     ('C:/temp/BH_Arnold_Magnetics_N30UH_80C.tab', 'C:/temp/BH_Arnold_Magnetics_N30UH_80C.tab')
     """
     if not destination:
         destination = EXAMPLES_PATH
     file1 = _download_file("nissan", "30DH_20C_smooth.tab", destination)
     file2 = _download_file("nissan", "BH_Arnold_Magnetics_N30UH_80C.tab", destination)
@@ -528,16 +528,16 @@
     -------
     str
         Path to the example folder containing all example files.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_custom_reports(force_download=True)
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_custom_reports(force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/custom_reports'
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "custom_reports")
@@ -570,16 +570,16 @@
     -------
     str
         Path to the example folder containing all example files.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_3dcomponent(force_download=True)
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_3dcomponent(force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/array_3d_component'
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, "array_3d_component")
@@ -607,16 +607,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_multiparts()
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_multiparts()
     >>> path
     'C:/Users/user/AppData/local/temp/multiparts/library'
     """
     if not destination:
         destination = EXAMPLES_PATH
     dest_folder = os.path.join(destination, "multiparts")
     if os.path.exists(os.path.join(dest_folder, "library")):
@@ -646,16 +646,16 @@
     -------
     str
         Path to the folder containing all Twin Builder example data files.
 
     Examples
     --------
     Download an example result file and return the path of the file.
-    >>> from pyaedt import examples
-    >>> path = examples.download_twin_builder_data(file_name="Example1.zip",force_download=True)
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_twin_builder_data(file_name="Example1.zip",force_download=True)
     >>> path
     'C:/Users/user/AppData/local/temp/twin_builder'
     """
     if not destination:
         destination = EXAMPLES_PATH
     if force_download:
         local_path = os.path.join(destination, os.path.join("twin_builder", file_name))
@@ -685,16 +685,16 @@
     str
         Path to the example file.
 
     Examples
     --------
     Download an example result file and return the path of the file.
 
-    >>> from pyaedt import examples
-    >>> path = examples.download_file("motorcad", "IPM_Vweb_Hairpin.mot")
+    >>> import pyaedt
+    >>> path = pyaedt.downloads.download_file("motorcad", "IPM_Vweb_Hairpin.mot")
     >>> path
     'C:/Users/user/AppData/local/temp/PyAEDTExamples/motorcad'
     """
     local_path = _download_file(directory, filename, destination)
 
     return local_path
```

### Comparing `pyaedt-0.6.71/pyaedt/edb.py` & `pyaedt-0.6.72/pyaedt/edb.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,14 @@
                     self._logger.info("Edb version " + edbversion)
                 except IndexError:
                     raise Exception("No ANSYSEM_ROOTxxx is found.")
             self.edbversion = edbversion
             self.isaedtowned = isaedtowned
             self._init_dlls()
             self._db = None
-            # self._edb.Database.SetRunAsStandAlone(not isaedtowned)
             self.isreadonly = isreadonly
             self.cellname = cellname
             if not edbpath:
                 if is_windows:
                     edbpath = os.getenv("USERPROFILE")
                     if not edbpath:
                         edbpath = os.path.expanduser("~")
@@ -457,17 +456,21 @@
 
         Returns
         -------
 
         """
         if init_dlls:
             self._init_dlls()
-        self.logger.info("EDB Path %s", self.edbpath)
-        self.logger.info("EDB Version %s", self.edbversion)
+        self.logger.info("EDB Path is %s", self.edbpath)
+        self.logger.info("EDB Version is %s", self.edbversion)
+        # if self.edbversion > "2023.1":
+        #     self.standalone = False
+
         self.edb.Database.SetRunAsStandAlone(self.standalone)
+
         self.logger.info("EDB Standalone %s", self.standalone)
         try:
             db = self.edb.Database.Open(self.edbpath, self.isreadonly)
         except Exception as e:
             db = None
             self.logger.error("Builder is not Initialized.")
         if not db:
@@ -554,14 +557,17 @@
         ----------
         init_dlls : bool, optional
             Whether to initialize DLLs. The default is ``False``.
 
         """
         if init_dlls:
             self._init_dlls()
+        # if self.edbversion > "2023.1":
+        #     self.standalone = False
+
         self.edb.Database.SetRunAsStandAlone(self.standalone)
         db = self.edb.Database.Create(self.edbpath)
         if not db:
             self.logger.warning("Error creating the database.")
             self._db = None
             self._active_cell = None
             self.builder = None
@@ -1083,14 +1089,16 @@
 
 
         Returns
         -------
         Instance of `Edb.Utility.Value`
 
         """
+        if isinstance(val, self.edb.Utility.Value):
+            return val
         if isinstance(val, (int, float)):
             return self.edb.Utility.Value(val)
         m1 = re.findall(r"(?<=[/+-/*//^/(/[])([a-z_A-Z/$]\w*)", str(val).replace(" ", ""))
         m2 = re.findall(r"^([a-z_A-Z/$]\w*)", str(val).replace(" ", ""))
         val_decomposed = list(set(m1).union(m2))
         if not val_decomposed:
             return self.edb.Utility.Value(val)
@@ -1101,14 +1109,54 @@
         if set(val_decomposed).intersection(var_names_cell):
             return self.edb.Utility.Value(val, var_server_cell)
         if set(val_decomposed).intersection(var_names):
             return self.edb.Utility.Value(val, var_server_db)
         return self.edb.Utility.Value(val)
 
     @pyaedt_function_handler()
+    def point_3d(self, x, y, z=0.0):
+        """Compute the Edb 3d Point Data.
+
+        Parameters
+        ----------
+        x : float, int or str
+            X value.
+        y : float, int or str
+            Y value.
+        z : float, int or str, optional
+            Z value.
+
+        Returns
+        -------
+        ``Geometry.Point3DData``.
+        """
+        return self.edb.Geometry.Point3DData(self.edb_value(x), self.edb_value(y), self.edb_value(z))
+
+    @pyaedt_function_handler()
+    def point_data(self, x, y=None):
+        """Compute the Edb Point Data.
+
+        Parameters
+        ----------
+        x : float, int or str
+            X value.
+        y : float, int or str, optional
+            Y value.
+
+
+        Returns
+        -------
+        ``Geometry.PointData``.
+        """
+        if y is None:
+            return self.edb.Geometry.PointData(self.edb_value(x))
+        else:
+            return self.edb.Geometry.PointData(self.edb_value(x), self.edb_value(y))
+
+    @pyaedt_function_handler()
     def _is_file_existing_and_released(self, filename):
         if os.path.exists(filename):
             try:
                 os.rename(filename, filename + "_")
                 os.rename(filename + "_", filename)
                 return True
             except OSError as e:
@@ -1384,16 +1432,20 @@
                 obj_data = prim.primitive_object.GetPolygonData().Expand(
                     expansion_size, tolerance, round_corner, round_extension
                 )
                 if obj_data:
                     _polys.extend(list(obj_data))
         if smart_cutout:
             _polys.extend(self._smart_cut(net_signals, reference_list, include_pingroups))
-        _poly = self.edb.Geometry.PolygonData.Unite(convert_py_list_to_net_list(_polys))[0]
-        return _poly
+        _poly_unite = list(self.edb.Geometry.PolygonData.Unite(convert_py_list_to_net_list(_polys)))
+        if len(_poly_unite) == 1:
+            return _poly_unite[0]
+        else:
+            areas = [i.Area() for i in _poly_unite]
+            return _poly_unite[areas.index(max(areas))]
 
     @pyaedt_function_handler()
     def _smart_cut(self, net_signals, reference_list=[], include_pingroups=True):
         _polys = []
         terms = [term for term in list(self.active_layout.Terminals) if int(term.GetBoundaryType()) in [0, 3, 4, 7, 8]]
         locations = []
         for term in terms:
@@ -2664,18 +2716,19 @@
             Either if generate or not current source report. Default is `True`.
         voltage_sources : bool, optional
             Either if generate or not voltage source report. Default is `True`.
         power_tree : bool, optional
             Either if generate or not power tree image. Default is `True`.
         loop_res : bool, optional
             Either if generate or not loop resistance report. Default is `True`.
+
         Returns
         -------
         list
-            list of files generated.
+            List of files generated.
         """
         process = SiwaveSolve(self.edbpath, aedt_version=self.edbversion)
         try:
             self._db.Close()
         except:
             pass
         return process.export_dc_report(
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/components.py` & `pyaedt-0.6.72/pyaedt/edb_core/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -654,15 +654,15 @@
         Parameters
         ----------
         sources : list[Source]
             List of ``edb_data.sources.Source`` objects.
 
         Returns
         -------
-        double, bool
+        bool
             ``True`` when successful, ``False`` when failed.
 
         """
 
         if not sources:  # pragma: no cover
             return False
         if isinstance(sources, Source):  # pragma: no cover
@@ -741,27 +741,23 @@
     ):
         """Create ports on given component.
 
         Parameters
         ----------
         component : str or self._edb.Cell.Hierarchy.Component
             EDB component or str component name.
-
         net_list : str or list of string.
             List of nets where ports must be created on the component.
             If the net is not part of the component, this parameter is skipped.
-
         port_type : SourceType enumerator, CoaxPort or CircuitPort
             Type of port to create. ``CoaxPort`` generates solder balls.
             ``CircuitPort`` generates circuit ports on pins belonging to the net list.
-
         do_pingroup : bool
             True activate pingroup during port creation (only used with combination of CoaxPort),
             False will take the closest reference pin and generate one port per signal pin.
-
         refnet : string or list of string.
             list of the reference net.
 
         Returns
         -------
         double, bool
             Salder ball height vale, ``False`` when failed.
@@ -873,17 +869,15 @@
 
         Returns
         -------
         Edb terminal.
         """
 
         pin_position = self.get_pin_position(pin)  # pragma no cover
-        pin_pos = self._edb.Geometry.PointData(
-            self._get_edb_value(pin_position[0]), self._get_edb_value(pin_position[1])  # pragma no cover
-        )
+        pin_pos = self._pedb.point_data(*pin_position)
         res, from_layer, _ = pin.GetLayerRange()
         cmp_name = pin.GetComponent().GetName()
         net_name = pin.GetNet().GetName()
         pin_name = pin.GetName()
         term_name = "{}.{}.{}".format(cmp_name, pin_name, net_name)
         term = self._edb.Cell.Terminal.PointTerminal.Create(
             pin.GetLayout(), pin.GetNet(), term_name, pin_pos, from_layer
@@ -902,22 +896,22 @@
 
         Returns
         -------
         Edb pin.
 
         """
         res, pin_position, pin_rot = pin.GetPositionAndRotation(
-            self._edb.Geometry.PointData(self._get_edb_value(0.0), self._get_edb_value(0.0)),
+            self._pedb.point_data(0.0, 0.0),
             0.0,
         )
         distance = 1e3
         closest_pin = ref_pinlist[0]
         for ref_pin in ref_pinlist:
             res, ref_pin_position, ref_pin_rot = ref_pin.GetPositionAndRotation(
-                self._edb.Geometry.PointData(self._get_edb_value(0.0), self._get_edb_value(0.0)),
+                self._pedb.point_data(0.0, 0.0),
                 0.0,
             )
             temp_distance = pin_position.Distance(ref_pin_position)
             if temp_distance < distance:
                 distance = temp_distance
                 closest_pin = ref_pin
         return closest_pin
@@ -989,29 +983,35 @@
             component = self.instances[component]
         if not isinstance(component, EDBComponent):  # pragma: no cover
             return False
         self.set_component_rlc(component.refdes)
         pins = self.get_pin_from_component(component.refdes)
         if len(pins) == 2:  # pragma: no cover
             pos_pin_loc = self.get_pin_position(pins[0])
-            pt = self._pedb.edb.Geometry.PointData(
-                self._get_edb_value(pos_pin_loc[0]), self._get_edb_value(pos_pin_loc[1])
-            )
+            pt = self._pedb.point_data(*pos_pin_loc)
+
             pin_layers = self._padstack._get_pin_layer_range(pins[0])
             pos_pin_term = self._pedb.edb.Cell.Terminal.PointTerminal.Create(
-                self._active_layout, pins[0].GetNet(), pins[0].GetName(), pt, pin_layers[0]
+                self._active_layout,
+                pins[0].GetNet(),
+                "{}_{}".format(component.refdes, pins[0].GetName()),
+                pt,
+                pin_layers[0],
             )
             if not pos_pin_term:  # pragma: no cover
                 return False
             neg_pin_loc = self.get_pin_position(pins[1])
-            pt = self._pedb.edb.Geometry.PointData(
-                self._get_edb_value(neg_pin_loc[0]), self._get_edb_value(neg_pin_loc[1])
-            )
+            pt = self._pedb.point_data(*neg_pin_loc)
+
             neg_pin_term = self._pedb.edb.Cell.Terminal.PointTerminal.Create(
-                self._active_layout, pins[1].GetNet(), pins[1].GetName() + "_ref", pt, pin_layers[0]
+                self._active_layout,
+                pins[1].GetNet(),
+                "{}_{}_ref".format(component.refdes, pins[1].GetName()),
+                pt,
+                pin_layers[0],
             )
             if not neg_pin_term:  # pragma: no cover
                 return False
             pos_pin_term.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.PortBoundary)
             pos_pin_term.SetIsCircuitPort(True)
             pos_pin_term.SetName(component.refdes)
             neg_pin_term.SetBoundaryType(self._pedb.edb.Cell.Terminal.BoundaryType.PortBoundary)
@@ -1105,27 +1105,22 @@
 
         Parameters
         ----------
         pins : list
              List of EDB pins, length must be 2, since only 2 pins component are currently supported.
              It can be an `pyaedt.edb_core.edb_data.padstacks_data.EDBPadstackInstance` object or
              an Edb Padstack Instance object.
-
         component_name : str
             Component definition name.
-
         r_value : float
             Resistor value.
-
         c_value : float
             Capacitance value.
-
         l_value : float
             Inductor value.
-
         is_parallel : bool
             Using parallel model when ``True``, series when ``False``.
 
         Returns
         -------
         Component
             Created EDB component.
@@ -1173,14 +1168,15 @@
             Resistor value.
         c_value : float
             Capacitance value.
         l_value : float
             Inductor value.
         is_parallel : bool
             Using parallel model when ``True``, series when ``False``.
+
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
@@ -1247,16 +1243,17 @@
             rlc_model.SetPinPairRlc(pin_pair, rlc)
             edb_rlc_component_property = self._edb.Cell.Hierarchy.RLCComponentProperty()
             if not edb_rlc_component_property.SetModel(rlc_model) or not new_cmp.SetComponentProperty(
                 edb_rlc_component_property
             ):
                 return False  # pragma no cover
         new_cmp.SetTransform(hosting_component_location)
-        self._cmp[new_cmp.GetName()] = EDBComponent(self, new_cmp)
-        return new_cmp
+        new_edb_comp = EDBComponent(self, new_cmp)
+        self._cmp[new_cmp.GetName()] = new_edb_comp
+        return new_edb_comp
 
     @pyaedt_function_handler()
     def create_component_from_pins(
         self, pins, component_name, placement_layer=None, component_part_name=None
     ):  # pragma: no cover
         """Create a component from pins.
 
@@ -1561,28 +1558,29 @@
         sball_mid_diam=None,
         chip_orientation="chip_down",
     ):
         """Set cylindrical solder balls on a given component.
 
         Parameters
         ----------
-        component_name : str or EDB component
+        component : str or EDB component, optional
             Name of the discrete component.
         sball_diam  : str, float, optional
             Diameter of the solder ball.
         sball_height : str, float, optional
             Height of the solder ball.
         shape : str, optional
             Shape of solder ball. Options are ``"Cylinder"``,
             ``"Spheroid"``. The default is ``"Cylinder"``.
         sball_mid_diam : str, float, optional
             Mid diameter of the solder ball.
-        chip_orientation : str
+        chip_orientation : str, optional
             Give the chip orientation, ``"chip_down"`` or ``"chip_up"``. Default is ``"chip_down"``. Only applicable on
             IC model.
+
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
@@ -1822,14 +1820,15 @@
              Column index of part name. The default is ``"1"``. Set to ``None`` if
              the column does not exist.
         comp_type_col : int, optional
             Column index of component type. The default is ``"2"``.
         value_col : int, optional
             Column index of value. The default is ``"3"``. Set to ``None``
             if the column does not exist.
+
         Returns
         -------
         bool
         """
         with open(bom_file, "r") as f:
             lines = f.readlines()
             unmount_comp_list = list(self.instances.keys())
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/components_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from collections import OrderedDict
 import math
 import warnings
 
 from pyaedt import is_ironpython
+from pyaedt.edb_core.edb_data.edbvalue import EdbValue
+from pyaedt.edb_core.general import PadGeometryTpe
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import String
 from pyaedt.generic.clr_module import _clr
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
@@ -32,16 +35,14 @@
     """
 
     def __init__(self, edb_padstack, layer_name, pad_type, p_edb_padstack):
         self._edb_padstack = edb_padstack
         self._pedbpadstack = p_edb_padstack
         self.layer_name = layer_name
         self.pad_type = pad_type
-        self._parameters_values = None
-        pass
 
     @property
     def _padstack_methods(self):
         return self._pedbpadstack._padstack_methods
 
     @property
     def _stackup_layers(self):
@@ -55,14 +56,21 @@
     def _edb(self):
         return self._pedbpadstack._edb
 
     def _get_edb_value(self, value):
         return self._pedbpadstack._get_edb_value(value)
 
     @property
+    def _pad_parameter_value(self):
+        pad_params = self._edb_padstack.GetData().GetPadParametersValue(
+            self.layer_name, self.int_to_pad_type(self.pad_type)
+        )
+        return pad_params
+
+    @property
     def geometry_type(self):
         """Geometry type.
 
         Returns
         -------
         int
             Type of the geometry.
@@ -92,28 +100,32 @@
         elif geom_type == 4:
             params = [val, val, val]
         elif geom_type == 5:
             params = [val, val, val]
         self._update_pad_parameters_parameters(geom_type=geom_type, params=params)
 
     @property
+    def shape(self):
+        """Get the shape of the pad."""
+        return self._pad_parameter_value[1].ToString()
+
+    @shape.setter
+    def shape(self, value):
+        self._update_pad_parameters_parameters(geom_type=PadGeometryTpe[value].value)
+
+    @property
     def parameters_values(self):
         """Parameters.
 
         Returns
         -------
         list
             List of parameters.
         """
-        self._parameters_values = []
-        pad_values = self._edb_padstack.GetData().GetPadParametersValue(
-            self.layer_name, self.int_to_pad_type(self.pad_type)
-        )
-        self._parameters_values = [i.ToDouble() for i in pad_values[2]]
-        return self._parameters_values
+        return [i.tofloat for i in self.parameters.values()]
 
     @property
     def polygon_data(self):
         """Parameters.
 
         Returns
         -------
@@ -126,35 +138,83 @@
             )
             return pad_values[1]
         except:
             return
 
     @property
     def parameters(self):
-        """Parameters.
+        """Get parameters.
 
         Returns
         -------
-        list
-            List of parameters.
+        dict
         """
-        pad_values = self._edb_padstack.GetData().GetPadParametersValue(
-            self.layer_name, self.int_to_pad_type(self.pad_type)
-        )
-
-        # pad_values = self._padstack_methods.GetPadParametersValue(self._edb_padstack, self.layer_name, self)
-        return [i.ToString() for i in pad_values[2]]
+        value = list(self._pad_parameter_value[2])
+        if self.shape == PadGeometryTpe.Circle.name:
+            return OrderedDict({"Diameter": EdbValue(value[0])})
+        elif self.shape == PadGeometryTpe.Square.name:
+            return OrderedDict({"Size": EdbValue(value[0])})
+        elif self.shape == PadGeometryTpe.Rectangle.name:
+            return OrderedDict({"XSize": EdbValue(value[0]), "YSize": EdbValue(value[1])})
+        elif self.shape in [PadGeometryTpe.Oval.name, PadGeometryTpe.Bullet.name]:
+            return OrderedDict(
+                {"XSize": EdbValue(value[0]), "YSize": EdbValue(value[1]), "CornerRadius": EdbValue(value[2])}
+            )
+        elif self.shape == PadGeometryTpe.NSidedPolygon.name:
+            return OrderedDict({"Size": EdbValue(value[0]), "NumSides": EdbValue(value[1])})
+        elif self.shape in [PadGeometryTpe.Round45.name, PadGeometryTpe.Round90.name]:  # pragma: no cover
+            return OrderedDict(
+                {"Inner": EdbValue(value[0]), "ChannelWidth": EdbValue(value[1]), "IsolationGap": EdbValue(value[2])}
+            )
+        else:
+            return OrderedDict()  # pragma: no cover
 
     @parameters.setter
-    def parameters(self, propertylist):
-        if not isinstance(propertylist, list):
-            propertylist = [self._get_edb_value(propertylist)]
+    def parameters(self, value):
+        """Set parameters.
+        "Circle", {"Diameter": "0.5mm"}
+
+        Parameters
+        ----------
+        value : dict
+            Pad parameters in dictionary.
+        >>> pad = Edb.padstacks["PlanarEMVia"]["TOP"]
+        >>> pad.shape = "Circle"
+        >>> pad.pad_parameters{"Diameter": "0.5mm"}
+        >>> pad.shape = "Bullet"
+        >>> pad.pad_parameters{"XSize": "0.5mm", "YSize": "0.5mm"}
+        """
+
+        if isinstance(value, dict):
+            value = {k: v.tostring if isinstance(v, EdbValue) else v for k, v in value.items()}
+            if self.shape == PadGeometryTpe.Circle.name:
+                params = [self._get_edb_value(value["Diameter"])]
+            elif self.shape == PadGeometryTpe.Square.name:
+                params = [self._get_edb_value(value["Size"])]
+            elif self.shape == PadGeometryTpe.Rectangle.name:
+                params = [self._get_edb_value(value["XSize"]), self._get_edb_value(value["YSize"])]
+            elif self.shape == [PadGeometryTpe.Oval.name, PadGeometryTpe.Bullet.name]:
+                params = [
+                    self._get_edb_value(value["XSize"]),
+                    self._get_edb_value(value["YSize"]),
+                    self._get_edb_value(value["CornerRadius"]),
+                ]
+            elif self.shape in [PadGeometryTpe.Round45.name, PadGeometryTpe.Round90.name]:  # pragma: no cover
+                params = [
+                    self._get_edb_value(value["Inner"]),
+                    self._get_edb_value(value["ChannelWidth"]),
+                    self._get_edb_value(value["IsolationGap"]),
+                ]
+            else:  # pragma: no cover
+                params = None
+        elif isinstance(value, list):
+            params = [self._get_edb_value(i) for i in value]
         else:
-            propertylist = [self._get_edb_value(i) for i in propertylist]
-        self._update_pad_parameters_parameters(params=propertylist)
+            params = [self._get_edb_value(value)]
+        self._update_pad_parameters_parameters(params=params)
 
     @property
     def offset_x(self):
         """Offset for the X axis.
 
         Returns
         -------
@@ -276,30 +336,32 @@
         """
         originalPadstackDefinitionData = self._edb_padstack.GetData()
         newPadstackDefinitionData = self._edb.Definition.PadstackDefData(originalPadstackDefinitionData)
         if not pad_type:
             pad_type = self.pad_type
         if not geom_type:
             geom_type = self.geometry_type
-        if not params:
-            params = [self._get_edb_value(i) for i in self.parameters]
+        if params:
+            params = convert_py_list_to_net_list(params)
+        else:
+            params = self._pad_parameter_value[2]
         if not offsetx:
             offsetx = self.offset_x
         if not offsety:
             offsety = self.offset_y
         if not rotation:
             rotation = self.rotation
         if not layer_name:
             layer_name = self.layer_name
 
         newPadstackDefinitionData.SetPadParameters(
             layer_name,
             self.int_to_pad_type(pad_type),
             self.int_to_geometry_type(geom_type),
-            convert_py_list_to_net_list(params),
+            params,
             self._get_edb_value(offsetx),
             self._get_edb_value(offsety),
             self._get_edb_value(rotation),
         )
         self._edb_padstack.SetData(newPadstackDefinitionData)
 
 
@@ -950,21 +1012,15 @@
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         if simple_check:
             pos = [i for i in self.position]
-            int_val = (
-                1
-                if polygon_data.PointInPolygon(
-                    self._pedb.edb.Geometry.PointData(self._pedb.edb_value(pos[0]), self._pedb.edb_value(pos[1]))
-                )
-                else 0
-            )
+            int_val = 1 if polygon_data.PointInPolygon(self._pedb.point_data(*pos)) else 0
         else:
             plane = self._pedb.modeler.Shape("rectangle", pointA=self.bounding_box[0], pointB=self.bounding_box[1])
             rectangle_data = self._pedb.modeler.shape_to_polygon_data(plane)
             int_val = polygon_data.GetIntersectionType(rectangle_data)
         # Intersection type:
         # 0 = objects do not intersect
         # 1 = this object fully inside other (no common contour points)
@@ -1441,22 +1497,23 @@
             * 4 Number of top/bottom association type.
             * -1 Undefined.
         """
         return int(self._edb_padstackinstance.GetGroup().GetPlacementLayer().GetTopBottomAssociation())
 
     @pyaedt_function_handler()
     def create_rectangle_in_pad(self, layer_name, return_points=False, partition_max_order=16):
-        """Create a rectangle inscribed inside a padstack instance pad. The rectangle is fully inscribed in the
-        pad and has the maximum area. It is necessary to specify the layer on which the rectangle will be created.
+        """Create a rectangle inscribed inside a padstack instance pad.
+
+        The rectangle is fully inscribed in the pad and has the maximum area.
+        It is necessary to specify the layer on which the rectangle will be created.
 
         Parameters
         ----------
         layer_name : str
             Name of the layer on which to create the polygon.
-
         return_points : bool, optional
             If `True` does not create the rectangle and just returns a list containing the rectangle vertices.
             Default is `False`.
         partition_max_order : float, optional
             Order of the lattice partition used to find the quasi-lattice polygon that approximates ``polygon``.
             Default is ``16``.
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,17 +35,21 @@
         self._use_default_coax_port_radial_extension = True
         self._trim_reference_size = False
         self._output_aedb = None
         self._signal_layers_properties = {}
         self._coplanar_instances = []
         self._signal_layer_etching_instances = []
         self._etching_factor_instances = []
-        self._dielectric_extent = 0.01
-        self._airbox_horizontal_extent = 0.04
+        self._use_dielectric_extent_multiple = True
+        self._dielectric_extent = 0.001
+        self._use_airbox_horizontal_multiple = True
+        self._airbox_horizontal_extent = 0.1
+        self._use_airbox_negative_vertical_extent_multiple = True
         self._airbox_negative_vertical_extent = 0.1
+        self._use_airbox_positive_vertical_extent_multiple = True
         self._airbox_positive_vertical_extent = 0.1
         self._honor_user_dielectric = False
         self._truncate_airbox_at_ground = False
         self._use_radiation_boundary = True
         self._do_cutout_subdesign = True
         self._do_pin_group = True
         self._sources = []
@@ -100,75 +104,149 @@
 
     @property
     def dielectric_extent(self):  # pragma: no cover
         """Retrieve the value of dielectric extent.
 
         Returns
         -------
-            float
-            Value of the dielectric extent.
+        float
+            Value of the dielectric extent. When absolute dimensions are used,
+            the values are in meters.
         """
         return self._dielectric_extent
 
     @dielectric_extent.setter
     def dielectric_extent(self, value):  # pragma: no cover
         if isinstance(value, (int, float)):
             self._dielectric_extent = value
 
     @property
+    def use_dielectric_extent_multiple(self):
+        """Whether the multiple value of the dielectric extent is used.
+
+        Returns
+        -------
+        bool
+           ``True`` when the multiple value (extent factor) is used. ``False`` when
+           absolute dimensions are used.
+        """
+        return self._use_dielectric_extent_multiple
+
+    @use_dielectric_extent_multiple.setter
+    def use_dielectric_extent_multiple(self, value):
+        if isinstance(value, bool):
+            self._use_dielectric_extent_multiple = value
+
+    @property
     def airbox_horizontal_extent(self):  # pragma: no cover
-        """Retrieve the air box horizontal extent size for HFSS.
+        """Horizontal extent of the airbox for HFSS. When absolute dimensions are used,
+        the values are in meters.
 
         Returns
         -------
             float
             Value of the air box horizontal extent.
         """
         return self._airbox_horizontal_extent
 
     @airbox_horizontal_extent.setter
     def airbox_horizontal_extent(self, value):  # pragma: no cover
         if isinstance(value, (int, float)):
             self._airbox_horizontal_extent = value
 
     @property
+    def use_airbox_horizontal_extent_multiple(self):
+        """Whether the multiple value is used for the horizontal extent of the air box.
+
+        Returns
+        -------
+        bool
+            ``True`` when the multiple value (extent factor) is used. ``False`` when
+            absolute dimensions are used.
+
+        """
+        return self._use_airbox_horizontal_multiple
+
+    @use_airbox_horizontal_extent_multiple.setter
+    def use_airbox_horizontal_extent_multiple(self, value):
+        if isinstance(value, bool):
+            self._use_airbox_horizontal_multiple = value
+
+    @property
     def airbox_negative_vertical_extent(self):  # pragma: no cover
-        """Retrieve the air box negative vertical extent size for HFSS.
+        """Negative vertical extent of the airbox for HFSS. When absolute dimensions
+        are used, the values are in meters.
 
         Returns
         -------
             float
             Value of the air box negative vertical extent.
         """
         return self._airbox_negative_vertical_extent
 
     @airbox_negative_vertical_extent.setter
     def airbox_negative_vertical_extent(self, value):  # pragma: no cover
         if isinstance(value, (int, float)):
             self._airbox_negative_vertical_extent = value
 
     @property
+    def use_airbox_negative_vertical_extent_multiple(self):
+        """Multiple value for the negative extent of the airbox.
+
+        Returns
+        -------
+        bool
+            ``True`` when the multiple value (extent factor) is used. ``False`` when
+            absolute dimensions are used.
+
+        """
+        return self._use_airbox_negative_vertical_extent_multiple
+
+    @use_airbox_negative_vertical_extent_multiple.setter
+    def use_airbox_negative_vertical_extent_multiple(self, value):
+        if isinstance(value, bool):
+            self._use_airbox_negative_vertical_extent_multiple = value
+
+    @property
     def airbox_positive_vertical_extent(self):  # pragma: no cover
-        """Retrieve the air box positive vertical extent size for HFSS.
+        """Positive vertical extent of the airbox for HFSS. When absolute dimensions are
+        used, the values are in meters.
 
         Returns
         -------
             float
             Value of the air box positive vertical extent.
         """
         return self._airbox_positive_vertical_extent
 
     @airbox_positive_vertical_extent.setter
     def airbox_positive_vertical_extent(self, value):  # pragma: no cover
         if isinstance(value, (int, float)):
             self._airbox_positive_vertical_extent = value
 
     @property
+    def use_airbox_positive_vertical_extent_multiple(self):
+        """Whether the multiple value for the positive extent of the airbox is used.
+
+        Returns
+        -------
+        bool
+            ``True`` when the multiple value (extent factor) is used. ``False`` when
+            absolute dimensions are used.
+        """
+        return self._use_airbox_positive_vertical_extent_multiple
+
+    @use_airbox_positive_vertical_extent_multiple.setter
+    def use_airbox_positive_vertical_extent_multiple(self, value):
+        if isinstance(value, bool):
+            self._use_airbox_positive_vertical_extent_multiple = value
+
+    @property
     def use_default_cutout(self):  # pragma: no cover
-        """Either if use the default EDB Cutout or new pyaedt cutout.
+        """Whether the default EDB cutout or a new PyAEDT cutout is used.
 
         Returns
         -------
         bool
         """
         return self._use_default_cutout
 
@@ -194,15 +272,15 @@
     @property
     def generate_solder_balls(self):  # pragma: no cover
         """Retrieve the boolean for applying solder balls.
 
         Returns
         -------
         bool
-            'True' when applied 'False' if not.
+            ``True`` when applied ``False`` if not.
         """
         return self._generate_solder_balls
 
     @generate_solder_balls.setter
     def generate_solder_balls(self, value):
         if isinstance(value, bool):  # pragma: no cover
             self._generate_solder_balls = value
@@ -275,15 +353,15 @@
     @property
     def use_default_coax_port_radial_extension(self):
         """Retrieve the boolean for using the default coaxial port extension value.
 
         Returns
         -------
         bool
-            'True' when the default value is used 'False' if not.
+            ``True`` when the default value is used ``False`` if not.
         """
         return self._use_default_coax_port_radial_extension
 
     @use_default_coax_port_radial_extension.setter
     def use_default_coax_port_radial_extension(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._use_default_coax_port_radial_extension = value
@@ -307,15 +385,15 @@
     @property
     def do_cutout_subdesign(self):
         """Retrieve boolean to perform the cutout during the project build.
 
         Returns
         -------
             bool
-            'True' when clipping the design is applied 'False' is not.
+            ``True`` when clipping the design is applied ``False`` is not.
         """
         return self._do_cutout_subdesign
 
     @do_cutout_subdesign.setter
     def do_cutout_subdesign(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._do_cutout_subdesign = value
@@ -337,15 +415,15 @@
 
     @property
     def cutout_subdesign_expansion(self):
         """Retrieve expansion factor used for clipping the design.
 
         Returns
         -------
-            float
+        float
             The value used as a ratio.
         """
 
         return self._cutout_subdesign_expansion
 
     @cutout_subdesign_expansion.setter
     def cutout_subdesign_expansion(self, value):  # pragma: no cover
@@ -353,16 +431,16 @@
 
     @property
     def cutout_subdesign_round_corner(self):
         """Retrieve boolean to perform the design clipping using round corner for the extent generation.
 
         Returns
         -------
-            bool
-            'True' when using round corner, 'False' if not.
+        bool
+            ``True`` when using round corner, ``False`` if not.
         """
 
         return self._cutout_subdesign_round_corner
 
     @cutout_subdesign_round_corner.setter
     def cutout_subdesign_round_corner(self, value):  # pragma: no cover
         if isinstance(value, bool):
@@ -373,15 +451,15 @@
         """Retrieve the path for the output aedb folder. When provided will copy the initial aedb to the specified
         path. This is used especially to preserve the initial project when several files have to be build based on
         the last one. When the path is None, the initial project will be overwritten. So when cutout is applied mand
         you want to preserve the project make sure you provide the full path for the new aedb folder.
 
         Returns
         -------
-            str
+        str
             Absolute path for the created aedb folder.
         """
         return self._output_aedb
 
     @output_aedb.setter
     def output_aedb(self, value):  # pragma: no cover
         if isinstance(value, str):
@@ -407,78 +485,75 @@
 
     @pyaedt_function_handler()
     def add_source(self, source=None):  # pragma: no cover
         """Add a new source to configuration.
 
         Parameters
         ----------
-        source :  :class:`pyaedt.edb_core.edb_data.sources.Source`
-
-        Returns
-        -------
+        source : :class:`pyaedt.edb_core.edb_data.sources.Source`
 
         """
         if isinstance(source, Source):
             self._sources.append(source)
 
     @property
     def honor_user_dielectric(self):  # pragma: no cover
         """Retrieve the boolean to activate the feature "'Honor user dielectric'".
 
         Returns
         -------
-            bool
-            "'True'" activated, "'False'" deactivated.
+        bool
+            ``True`` activated, ``False`` deactivated.
         """
         return self._honor_user_dielectric
 
     @honor_user_dielectric.setter
     def honor_user_dielectric(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._honor_user_dielectric = value
 
     @property
     def truncate_airbox_at_ground(self):  # pragma: no cover
         """Retrieve the boolean to truncate hfss air box at ground.
 
         Returns
         -------
-            bool
-            "'True'" activated, "'False'" deactivated.
+        bool
+            ``True`` activated, ``False`` deactivated.
         """
         return self._truncate_airbox_at_ground
 
     @truncate_airbox_at_ground.setter
     def truncate_airbox_at_ground(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._truncate_airbox_at_ground = value
 
     @property
     def use_radiation_boundary(self):  # pragma: no cover
         """Retrieve the boolean to use radiation boundary with HFSS.
 
         Returns
         -------
-            bool
-            "'True'" activated, "'False'" deactivated.
+        bool
+            ``True`` activated, ``False`` deactivated.
         """
         return self._use_radiation_boundary
 
     @use_radiation_boundary.setter
     def use_radiation_boundary(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._use_radiation_boundary = value
 
     @property
     def signal_layers_properties(self):  # pragma: no cover
         """Retrieve the list of layers to have properties changes.
 
         Returns
         -------
-            list[str]
+        list[str]
             List of layer name.
         """
         return self._signal_layers_properties
 
     @signal_layers_properties.setter
     def signal_layers_properties(self, value):  # pragma: no cover
         if isinstance(value, dict):
@@ -525,15 +600,15 @@
 
     @property
     def dc_min_plane_area_to_mesh(self):  # pragma: no cover
         """Retrieve the value of the minimum plane area to be meshed by Siwave for DC solution.
 
         Returns
         -------
-            float
+        float
             The value of the minimum plane area.
         """
         return self._dc_min_plane_area_to_mesh
 
     @dc_min_plane_area_to_mesh.setter
     def dc_min_plane_area_to_mesh(self, value):  # pragma: no cover
         if isinstance(value, str):
@@ -541,31 +616,31 @@
 
     @property
     def dc_compute_inductance(self):
         """Return the boolean for computing the inductance with SIwave DC solver.
 
         Returns
         -------
-            bool
-            'True' activate 'False' deactivated.
+        bool
+            ``True`` activate ``False`` deactivated.
         """
         return self._dc_compute_inductance
 
     @dc_compute_inductance.setter
     def dc_compute_inductance(self, value):
         if isinstance(value, bool):
             self._dc_compute_inductance = value
 
     @property
     def dc_contact_radius(self):
         """Retrieve the value for SIwave DC contact radius.
 
         Returns
         -------
-            str
+        str
             The contact radius value.
 
         """
         return self._dc_contact_radius
 
     @dc_contact_radius.setter
     def dc_contact_radius(self, value):
@@ -579,15 +654,15 @@
 
     @property
     def dc_slide_position(self):
         """Retrieve the SIwave DC slide position value.
 
         Returns
         -------
-            int
+        int
             The position value, 0 Optimum speed, 1 balanced, 2 optimum accuracy.
         """
         return self._dc_slide_position
 
     @dc_slide_position.setter
     def dc_slide_position(self, value):
         if isinstance(value, int):
@@ -595,16 +670,16 @@
 
     @property
     def dc_use_dc_custom_settings(self):
         """Retrieve the value for using DC custom settings.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_use_dc_custom_settings
 
     @dc_use_dc_custom_settings.setter
     def dc_use_dc_custom_settings(self, value):
         if isinstance(value, bool):
@@ -612,16 +687,16 @@
 
     @property
     def dc_plot_jv(self):
         """Retrieve the value for computing current density and voltage distribution.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated. Default value True
+        bool
+            ``True`` when activated, ``False`` deactivated. Default value True
 
         """
         return self._dc_plot_jv
 
     @dc_plot_jv.setter
     def dc_plot_jv(self, value):
         if isinstance(value, bool):
@@ -629,15 +704,15 @@
 
     @property
     def dc_min_void_area_to_mesh(self):
         """Retrieve the value for the minimum void surface to mesh.
 
         Returns
         -------
-            str
+        str
             The area value.
 
         """
         return self._dc_min_void_area_to_mesh
 
     @dc_min_void_area_to_mesh.setter
     def dc_min_void_area_to_mesh(self, value):
@@ -646,15 +721,15 @@
 
     @property
     def dc_error_energy(self):
         """Retrieve the value for the DC error energy.
 
         Returns
         -------
-            float
+        float
             The error energy value, 0.2 as default.
 
         """
         return self._dc_error_energy
 
     @dc_error_energy.setter
     def dc_error_energy(self, value):
@@ -663,15 +738,15 @@
 
     @property
     def dc_max_init_mesh_edge_length(self):
         """Retrieve the maximum initial mesh edge value.
 
         Returns
         -------
-            str
+        str
             maximum mesh length.
 
         """
         return self._dc_max_init_mesh_edge_length
 
     @dc_max_init_mesh_edge_length.setter
     def dc_max_init_mesh_edge_length(self, value):
@@ -680,15 +755,15 @@
 
     @property
     def dc_max_num_pass(self):
         """Retrieve the maximum number of adaptive passes.
 
         Returns
         -------
-            int
+        int
             number of passes.
         """
         return self._dc_max_num_pass
 
     @dc_max_num_pass.setter
     def dc_max_num_pass(self, value):
         if isinstance(value, int):
@@ -696,15 +771,15 @@
 
     @property
     def dc_min_num_pass(self):
         """Retrieve the minimum number of adaptive passes.
 
         Returns
         -------
-            nt
+        int
             number of passes.
         """
         return self._dc_min_num_pass
 
     @dc_min_num_pass.setter
     def dc_min_num_pass(self, value):
         if isinstance(value, int):
@@ -712,16 +787,16 @@
 
     @property
     def dc_mesh_bondwires(self):
         """Retrieve the value for meshing bondwires.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_mesh_bondwires
 
     @dc_mesh_bondwires.setter
     def dc_mesh_bondwires(self, value):
         if isinstance(value, bool):
@@ -729,15 +804,15 @@
 
     @property
     def dc_num_bondwire_sides(self):
         """Retrieve the number of sides used for cylinder discretization.
 
         Returns
         -------
-            int
+        int
             Number of sides.
 
         """
         return self._dc_num_bondwire_sides
 
     @dc_num_bondwire_sides.setter
     def dc_num_bondwire_sides(self, value):
@@ -746,16 +821,16 @@
 
     @property
     def dc_mesh_vias(self):
         """Retrieve the value for meshing vias.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_mesh_vias
 
     @dc_mesh_vias.setter
     def dc_mesh_vias(self, value):
         if isinstance(value, bool):
@@ -763,15 +838,15 @@
 
     @property
     def dc_num_via_sides(self):
         """Retrieve the number of sides used for cylinder discretization.
 
         Returns
         -------
-            int
+        int
             Number of sides.
 
         """
         return self._dc_num_via_sides
 
     @dc_num_via_sides.setter
     def dc_num_via_sides(self, value):
@@ -780,15 +855,15 @@
 
     @property
     def dc_percent_local_refinement(self):
         """Retrieve the value for local mesh refinement.
 
         Returns
         -------
-            float
+        float
             The refinement value, 0.2 (20%) as default.
 
         """
         return self._dc_percent_local_refinement
 
     @dc_percent_local_refinement.setter
     def dc_percent_local_refinement(self, value):
@@ -797,16 +872,16 @@
 
     @property
     def dc_perform_adaptive_refinement(self):
         """Retrieve the value for performing adaptive meshing.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_perform_adaptive_refinement
 
     @dc_perform_adaptive_refinement.setter
     def dc_perform_adaptive_refinement(self, value):
         if isinstance(value, bool):
@@ -814,16 +889,16 @@
 
     @property
     def dc_refine_bondwires(self):
         """Retrieve the value for performing bond wire refinement.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_refine_bondwires
 
     @dc_refine_bondwires.setter
     def dc_refine_bondwires(self, value):
         if isinstance(value, bool):
@@ -831,16 +906,16 @@
 
     @property
     def dc_refine_vias(self):
         """Retrieve the value for performing vias refinement.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_refine_vias
 
     @dc_refine_vias.setter
     def dc_refine_vias(self, value):
         if isinstance(value, bool):
@@ -848,15 +923,15 @@
 
     @property
     def dc_report_config_file(self):
         """Retrieve the report configuration file path.
 
         Returns
         -------
-            str
+        str
             The file path.
 
         """
         return self._dc_report_config_file
 
     @dc_report_config_file.setter
     def dc_report_config_file(self, value):
@@ -865,16 +940,16 @@
 
     @property
     def dc_report_show_Active_devices(self):
         """Retrieve the value for showing active devices.
 
         Returns
         -------
-            bool
-            'True' when activated, 'False' deactivated.
+        bool
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_report_show_Active_devices
 
     @dc_report_show_Active_devices.setter
     def dc_report_show_Active_devices(self, value):
         if isinstance(value, bool):
@@ -883,15 +958,15 @@
     @property
     def dc_export_thermal_data(self):
         """Retrieve the value for using external data.
 
         Returns
         -------
             bool
-            'True' when activated, 'False' deactivated.
+            ``True`` when activated, ``False`` deactivated.
 
         """
         return self._dc_export_thermal_data
 
     @dc_export_thermal_data.setter
     def dc_export_thermal_data(self, value):
         if isinstance(value, bool):
@@ -933,15 +1008,15 @@
     @property
     def dc_import_thermal_data(self):
         """Retrieve the value for importing thermal data.
 
         Returns
         -------
             bool
-            'True' when activated,'False' deactivated.
+            ``True`` when activated,``False`` deactivated.
 
         """
         return self._dc_import_thermal_data
 
     @dc_import_thermal_data.setter
     def dc_import_thermal_data(self, value):
         if isinstance(value, bool):
@@ -1086,15 +1161,15 @@
     @property
     def sweep_interpolating(self):  # pragma: no cover
         """Retrieve boolean to add a sweep interpolating sweep.
 
         Returns
         -------
             bool
-            'True' when a sweep interpolating is defined, 'False' when a discrete one is defined instead.
+            ``True`` when a sweep interpolating is defined, ``False`` when a discrete one is defined instead.
         """
 
         return self._sweep_interpolating
 
     @sweep_interpolating.setter
     def sweep_interpolating(self, value):  # pragma: no cover
         if isinstance(value, bool):
@@ -1103,15 +1178,15 @@
     @property
     def use_q3d_for_dc(self):  # pragma: no cover
         """Retrieve boolean to Q3D solver for DC point value computation.
 
         Returns
         -------
             bool
-            'True' when Q3D solver is used 'False' when interpolating value is used instead.
+            ``True`` when Q3D solver is used ``False`` when interpolating value is used instead.
         """
 
         return self._use_q3d_for_dc
 
     @use_q3d_for_dc.setter
     def use_q3d_for_dc(self, value):  # pragma: no cover
         if isinstance(value, bool):
@@ -1154,15 +1229,15 @@
     @property
     def percentage_error_z0(self):  # pragma: no cover
         """Retrieve boolean to perform the cutout during the project build.
 
         Returns
         -------
             bool
-            'True' when clipping the design is applied 'False' if not.
+            ``True`` when clipping the design is applied ``False`` if not.
         """
 
         return self._percentage_error_z0
 
     @percentage_error_z0.setter
     def percentage_error_z0(self, value):  # pragma: no cover
         if isinstance(value, (int, float)):
@@ -1171,15 +1246,15 @@
     @property
     def enforce_causality(self):  # pragma: no cover
         """Retrieve boolean to enforce causality for the frequency sweep.
 
         Returns
         -------
             bool
-            'True' when causality is enforced 'False' if not.
+            ``True`` when causality is enforced ``False`` if not.
         """
 
         return self._enforce_causality
 
     @enforce_causality.setter
     def enforce_causality(self, value):  # pragma: no cover
         if isinstance(value, bool):
@@ -1188,15 +1263,15 @@
     @property
     def enforce_passivity(self):  # pragma: no cover
         """Retrieve boolean to enforce passivity for the frequency sweep.
 
         Returns
         -------
             bool
-            'True' when passivity is enforced 'False' if not.
+            ``True`` when passivity is enforced ``False`` if not.
         """
         return self._enforce_passivity
 
     @enforce_passivity.setter
     def enforce_passivity(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._enforce_passivity = value
@@ -1412,15 +1487,15 @@
     @property
     def do_lambda_refinement(self):  # pragma: no cover
         """Retrieve boolean to activate the lambda refinement.
 
         Returns
         -------
             bool
-            'True' Enable the lambda meshing refinement with HFSS, 'False' deactivate.
+            ``True`` Enable the lambda meshing refinement with HFSS, ``False`` deactivate.
         """
         return self._do_lambda_refinement
 
     @do_lambda_refinement.setter
     def do_lambda_refinement(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._do_lambda_refinement = value
@@ -1476,15 +1551,15 @@
     @property
     def use_arc_to_chord_error(self):  # pragma: no cover
         """Retrieve the boolean for activating the arc to chord for HFSS meshing.
 
         Returns
         -------
             bool
-            Activate when 'True', deactivated when 'False'.
+            Activate when ``True``, deactivated when ``False``.
         """
         return self._use_arc_to_chord_error
 
     @use_arc_to_chord_error.setter
     def use_arc_to_chord_error(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._use_arc_to_chord_error = value
@@ -1526,15 +1601,15 @@
         """Retrieve the boolean to activate the layout defeaturing.This method has been developed to simplify polygons
         with reducing the number of points to simplify the meshing with controlling its surface deviation. This method
         should be used at last resort when other methods failed.
 
         Returns
         -------
             bool
-            'True' when activated 'False when deactivated.
+            ``True`` when activated 'False when deactivated.
         """
         return self._defeature_layout
 
     @defeature_layout.setter
     def defeature_layout(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._defeature_layout = value
@@ -1623,15 +1698,15 @@
     @property
     def include_inter_plane_coupling(self):  # pragma: no cover
         """Boolean to activate the inter-plane coupling with Siwave.
 
         Returns
         -------
             bool
-            'True' activated 'False' deactivated.
+            ``True`` activated ``False`` deactivated.
         """
         return self._include_inter_plane_coupling
 
     @include_inter_plane_coupling.setter
     def include_inter_plane_coupling(self, value):  # pragma: no cover
         if isinstance(value, bool):
             self._include_inter_plane_coupling = value
@@ -1689,15 +1764,15 @@
     @property
     def snap_length_threshold(self):  # pragma: no cover
         """Retrieve the boolean to activate the snapping threshold feature.
 
         Returns
         -------
             bool
-            'True' activate 'False' deactivated.
+            ``True`` activate ``False`` deactivated.
         """
         return self._snap_length_threshold
 
     @snap_length_threshold.setter
     def snap_length_threshold(self, value):  # pragma: no cover
         if isinstance(value, str):
             self._snap_length_threshold = value
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,41 +143,38 @@
         - Plane edges that form a narrow trace-like plane.
         The former leads to crosstalk between adjacent planes for which
         a specific coupling model is applied. For the latter, fringing effects
         are considered to model accurately the propagation characteristics
         of trace-like cavities. Further, the coupling between narrow planes is
         also modeled by enabling this feature.
 
-
         Returns
         -------
         bool
             ``True`` if split plane coupling is used, ``False`` otherwise.
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.IncludeSplitPlaneCoupling
 
     @property
     def include_infinite_ground(self):
         """Whether to Include a ground plane to serve as a voltage reference for traces and planes
         if they are not defined in the layout.
 
-
         Returns
         -------
         bool
             ``True`` if infinite ground is used, ``False`` otherwise.
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.IncludeInfGnd
 
     @property
     def include_trace_coupling(self):
         """Whether to model coupling between adjacent traces.
         Coupling is considered for parallel and almost parallel trace segments.
 
-
         Returns
         -------
         bool
             ``True`` if trace coupling is used, ``False`` otherwise.
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.IncludeTraceCoupling
 
@@ -193,26 +190,24 @@
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.IncludeVISources
 
     @property
     def infinite_ground_location(self):
         """Elevation of the infinite unconnected ground plane placed under the design.
 
-
         Returns
         -------
         str
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.InfGndLocation
 
     @property
     def max_coupled_lines(self):
         """Maximum number of coupled lines to build the new coupled transmission line model.
 
-
         Returns
         -------
         int
         """
         return self.sim_setup_info.SimulationSettings.AdvancedSettings.MaxCoupledLines
 
     @property
@@ -992,15 +987,15 @@
 
     @property
     def source_terms_to_ground(self):
         """Dictionary of grounded terminals.
 
         Returns
         -------
-            Dictionary
+        Dictionary
             {str, int}, keys is source name, value int 0 unspecified, 1 negative node, 2 positive one.
 
         """
         return convert_netdict_to_pydict(self._edb_sim_setup_info.SimulationSettings.DCIRSettings.SourceTermsToGround)
 
     @pyaedt_function_handler()
     def add_source_terminal_to_ground(self, source_name, terminal=0):
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/sources.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.72/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/general.py` & `pyaedt-0.6.72/pyaedt/edb_core/general.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,19 +3,28 @@
 
 """
 
 from __future__ import absolute_import  # noreorder
 
 import logging
 
+from pyaedt import is_ironpython
 from pyaedt.generic.clr_module import Dictionary
 from pyaedt.generic.clr_module import List
 from pyaedt.generic.clr_module import Tuple
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
+if not is_ironpython:  # pragma: no cover
+    try:
+        from enum import Enum
+    except ImportError:
+        Enum = None
+else:  # pragma: no cover
+    Enum = object
+
 logger = logging.getLogger(__name__)
 
 
 @pyaedt_function_handler()
 def convert_netdict_to_pydict(dict_in):
     """Convert a net dictionary to a Python dictionary.
 
@@ -114,7 +123,29 @@
     list
         List converted to Python.
     """
     pylist = []
     for el in netlist:
         pylist.__add__(el)
     return pylist
+
+
+class PadGeometryTpe(Enum):  # pragma: no cover
+    Circle = 1
+    Square = 2
+    Rectangle = 3
+    Oval = 4
+    Bullet = 5
+    NSidedPolygon = 6
+    Polygon = 7
+    Round45 = 8
+    Round90 = 9
+    Square45 = 10
+    Square90 = 11
+    InvalidGeometry = 12
+
+
+class DielectricExtentType(Enum):
+    BoundingBox = 0
+    Conforming = 1
+    ConvexHull = 2
+    Polygon = 3
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.72/pyaedt/edb_core/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This module contains the ``EdbHfss`` class.
 """
 import math
 
+from pyaedt.edb_core.edb_data.hfss_extent_info import HfssExtentInfo
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.edb_data.simulation_configuration import SimulationConfiguration
 from pyaedt.edb_core.edb_data.sources import ExcitationBundle
 from pyaedt.edb_core.edb_data.sources import ExcitationDifferential
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
 from pyaedt.generic.constants import RadiationBoxType
@@ -27,19 +28,30 @@
     >>> edb_hfss = edb_3dedbapp.hfss
     """
 
     def __init__(self, p_edb):
         self._pedb = p_edb
 
     @property
+    def hfss_extent_info(self):
+        """HFSS extent information."""
+        return HfssExtentInfo(self._pedb)
+
+    @property
     def _logger(self):
         return self._pedb.logger
 
     @property
     def _edb(self):
+        """EDB object.
+
+        Returns
+        -------
+        Ansys.Ansoft.Edb
+        """
         return self._pedb.edb
 
     @property
     def _active_layout(self):
         return self._pedb.active_layout
 
     @property
@@ -1067,23 +1079,31 @@
         hfss_extent = self._edb.Utility.HFSSExtentInfo()
         if simulation_setup.radiation_box == RadiationBoxType.BoundingBox:
             hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.BoundingBox
         elif simulation_setup.radiation_box == RadiationBoxType.Conformal:
             hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.Conforming
         else:
             hfss_extent.ExtentType = self._edb.Utility.HFSSExtentInfoType.ConvexHull
-        hfss_extent.DielectricExtentSize = convert_pytuple_to_nettuple((simulation_setup.dielectric_extent, True))
+        hfss_extent.DielectricExtentSize = convert_pytuple_to_nettuple(
+            (simulation_setup.dielectric_extent, simulation_setup.use_dielectric_extent_multiple)
+        )
         hfss_extent.AirBoxHorizontalExtent = convert_pytuple_to_nettuple(
-            (simulation_setup.airbox_horizontal_extent, True)
+            (simulation_setup.airbox_horizontal_extent, simulation_setup.use_airbox_horizontal_extent_multiple)
         )
         hfss_extent.AirBoxNegativeVerticalExtent = convert_pytuple_to_nettuple(
-            (simulation_setup.airbox_negative_vertical_extent, True)
+            (
+                simulation_setup.airbox_negative_vertical_extent,
+                simulation_setup.use_airbox_negative_vertical_extent_multiple,
+            )
         )
         hfss_extent.AirBoxPositiveVerticalExtent = convert_pytuple_to_nettuple(
-            (simulation_setup.airbox_positive_vertical_extent, True)
+            (
+                simulation_setup.airbox_positive_vertical_extent,
+                simulation_setup.use_airbox_positive_vertical_extent_multiple,
+            )
         )
         hfss_extent.HonorUserDielectric = simulation_setup.honor_user_dielectric
         hfss_extent.TruncateAirBoxAtGround = simulation_setup.truncate_airbox_at_ground
         hfss_extent.UseOpenRegion = simulation_setup.use_radiation_boundary
         self._active_layout.GetCell().SetHFSSExtentInfo(hfss_extent)  # returns void
         return True
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.72/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/layout.py` & `pyaedt-0.6.72/pyaedt/edb_core/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -352,17 +352,17 @@
             try:
                 point = poligon_data.GetPoint(i)
                 if prev_point != point:
                     check_inside = selection_polygon_data.PointInPolygon(point)
                     if check_inside:
                         xcoeff, ycoeff = calc_slope([point.X.ToDouble(), point.X.ToDouble()], origin)
 
-                        new_points = self._edb.Geometry.PointData(
-                            self._get_edb_value(point.X.ToString() + "{}*{}".format(xcoeff, offset_name)),
-                            self._get_edb_value(point.Y.ToString() + "{}*{}".format(ycoeff, offset_name)),
+                        new_points = self._pedb.point_data(
+                            point.X.ToString() + "{}*{}".format(xcoeff, offset_name),
+                            point.Y.ToString() + "{}*{}".format(ycoeff, offset_name),
                         )
                         poligon_data.SetPoint(i, new_points)
                     prev_point = point
                     i += 1
                 else:
                     continue_iterate = False
             except:
@@ -427,17 +427,15 @@
         if corner_style.lower() == "round":
             corner_style = self._edb.Cell.Primitive.PathCornerStyle.RoundCorner
         elif corner_style.lower() == "sharp":
             corner_style = self._edb.Cell.Primitive.PathCornerStyle.SharpCorner  # pragma: no cover
         else:
             corner_style = self._edb.Cell.Primitive.PathCornerStyle.MiterCorner  # pragma: no cover
 
-        pointlists = [
-            self._edb.Geometry.PointData(self._get_edb_value(i[0]), self._get_edb_value(i[1])) for i in path_list.points
-        ]
+        pointlists = [self._pedb.point_data(i[0], i[1]) for i in path_list.points]
         polygonData = self._edb.Geometry.PolygonData(convert_py_list_to_net_list(pointlists), False)
         polygon = self._edb.Cell.Primitive.Path.Create(
             self._active_layout,
             layer_name,
             net,
             self._get_edb_value(width),
             start_cap_style,
@@ -864,22 +862,16 @@
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
                     or endPoint[0].IsParametric()
                     or endPoint[1].IsParametric()
                 )
                 arc = self._edb.Geometry.ArcData(
-                    self._edb.Geometry.PointData(
-                        self._get_edb_value(startPoint[0].ToDouble()),
-                        self._get_edb_value(startPoint[1].ToDouble()),
-                    ),
-                    self._edb.Geometry.PointData(
-                        self._get_edb_value(endPoint[0].ToDouble()),
-                        self._get_edb_value(endPoint[1].ToDouble()),
-                    ),
+                    self._pedb.point_data(startPoint[0], startPoint[1]),
+                    self._pedb.point_data(endPoint[0], endPoint[1]),
                 )
                 arcs.append(arc)
             elif len(endPoint) == 5:
                 is_parametric = (
                     is_parametric
                     or startPoint[0].IsParametric()
                     or startPoint[1].IsParametric()
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/materials.py` & `pyaedt-0.6.72/pyaedt/edb_core/materials.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/nets.py` & `pyaedt-0.6.72/pyaedt/edb_core/nets.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.72/pyaedt/edb_core/padstack.py`

 * *Files 2% similar despite different names*

```diff
@@ -749,16 +749,14 @@
         """
         warnings.warn("Use :func:`create` method instead.", DeprecationWarning)
         return self.create(
             padstackname=padstackname,
             holediam=holediam,
             paddiam=paddiam,
             antipaddiam=antipaddiam,
-            startlayer=startlayer,
-            endlayer=endlayer,
             antipad_shape=antipad_shape,
             x_size=x_size,
             y_size=y_size,
             corner_radius=corner_radius,
             offset_x=offset_x,
             offset_y=offset_y,
             rotation=rotation,
@@ -771,16 +769,14 @@
     @pyaedt_function_handler()
     def create(
         self,
         padstackname=None,
         holediam="300um",
         paddiam="400um",
         antipaddiam="600um",
-        startlayer=None,
-        endlayer=None,
         pad_shape="Circle",
         antipad_shape="Circle",
         x_size="600um",
         y_size="600um",
         corner_radius="300um",
         offset_x="0.0",
         offset_y="0.0",
@@ -798,20 +794,14 @@
             Name of the padstack. The default is ``None``.
         holediam : str, optional
             Diameter of the hole with units. The default is ``"300um"``.
         paddiam : str, optional
             Diameter of the pad with units. The default is ``"400um"``.
         antipaddiam : str, optional
             Diameter of the antipad with units. The default is ``"600um"``.
-        startlayer : str, optional
-            Starting layer. The default is ``None``, in which case the top
-            is the starting layer.
-        endlayer : str, optional
-            Ending layer. The default is ``None``, in which case the bottom
-            is the ending layer.
         pad_shape : str, optional
             Shape of the pad. The default is ``"Circle``. Options are ``"Circle"`` and ``"Rectangle"``.
         antipad_shape : str, optional
             Shape of the antipad. The default is ``"Circle"``. Options are ``"Circle"`` and ``"Bullet"``.
         x_size : str, optional
             Only applicable to bullet shape. The default is ``"600um"``.
         y_size : str, optional
@@ -865,18 +855,15 @@
 
         padstackData.SetHoleParameters(ptype, holparam, value0, value0, value0)
 
         padstackData.SetHolePlatingPercentage(self._get_edb_value(20.0))
         padstackData.SetHoleRange(self._edb.Definition.PadstackHoleRange.UpperPadToLowerPad)
         padstackData.SetMaterial("copper")
         layers = list(self._pedb.stackup.signal_layers.keys())
-        if not startlayer:
-            startlayer = layers[0]
-        if not endlayer:
-            endlayer = layers[len(layers) - 1]
+
         if pad_shape == "Circle":
             pad_array = Array[type(paddiam)]([paddiam])
             pad_shape = self._edb.Definition.PadGeometryType.Circle
         elif pad_shape == "Rectangle":
             pad_array = Array[type(x_size)]([x_size, y_size])
             pad_shape = self._edb.Definition.PadGeometryType.Rectangle
         if antipad_shape == "Bullet":
@@ -904,21 +891,14 @@
                 antipad_shape,
                 antipad_array,
                 offset_x,
                 offset_y,
                 rotation,
             )
 
-        padstackLayerIdMap = {k: v for k, v in zip(padstackData.GetLayerNames(), padstackData.GetLayerIds())}
-        padstackLayerMap = self._edb.Utility.LayerMap(self._edb.Utility.UniqueDirection.ForwardUnique)
-        for layer, padstackLayerName in zip(
-            self._active_layout.GetLayerCollection().Layers(self._edb.Cell.LayerTypeSet.SignalLayerSet),
-            [startlayer, "Default", endlayer],
-        ):
-            padstackLayerMap.SetMapping(layer.GetLayerId(), padstackLayerIdMap[padstackLayerName])
         padstackDefinition = self._edb.Definition.PadstackDef.Create(self.db, padstackname)
         padstackDefinition.SetData(padstackData)
         self._logger.info("Padstack %s create correctly", padstackname)
         return padstackname
 
     @pyaedt_function_handler()
     def _get_pin_layer_range(self, pin):
```

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.72/pyaedt/edb_core/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.72/pyaedt/edb_core/stackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,38 @@
         Returns
         -------
         type
             Types of layers.
         """
         return self._pedb.edb.Cell.LayerType
 
+    @property
+    def thickness(self):
+        """Retrieve Stackup thickness.
+
+        Returns
+        -------
+        float
+            Layout stackup thickness.
+
+        """
+        return self.get_layout_thickness()
+
+    @property
+    def num_layers(self):
+        """Retrieve the stackup layer number.
+
+        Returns
+        -------
+        int
+            layer number.
+
+        """
+        return len(list(self.stackup_layers.keys()))
+
     @pyaedt_function_handler()
     def _int_to_layer_types(self, val):
         if int(val) == 0:
             return self.layer_types.SignalLayer
         elif int(val) == 1:
             return self.layer_types.DielectricLayer
         elif int(val) == 2:
@@ -1007,19 +1031,20 @@
         """Return the layout thickness.
 
         Returns
         -------
         float
             The thickness value.
         """
-        layers_name = list(self.stackup_layers.keys())
-        bottom_layer = self.stackup_layers[layers_name[0]]
-        top_layer = self.stackup_layers[layers_name[-1]]
-        thickness = top_layer.lower_elevation + top_layer.thickness - bottom_layer.lower_elevation
-        return thickness
+        layers = list(self.stackup_layers.values())
+        layers.sort(key=lambda lay: lay.lower_elevation)
+        top_layer = layers[-1]
+        bottom_layer = layers[0]
+        thickness = abs(top_layer.upper_elevation - bottom_layer.lower_elevation)
+        return round(thickness, 7)
 
     @pyaedt_function_handler()
     def _get_solder_height(self, layer_name):
         for _, val in self._pedb.components.components.items():
             if val.solder_ball_height and val.placement_layer == layer_name:
                 return val.solder_ball_height
         return 0
@@ -1289,20 +1314,18 @@
             elevation = target_bottom_elevation - source_stack_top_elevation
             solder_height = -solder_height
 
         h_stackup = self._edb_value(elevation + solder_height)
 
         zero_data = self._edb_value(0.0)
         one_data = self._edb_value(1.0)
-        point3d_t = self._pedb.edb.Geometry.Point3DData(_offset_x, _offset_y, h_stackup)
-        point_loc = self._pedb.edb.Geometry.Point3DData(zero_data, zero_data, zero_data)
-        point_from = self._pedb.edb.Geometry.Point3DData(one_data, zero_data, zero_data)
-        point_to = self._pedb.edb.Geometry.Point3DData(
-            self._edb_value(math.cos(_angle)), self._edb_value(-1 * math.sin(_angle)), zero_data
-        )
+        point3d_t = self._pedb.point_3d(_offset_x, _offset_y, h_stackup)
+        point_loc = self._pedb.point_3d(zero_data, zero_data, zero_data)
+        point_from = self._pedb.point_3d(one_data, zero_data, zero_data)
+        point_to = self._pedb.point_3d(math.cos(_angle), -1 * math.sin(_angle), zero_data)
         cell_inst2.Set3DTransformation(point_loc, point_from, point_to, rotation, point3d_t)
         self.refresh_layer_collection()
         return True
 
     @pyaedt_function_handler()
     def place_instance(
         self,
@@ -1435,20 +1458,18 @@
             elevation = target_bottom_elevation - source_stack_top_elevation
             solder_height = -solder_height
 
         h_stackup = self._edb_value(elevation + solder_height)
 
         zero_data = self._edb_value(0.0)
         one_data = self._edb_value(1.0)
-        point3d_t = self._pedb.edb.Geometry.Point3DData(_offset_x, _offset_y, h_stackup)
-        point_loc = self._pedb.edb.Geometry.Point3DData(zero_data, zero_data, zero_data)
-        point_from = self._pedb.edb.Geometry.Point3DData(one_data, zero_data, zero_data)
-        point_to = self._pedb.edb.Geometry.Point3DData(
-            self._edb_value(math.cos(_angle)), self._edb_value(-1 * math.sin(_angle)), zero_data
-        )
+        point3d_t = self._pedb.point_3d(_offset_x, _offset_y, h_stackup)
+        point_loc = self._pedb.point_3d(zero_data, zero_data, zero_data)
+        point_from = self._pedb.point_3d(one_data, zero_data, zero_data)
+        point_to = self._pedb.point_3d(math.cos(_angle), -1 * math.sin(_angle), zero_data)
         cell_inst2.Set3DTransformation(point_loc, point_from, point_to, rotation, point3d_t)
         self.refresh_layer_collection()
         return True
 
     @pyaedt_function_handler()
     def place_a3dcomp_3d_placement(self, a3dcomp_path, angle=0.0, offset_x=0.0, offset_y=0.0, place_on_top=True):
         """Place a 3D Component into current layout.
@@ -1482,34 +1503,32 @@
         >>> a3dcomp_path = "connector.a3dcomp"
         >>> edb1.stackup.place_a3dcomp_3d_placement(a3dcomp_path, angle=0.0, offset_x="1mm",
         ...                                   offset_y="2mm", flipped_stackup=False, place_on_top=True,
         ...                                   )
         """
         zero_data = self._edb_value(0.0)
         one_data = self._edb_value(1.0)
-        local_origin = self._pedb.edb.Geometry.Point3DData(zero_data, zero_data, zero_data)
-        rotation_axis_from = self._pedb.edb.Geometry.Point3DData(one_data, zero_data, zero_data)
+        local_origin = self._pedb.point_3d(0.0, 0.0, 0.0)
+        rotation_axis_from = self._pedb.point_3d(1.0, 0.0, 0.0)
         _angle = angle * math.pi / 180.0
-        rotation_axis_to = self._pedb.edb.Geometry.Point3DData(
-            self._edb_value(math.cos(_angle)), self._edb_value(-1 * math.sin(_angle)), zero_data
-        )
+        rotation_axis_to = self._pedb.point_3d(math.cos(_angle), -1 * math.sin(_angle), 0.0)
 
         stackup_target = self._pedb.edb.Cell.LayerCollection(self._pedb.active_layout.GetLayerCollection())
         sig_set = self._pedb.edb.Cell.LayerTypeSet.SignalLayerSet
         res = stackup_target.GetTopBottomStackupLayers(sig_set)
         target_top_elevation = res[2]
         target_bottom_elevation = res[4]
         flip_angle = self._edb_value("0deg")
         if place_on_top:
             elevation = target_top_elevation
         else:
             flip_angle = self._edb_value("180deg")
             elevation = target_bottom_elevation
         h_stackup = self._edb_value(elevation)
-        location = self._pedb.edb.Geometry.Point3DData(self._edb_value(offset_x), self._edb_value(offset_y), h_stackup)
+        location = self._pedb.point_3d(offset_x, offset_y, h_stackup)
 
         mcad_model = self._pedb.edb.McadModel.Create3DComp(self._pedb.active_layout, a3dcomp_path)
         if mcad_model.IsNull():  # pragma: no cover
             logger.error("Failed to create MCAD model from a3dcomp")
             return False
 
         cell_instance = mcad_model.GetCellInstance()
```

### Comparing `pyaedt-0.6.71/pyaedt/emit.py` & `pyaedt-0.6.72/pyaedt/emit.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from __future__ import absolute_import
 
-import sys
 import warnings
 
+from pyaedt import emit_core
 from pyaedt import generate_unique_project_name
 from pyaedt.application.Design import Design
-from pyaedt.emit_core import EMIT_MODULE
 from pyaedt.emit_core import EmitConstants
 from pyaedt.emit_core.Couplings import CouplingsEmit
 from pyaedt.emit_core.results.results import Results
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.schematic import ModelerEmit
 
 
@@ -119,23 +118,15 @@
     ):
         if projectname is None:
             projectname = generate_unique_project_name()
         self.__emit_api_enabled = False
         self.results = None
         """Constructor for the ``FieldAnalysisEmit`` class"""
 
-        self._units = {
-            "Power": "dBm",
-            "Frequency": "MHz",
-            "Length": "meter",
-            "Time": "ns",
-            "Voltage": "mV",
-            "Data Rate": "bps",
-            "Resistance": "ohm",
-        }
+        self._units = {}
         """Default Emit units."""
 
         Design.__init__(
             self,
             "EMIT",
             projectname,
             designname,
@@ -147,23 +138,33 @@
             student_version,
             machine=machine,
             port=port,
             aedt_process_id=aedt_process_id,
         )
         self._modeler = ModelerEmit(self)
         self._couplings = CouplingsEmit(self)
-        if self._aedt_version >= "2023.1" and sys.version_info.major == 3 and sys.version_info.minor == 7:
-            self._emit_api = EMIT_MODULE.EmitApi()
-            """Instance of the Emit api."""
+        if self._aedt_version > "2023.1":
+            # the next 2 lines of code are needed to point
+            # the Emit object to the correct EmiApiPython
+            # module for the current AEDT version
+            emit_core._set_api(self.aedt_version_id)
+            self._emit_api = emit_core.emit_api_python().EmitApi()
+            """Instance of the EMIT API."""
 
             self.results = Results(self)
             """''Result'' object for the selected design."""
 
             self.__emit_api_enabled = True
 
+            # set the default units here to make sure the EmitApi level
+            # stays synced with pyaedt
+            unit_types = ["Power", "Frequency", "Length", "Time", "Voltage", "Data Rate", "Resistance"]
+            unit_values = ["dBm", "MHz", "meter", "ns", "mV", "bps", "Ohm"]
+            self.set_units(unit_types, unit_values)
+
     @property
     def modeler(self):
         """Modeler.
 
         Returns
         -------
         pyaedt.modeler.schematic.ModelerEmit
@@ -242,43 +243,45 @@
             for t, v in zip(unit_type, unit_value):
                 if t not in valid_type:
                     warnings.warn("[{}] units are not supported by EMIT. The options are: {}: ".format(t, valid_type))
                     return False
                 if v not in valid_units[t]:
                     warnings.warn("[{}] are not supported by EMIT. The options are: {}: ".format(v, valid_units[t]))
                     return False
-                ut = EmitConstants.EMIT_UNIT_TYPE_STRING_TO_ENUM[t]
+                ut = EmitConstants.emit_unit_type_string_to_enum(t)
                 self._emit_api.set_units(ut, v)
                 self._units[t] = v
         else:
             if unit_type not in valid_type:
                 warnings.warn(
                     "[{}] units are not supported by EMIT. The options are: {}: ".format(unit_type, valid_type)
                 )
                 return False
             if unit_value not in valid_units[unit_type]:
                 warnings.warn(
                     "[{}] are not supported by EMIT. The options are: {}: ".format(unit_value, valid_units[unit_type])
                 )
                 return False
             # keep the backend global units synced
-            ut = EmitConstants.EMIT_UNIT_TYPE_STRING_TO_ENUM[unit_type]
+            ut = EmitConstants.emit_unit_type_string_to_enum(unit_type)
             self._emit_api.set_units(ut, unit_value)
             self._units[unit_type] = unit_value
         return True
 
     @pyaedt_function_handler()
     def get_units(self, unit_type=""):
         """Get units for the component.
 
         Parameters
         ----------
-        unit_type : str
+        unit_type : str, optional
             System of units: options are power, frequency,
-                length, time, voltage, data rate, or resistance.
+            length, time, voltage, data rate, or resistance.
+            The default is ``None`` which uses the units
+            specified globally for the project.
 
         Returns
         -------
         Str or Dict
             If unit_type is specified returns the units for that type
             and if unit_type="", returns a Dict of all units.
         """
```

### Comparing `pyaedt-0.6.71/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.72/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.72/pyaedt/emit_core/EmitConstants.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,8 @@
-import os
-import sys
-
-from pyaedt.emit_core import EMIT_MODULE
+from pyaedt import emit_core
 
 
 def result_type():
     """
     Get a result type.
 
     Returns
@@ -16,15 +13,15 @@
 
     Examples
     --------
     >>> tx_rx = EmitConstants.result_type()
 
     """
     try:
-        result = EMIT_MODULE.result_type()
+        result = emit_core.emit_api_python().result_type()
     except NameError:
         raise ValueError("An Emit object must be initialized before any static member of EmitConstants is accessed.")
     return result
 
 
 def tx_rx_mode():
     """
@@ -37,15 +34,15 @@
 
     Examples
     --------
     >>> tx_rx = EmitConstants.tx_rx_mode()
 
     """
     try:
-        tx_rx = EMIT_MODULE.tx_rx_mode()
+        tx_rx = emit_core.emit_api_python().tx_rx_mode()
     except NameError:
         raise ValueError("An Emit object must be initialized before any static member of EmitConstants is accessed.")
     return tx_rx
 
 
 def interferer_type():
     """Get an ``interferer_type`` object.
@@ -56,15 +53,15 @@
         Type of interferer: transmitters, emitters, or transmitters_and_emitters.
 
     Examples
     >>> int_type = EmitConstants.interferer_type()
     >>> tx_only = int_type.transmitters
     """
     try:
-        inter_type = EMIT_MODULE.interferer_type()
+        inter_type = emit_core.emit_api_python().interferer_type()
     except NameError:
         raise ValueError("An Emit object must be initialized before any static member of EmitConstants is accessed.")
     return inter_type
 
 
 def unit_type():
     """Get a ``unit_type`` object.
@@ -73,15 +70,15 @@
     :class:`EmitConstants.unit_type`
         Type of unit. Options are ``"Power"``, ``"Frequency"``, ``"Length"``,
         ``"Time"``, ``"Voltage"``, ``"DataRate"``, and ``"Resistance"``.
     Examples
     >>> unit_type = EmitConstants.unit_type()
     """
     try:
-        unit_type = EMIT_MODULE.unit_type()
+        unit_type = emit_core.emit_api_python().unit_type()
     except NameError:
         raise ValueError("An Emit object must be initialized before any static member of EmitConstants is accessed.")
     return unit_type
 
 
 EMIT_UNIT_TYPE = ["Power", "Frequency", "Length", "Time", "Voltage", "Data Rate", "Resistance"]
 """Valid unit type."""
@@ -93,18 +90,19 @@
     "Time": ["ps", "ns", "us", "ms", "s"],
     "Voltage": ["mV", "V"],
     "Data Rate": ["bps", "kbps", "Mbps", "Gbps"],
     "Resistance": ["uOhm", "mOhm", "Ohm", "kOhm", "megOhm", "GOhm"],
 }
 """Valid units for each unit type."""
 
-desktop_path = os.environ.get("ANSYSEM_ROOT232")
-if desktop_path and sys.version_info < (3, 8):
+
+def emit_unit_type_string_to_enum(unit_string):
     EMIT_UNIT_TYPE_STRING_TO_ENUM = {
         "Power": unit_type().power,
         "Frequency": unit_type().frequency,
         "Length": unit_type().length,
         "Time": unit_type().time,
         "Voltage": unit_type().voltage,
         "Data Rate": unit_type().dataRate,
         "Resistance": unit_type().resistance,
     }
+    return EMIT_UNIT_TYPE_STRING_TO_ENUM[unit_string]
```

### Comparing `pyaedt-0.6.71/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.72/pyaedt/emit_core/results/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import warnings
 
-from pyaedt.emit_core import EMIT_MODULE
+from pyaedt import emit_core
 from pyaedt.emit_core.results.revision import Revision
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Results:
     """
     Provides the ``Results`` object.
@@ -47,17 +47,22 @@
             be named the current design revision.
 
         Returns
         -------
         ``Revision`` object that was created.
         """
         if name == None:
-            self.design.AddResult()
-            rev_num = self.design.GetRevision()
-            name = "Revision {}".format(rev_num)
+            # check for a Current Revision that just hasn't been
+            # loaded by pyaedt
+            if self.design.GetCurrentResult() == "":
+                self.design.AddResult()
+                rev_num = self.design.GetRevision()
+                name = "Revision {}".format(rev_num)
+            else:
+                name = self.design.GetCurrentResult()
         revision = Revision(self, self.emit_project, name)
         self.revisions.append(revision)
         return revision
 
     @pyaedt_function_handler()
     def delete_revision(self, revision_name):
         """Delete the specified revision from the results.
@@ -99,15 +104,15 @@
 
         Examples
         --------
         >>> domain = Emit.results.InteractionDomain()
 
         """
         try:
-            domain = EMIT_MODULE.InteractionDomain()
+            domain = emit_core.emit_api_python().InteractionDomain()
         except NameError:
             raise ValueError("An Emit object must be initialized before any static member of the Results.")
         return domain
 
     @pyaedt_function_handler
     def _unload_revisions(self):
         """Convenience function to set all revisions
@@ -143,15 +148,15 @@
     @pyaedt_function_handler
     def get_revision(self, revision_name=None):
         """
         Load the specified revision.
 
         Parameters
         ----------
-        revision_name : str
+        revision_name : str, optional
             Revision to load. The default is  ``None`` in which
             case the latest revision will be returned.
 
         Returns
         -------
         rev:class:`pyaedt.modules.Revision`
             Specified ``Revision`` object that was loaded.
@@ -175,15 +180,23 @@
             rev = [x for x in self.revisions if revision_name == x.name]
             if len(rev) > 0:
                 # unload the current revision and load the specified revision
                 self.current_revision.revision_loaded = False
                 self.current_revision = rev[0]
                 self.current_revision._load_revision()
             else:
-                warnings.warn("{} not found.".format(revision_name))
+                # might be an old revision that was never loaded by pyaedt
+                aedt_result_list = self.design.GetResultList()
+                rev = [x for x in aedt_result_list if revision_name == x]
+                if len(rev) > 0:
+                    # unload the current revision and load the specified revision
+                    self.current_revision.revision_loaded = False
+                    self.current_revision = self._add_revision(rev[0])
+                else:
+                    warnings.warn("{} not found.".format(revision_name))
         return self.current_revision
 
     @pyaedt_function_handler()
     def analyze(self):
         """
         Analyze the current revision or create a new revision if
         the design has changed.
```

### Comparing `pyaedt-0.6.71/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.72/pyaedt/emit_core/results/revision.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,15 +56,17 @@
 
         self.path = full
         """Full path of the revision."""
 
         self.emit_project = emit_obj
         """Emit project."""
 
-        self.revision_number = design.GetRevision()
+        result_props = design.GetResultProperties(name)
+        # Strip off the Revision #
+        self.revision_number = result_props[0][9:]
         """Unique revision number from the Emit design"""
 
         result_props = design.GetResultProperties(name)
         # Strip off the 'Timestamp='
         self.timestamp = result_props[1][10:]
         """Unique timestamp for the revision"""
 
@@ -75,21 +77,15 @@
         self.revision_loaded = False
         """``True`` if the revision is loaded and ``False`` if it is not."""
         self._load_revision()
 
     @pyaedt_function_handler()
     def _load_revision(self):
         """
-        Load a specific revision.
-
-        Parameters
-        ----------
-        path : str
-            Path to an AEDT EMIT result directory.
-            For example, "Revision 1.emit"
+        Load this revision.
 
         Examples
         ----------
         >>> aedtapp.results.revision.load_revision()
         """
         if self.revision_loaded:
             return
@@ -154,20 +150,21 @@
         self._load_revision()
         engine = self.emit_project._emit_api.get_engine()
         return engine.is_domain_valid(domain)
 
     @pyaedt_function_handler()
     def get_instance_count(self, domain):
         """
-                Return the number of instances in the domain for the current revision.
+        Return the number of instances in the domain for the current revision.
+
+        Parameters
+        ----------
+        domain :
+            ``InteractionDomain`` object for constraining the analysis parameters.
 
-                Parameters
-                ----------
-                domain :
-                    ``InteractionDomain`` object for constraining the analysis parameters.
         Returns
         --------
         count : int
             Number of instances in the domain for the current revision.
 
         Examples
         ----------
@@ -210,16 +207,17 @@
     @pyaedt_function_handler()
     def get_interferer_names(self, interferer_type=None):
         """
         Get a list of all interfering transmitters/emitters in the project.
 
         Parameters
         ----------
-        interferer_type : interferer_type object
-            Type of interferer to return. Options are:
+        interferer_type : interferer_type object, optional
+            Type of interferer to return. The default is ``None``, in which
+            case both transmitters and emitters are returned. Options are:
                 - transmitters
                 - emitters
                 - transmitters_and_emitters
 
         Returns
         -------
         radios:class:`list of str`
@@ -243,69 +241,76 @@
             self.result_mode_error()
         if len(radios) == 0:
             warnings.warn("No valid radios or emitters in the project.")
             return None
         return radios
 
     @pyaedt_function_handler()
-    def get_band_names(self, radio_name, tx_rx_mode):
+    def get_band_names(self, radio_name, tx_rx_mode=None):
         """
         Get a list of all ``tx`` or ``rx`` bands (or waveforms) in
         a given radio/emitter.
 
         Parameters
         ----------
         radio_name : str
             Name of the radio/emitter.
-        tx_rx : tx_rx_mode object
-            Specifies whether to get ``tx`` or ``rx`` band names.
+        tx_rx : :class:`EmitConstants.tx_rx_mode`, optional
+            Specifies whether to get ``tx`` or ``rx`` band names. The default
+            is ``None``, in which case the names of all enabled bands are returned.
 
         Returns
         -------
         bands:class:`list of str`
             List of ``tx`` or ``rx`` band/waveform names.
 
         Examples
         ----------
         >>> bands = aedtapp.results.current_revision.get_band_names('Bluetooth', Emit.tx_rx_mode.rx)
         >>> waveforms = aedtapp.results.current_revision.get_band_names('USB_3.x', Emit.tx_rx_mode.tx)
         """
+        if tx_rx_mode is None:
+            tx_rx_mode = emitConsts.tx_rx_mode().both
         if self.revision_loaded:
             bands = self.emit_project._emit_api.get_band_names(radio_name, tx_rx_mode)
         else:
             bands = None
             self.result_mode_error()
         return bands
 
     @pyaedt_function_handler()
-    def get_active_frequencies(self, radio_name, band_name, tx_rx_mode, units=""):
+    def get_active_frequencies(self, radio_name, band_name, tx_rx_mode=None, units=""):
         """
         Get a list of active frequencies for a ``tx`` or ``rx`` band in a radio/emitter.
 
         Parameters
         ----------
         radio_name : str
             Name of the radio/emitter.
         band_name : str
            Name of the band.
-        tx_rx : tx_rx_mode object
-            Specifies whether to get ``tx`` or ``rx`` radio freqs.
-        units : str
-            Units for the frequencies.
+        tx_rx : :class:`EmitConstants.tx_rx_mode`, optional
+            Specifies whether to get ``tx`` or ``rx`` radio freqs. The default
+            is ``None``, in which case both ``tx`` and ``rx`` freqs are returned.
+        units : str, optional
+            Units for the frequencies. The default is ``None`` which uses the units
+            specified globally for the project.
 
         Returns
         -------
         freqs : List of float
             List of ``tx`` or ``rx`` radio/emitter frequencies.
 
         Examples
         ----------
         >>> freqs = aedtapp.results.current_revision.get_active_frequencies(
                 'Bluetooth', 'Rx - Base Data Rate', Emit.tx_rx_mode.rx)
         """
+        if tx_rx_mode is None:
+            tx_rx_mode = emitConsts.tx_rx_mode().both
         if self.revision_loaded:
             freqs = self.emit_project._emit_api.get_active_frequencies(radio_name, band_name, tx_rx_mode, units)
         else:
             freqs = None
             self.result_mode_error()
         return freqs
```

### Comparing `pyaedt-0.6.71/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.72/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.72/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/clr_module.py` & `pyaedt-0.6.72/pyaedt/generic/clr_module.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import warnings
 
 modules = [tup[1] for tup in pkgutil.iter_modules()]
 pyaedt_path = os.path.dirname(os.path.dirname(__file__))
 cpython = "IronPython" not in sys.version and ".NETFramework" not in sys.version
 is_linux = os.name == "posix"
 is_windows = not is_linux
+is_clr = False
 if is_linux and cpython:  # pragma: no cover
     try:
         if os.environ.get("DOTNET_ROOT") is None:
             try:
                 import dotnet
 
                 runtime = os.path.join(os.path.dirname(dotnet.__path__))
@@ -29,17 +30,26 @@
         print("DotNet Core correctly loaded.")
         if "Delcross" not in os.getenv("LD_LIBRARY_PATH", "") or "mono" not in os.getenv("LD_LIBRARY_PATH", ""):
             warnings.warn("LD_LIBRARY_PATH needs to be setup to use pyaedt.")
             warnings.warn("export ANSYSEM_ROOT222=/path/to/AnsysEM/v222/Linux64")
             msg = "export LD_LIBRARY_PATH="
             msg += "$ANSYSEM_ROOT222/common/mono/Linux64/lib64:$ANSYSEM_ROOT222/Delcross:$LD_LIBRARY_PATH"
             warnings.warn(msg)
+        is_clr = True
     except ImportError:
         msg = "pythonnet or dotnetcore not installed. Pyaedt will work only in client mode."
         warnings.warn(msg)
+else:
+    try:
+        from pythonnet import load
+
+        load("coreclr")
+        is_clr = True
+    except:
+        pass
 
 
 try:  # work around a number formatting bug in the EDB API for non-English locales
     # described in #1980
     import clr as _clr  # isort:skip
     from System.Globalization import CultureInfo as _CultureInfo
```

### Comparing `pyaedt-0.6.71/pyaedt/generic/configurations.py` & `pyaedt-0.6.72/pyaedt/generic/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1851,15 +1851,15 @@
                     ],
                     vector=[
                         decompose_variable_value(operation_dict["Props"]["Normal Position"][2 * i + 1])[0]
                         for i in range(3)
                     ],
                 )
             else:  # pragma: no cover
-                raise "Operation not supported"
+                raise ValueError("Operation not supported")
             if new_objs:
                 new_objs = list(set(new_objs) - set(old_objs))
                 for new_obj in new_objs:
                     if native_dict[new_obj]["Operations"]:
                         for dup_obj in operation_dict["Props"]["Duplicate Object"]:
                             for _, operation_dict in native_dict[dup_obj]["Operations"].items():
                                 apply_operations_to_native_components(
```

### Comparing `pyaedt-0.6.71/pyaedt/generic/constants.py` & `pyaedt-0.6.72/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/design_types.py` & `pyaedt-0.6.72/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/filesystem.py` & `pyaedt-0.6.72/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/general_methods.py` & `pyaedt-0.6.72/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,29 +95,34 @@
         if func.__name__ in el:
             _write_mes("Error in : " + el)
     _write_mes("{} - {} -  {}.".format(ex_info[1], func.__name__, message.upper()))
 
     if message_to_print:
         _write_mes(message_to_print)
     _write_mes("Arguments with values: ")
+    args_name = []
     try:
         if int(sys.version[0]) > 2:
             args_name = list(OrderedDict.fromkeys(inspect.getfullargspec(func)[0] + list(kwargs.keys())))
             args_dict = OrderedDict(list(itertools.zip_longest(args_name, args)) + list(kwargs.items()))
         else:
             args_name = list(OrderedDict.fromkeys(inspect.getargspec(func)[0] + list(kwargs.keys())))
             args_dict = OrderedDict(list(itertools.izip(args_name, args)) + list(kwargs.iteritems()))
 
         for el in args_dict:
             if el != "self":
                 _write_mes("    {} = {} ".format(el, args_dict[el]))
     except:
         pass
-
-    _write_mes("Check Online documentation on: https://aedt.docs.pyansys.com/search.html?q={}".format(func.__name__))
+    args = [func.__name__] + [i for i in args_name if i not in ["self"]]
+    _write_mes(
+        "Check Online documentation on: https://aedt.docs.pyansys.com/version/stable/search.html?q={}".format(
+            "+".join(args)
+        )
+    )
 
 
 def _check_types(arg):
     if "netref.builtins.list" in str(type(arg)):
         return "list"
     elif "netref.builtins.dict" in str(type(arg)):
         return "dict"
@@ -1800,15 +1805,16 @@
 
     @global_log_file_name.setter
     def global_log_file_name(self, value):
         self._global_log_file_name = value
 
     @property
     def enable_pandas_output(self):
-        """Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
+        """
+        Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
         If ``True`` the property or method will return a pandas object in CPython environment.
         Default is ``False``.
 
         Returns
         -------
         bool
         """
@@ -1816,15 +1822,16 @@
 
     @enable_pandas_output.setter
     def enable_pandas_output(self, val):
         self._enable_pandas_output = val
 
     @property
     def enable_debug_methods_argument_logger(self):
-        """Set/Get a flag to plot methods argument in debug logger.
+        """
+        Set/Get a flag to plot methods argument in debug logger.
         Default is ``False``.
 
         Returns
         -------
         bool
         """
         return self._enable_debug_methods_argument_logger
```

### Comparing `pyaedt-0.6.71/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.72/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.72/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/plot.py` & `pyaedt-0.6.72/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/process.py` & `pyaedt-0.6.72/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.72/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.72/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/toolkit.py` & `pyaedt-0.6.72/pyaedt/generic/toolkit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.72/pyaedt/generic/touchstone_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,23 +16,26 @@
 MAG_ANGLE = "MA"
 DB_ANGLE = "DB"
 
 keys = {REAL_IMAG: ("real", "imag"), MAG_ANGLE: ("mag", "deg"), DB_ANGLE: ("db20", "deg")}
 
 
 def _parse_ports_name(file):
-    """Parse and interpret the option line in the touchstone file
+    """Parse and interpret the option line in the touchstone file.
+
     Parameters
     ----------
     file : str
         Path of the touchstone file.
+
     Returns
     -------
     List of str
         Names of the ports in the touchstone file.
+
     """
     portnames = []
     line = file.readline()
     while not line.startswith("! Port"):
         line = file.readline()
     while line.startswith("! Port"):
         portnames.append(line.split(" = ")[1].strip())
```

### Comparing `pyaedt-0.6.71/pyaedt/hfss.py` & `pyaedt-0.6.72/pyaedt/hfss.py`

 * *Files 0% similar despite different names*

```diff
@@ -5958,15 +5958,15 @@
         deembed=False,
         terminals_rename=True,
     ):
         """Create a waveport taking the closest edges of two objects.
 
         Parameters
         ----------
-        signal : str, int, list or :class:`pyaedt.modeler.object3d.Object3d` or
+        signal : str, int, list, :class:`pyaedt.modeler.object3d.Object3d` or
          :class:`pyaedt.modeler.elements3d.FacePrimitive`
             Main object for port creation or starting object for the integration line.
         reference : int, list or :class:`pyaedt.modeler.object3d.Object3d`
             Ending object for the integration line or reference for Terminal solution. Can be multiple objects.
         create_port_sheet : bool, optional
             Whether to create a port sheet or use given start_object as port shee.
         integration_line : int or :class:`pyaedt.application.Analysis.Analysis.AxisDir`, optional
```

### Comparing `pyaedt-0.6.71/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.72/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/icepak.py` & `pyaedt-0.6.72/pyaedt/icepak.py`

 * *Files 2% similar despite different names*

```diff
@@ -2794,102 +2794,14 @@
                     sm.surface_diffuse_absorptance = oo.GetPropEvaluatedValue("Solar Diffuse Absorptance")
                 if "Solar Normal Absorptance" in props:
                     sm.surface_incident_absorptance = oo.GetPropEvaluatedValue("Solar Normal Absorptance")
                 self.materials.surface_material_keys[mat.lower()] = sm
         return True
 
     @pyaedt_function_handler()
-    def create_two_resistor_network_block_depr(self, object_name, power, rjb, rjc, placement):
-        """Create a two-resistor network block.
-
-        .. deprecated:: 0.6.30
-            This method is replaced by the ``create_two_resistor_network_block`` method.
-
-        Parameters
-        ----------
-        object_name : str
-            Name of the object (3D block primitive) on which to create the two-resistor
-            network.
-        power : float
-            Junction power in [W].
-        rjb : float
-            Junction-to-board thermal resistance in [K/W].
-        rjc : float
-            Junction-to-case thermal resistance in [K/W].
-        placement : str
-            Placement of the network block. Options are:
-            - ``top``: Network block is placed on top of the board.
-            - "bottom" : Network block is placed on bottom of the board.
-
-        Returns
-        -------
-        :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Boundary object.
-
-        References
-        ----------
-
-        >>> oModule.AssignNetworkBoundary
-
-        Examples
-        --------
-
-        >>> box = icepak.modeler.create_box([4, 5, 6], [5, 5, 5], "NetworkBox1", "copper")
-        >>> block = icepak.create_two_resistor_network_block("NetworkBox1", "2W", 20, 10, "top")
-        >>> block.props["Nodes"]["Internal"][0]
-        '2W'
-        """
-        warnings.warn(
-            "This method is deprecated in 0.6.29. Use the ``create_two_resistor_network_block`` method instead.",
-            DeprecationWarning,
-        )
-        object_handle = self.modeler.get_object_from_name(object_name)
-        placement = placement.lower()
-        if placement == "top":
-            board_face_id = object_handle.top_face_z.id
-            case_face_id = object_handle.bottom_face_z.id
-            board_side = "bottom"
-            case_side = "top"
-        else:
-            board_face_id = object_handle.bottom_face_z.id
-            case_face_id = object_handle.top_face_z.id
-            board_side = "top"
-            case_side = "bottom"
-
-        # Define network properties in props directory
-        props = {
-            "Faces": [board_face_id, case_face_id],
-            "Nodes": OrderedDict(
-                {
-                    "Case_side(" + case_side + ")": [case_face_id, "NoResistance"],
-                    "Board_side(" + board_side + ")": [board_face_id, "NoResistance"],
-                    "Internal": [power],
-                }
-            ),
-            "Links": OrderedDict(
-                {
-                    "Rjc": ["Case_side(" + case_side + ")", "Internal", "R", str(rjc) + "cel_per_w"],
-                    "Rjb": ["Board_side(" + board_side + ")", "Internal", "R", str(rjb) + "cel_per_w"],
-                }
-            ),
-            "SchematicData": ({}),
-        }
-
-        # Default material is Ceramic_material
-        self.modeler[object_name].material_name = "Ceramic_material"
-
-        # Create boundary condition and set solve_inside = False
-        bound = BoundaryObject(self, object_name, props, "Network")
-        if bound.create():
-            self.boundaries.append(bound)
-            self.modeler.primitives[object_name].solve_inside = False
-            return bound
-        return None
-
-    @pyaedt_function_handler()
     def import_idf(
         self,
         board_path,
         library_path=None,
         control_path=None,
         filter_cap=False,
         filter_ind=False,
@@ -3797,14 +3709,25 @@
             Boundary object when successful or ``None`` when failed.
 
         References
         ----------
 
         >>> oModule.AssignSourceBoundary
 
+        Examples
+        --------
+
+        >>> from pyaedt import Icepak
+        >>> app = Icepak()
+        >>> box = app.modeler.create_box([0, 0, 0], [20, 20, 20], name="box")
+        >>> ds = app.create_dataset1d_design("Test_DataSet", [1, 2, 3], [3, 4, 5])
+        >>> app.solution_type = "Transient"
+        >>> b = app.assign_source("box", "Total Power", assignment_value={"Type": "Temp Dep",
+        ... "Function": "Piecewise Linear", "Values": "Test_DataSet"})
+
         """
         default_values = {"Total Power": "0W", "Surface Heat": "0irrad_W_per_m2", "Temperature": "AmbientTemp"}
         if not boundary_name:
             boundary_name = generate_unique_name("Source")
         props = {}
         if isinstance(assignment, int):
             props["Faces"] = [assignment]
```

### Comparing `pyaedt-0.6.71/pyaedt/maxwell.py` & `pyaedt-0.6.72/pyaedt/maxwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,17 @@
     @pyaedt_function_handler()
     def setup_ctrlprog(
         self, setupname, file_str=None, keep_modifications=False, python_interpreter=None, aedt_lib_dir=None
     ):
         """Configure the transient design setup to run a specific control program.
         The control program is executed from a temporary directory that Maxwell creates for every setup run.
 
+        .. deprecated:: 0.6.71
+        Use :func:`enable_control_program` method instead.
+
         Parameters
         ----------
         setupname : str
             Name of the setup.
             It will become the name of the Python file.
         file_str : str, optional
             Name of the file. The default value is ``None``.
@@ -2649,14 +2652,15 @@
 
     @property
     def model_depth(self):
         """Model depth."""
 
         if "ModelDepth" in self.design_properties:
             value_str = self.design_properties["ModelDepth"]
+            a = None
             try:
                 a = float_units(value_str)
             except:
                 a = self.variable_manager[value_str].value
             finally:
                 return a
         else:
```

### Comparing `pyaedt-0.6.71/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.72/pyaedt/maxwellcircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 from pyaedt.application.AnalysisMaxwellCircuit import AnalysisMaxwellCircuit
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class MaxwellCircuit(AnalysisMaxwellCircuit, object):
-    """Provides the Maxwell Circuit application interface.
+    """Provide the Maxwell Circuit application interface.
 
     Parameters
     ----------
     projectname : str, optional
         Name of the project to select or the full path to the project
-        or AEDTZ archive to open.  The default is ``None``, in which
+        or AEDTZ archive to open. The default is ``None``, in which
         case an attempt is made to get an active project. If no
         projects are present, an empty project is created.
     designname : str, optional
         Name of the design to select. The default is ``None``, in
         which case an attempt is made to get an active design. If no
         designs are present, an empty design is created.
     specified_version : str, optional
@@ -30,15 +30,15 @@
     non-graphical : bool, optional
         Whether to launch AEDT in non-graphical mode. The default
         is ``False``, in which case AEDT is launched in graphical mode.
         This parameter is ignored when a script is launched within AEDT.
     new_desktop_session : bool, optional
         Whether to launch an instance of AEDT in a new thread, even if
         another instance of the ``specified_version`` is active on the
-        machine.  The default is ``True``.
+        machine. The default is ``True``.
     close_on_exit : bool, optional
         Whether to release AEDT on exit. The default is ``False``.
     student_version : bool, optional
         Whether to open the AEDT student version. The default is ``False``.
     machine : str, optional
         Machine name to connect the oDesktop session to. This works only in 2022 R2
         and later. The remote server must be up and running with the command
@@ -175,16 +175,15 @@
                     if ypos > 0.254:
                         xpos += delta
                         ypos = 0
         return True
 
     @pyaedt_function_handler
     def export_netlist_from_schematic(self, file_to_export):
-        """
-        Create netlist from schematic circuit.
+        """Create netlist from schematic circuit.
 
         Parameters
         ----------
         file_to_export : str
             File path to export the netlist to.
 
         Returns
```

### Comparing `pyaedt-0.6.71/pyaedt/mechanical.py` & `pyaedt-0.6.72/pyaedt/mechanical.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,18 +132,18 @@
     @pyaedt_function_handler()
     def assign_em_losses(
         self,
         designname="HFSSDesign1",
         setupname="Setup1",
         sweepname="LastAdaptive",
         map_frequency=None,
-        surface_objects=[],
+        surface_objects=None,
         source_project_name=None,
-        paramlist=[],
-        object_list=[],
+        paramlist=None,
+        object_list=None,
     ):
         """Map EM losses to a Mechanical design.
 
         Parameters
         ----------
         designname : str, optional
             Name of the design of the source mapping. The default is ``"HFSSDesign1"``.
@@ -151,32 +151,39 @@
             Name of the EM setup. The default is ``"Setup1"``.
         sweepname : str, optional
             Name of the EM sweep to use for the mapping. The default is ``"LastAdaptive"``.
         map_frequency : str, optional
             Frequency to map. The default is ``None``. The value must be ``None`` for
             Eigenmode analysis.
         surface_objects : list, optional
-            List objects in the source that are metals. The default is ``[]``.
+            List objects in the source that are metals. The default is ``None``.
         source_project_name : str, optional
             Name of the source project. The default is ``None``, in which case
             the source from the same project is used.
         paramlist : list, optional
-            List of all parameters in the EM to map. The default is ``[]``.
+            List of all parameters in the EM to map. The default is ``None``.
         object_list : list, optional
-             The default is ``[]``.
+             The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
 
         References
         ----------
 
         >>> oModule.AssignEMLoss
         """
+        if surface_objects is None:
+            surface_objects = []
+        if paramlist is None:
+            paramlist = []
+        if object_list is None:
+            object_list = []
+
         assert "Thermal" in self.solution_type, "This method works only in a Mechanical Thermal analysis."
 
         self.logger.info("Mapping HFSS EM Lossess")
         oName = self.project_name
         if oName == source_project_name or source_project_name is None:
             projname = "This Project*"
         else:
@@ -231,15 +238,15 @@
     def assign_thermal_map(
         self,
         object_list,
         designname="IcepakDesign1",
         setupname="Setup1",
         sweepname="SteadyState",
         source_project_name=None,
-        paramlist=[],
+        paramlist=None,
     ):
         """Map thermal losses to a Mechanical design.
 
         .. note::
            This method works in 2021 R2 only when coupled with Icepak.
 
         Parameters
@@ -252,26 +259,28 @@
             Name of the EM setup. The default is ``"Setup1"``.
         sweepname : str, optional
             Name of the EM sweep to use for the mapping. The default is ``"SteadyState"``.
         source_project_name : str, optional
             Name of the source project. The default is ``None``, in which case the
             source from the same project is used.
         paramlist : list, optional
-            List of all parameters in the EM to map. The default is ``[]``.
+            List of all parameters in the EM to map. The default is ``None``.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
 
         References
         ----------
 
         >>> oModule.AssignThermalCondition
         """
+        if paramlist is None:
+            paramlist = []
 
         assert self.solution_type == "Structural", "This method works only in a Mechanical Structural analysis."
 
         self.logger.info("Mapping HFSS EM Lossess")
         oName = self.project_name
         if oName == source_project_name or source_project_name is None:
             projname = "This Project*"
```

### Comparing `pyaedt-0.6.71/pyaedt/misc/Console.py_build` & `pyaedt-0.6.72/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.72/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.72/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.72/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.72/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.72/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import argparse
 import os
 import shutil
 import sys
 import warnings
 from xml.dom.minidom import parseString
 import xml.etree.ElementTree as ET
 from xml.etree.ElementTree import ParseError
@@ -16,24 +17,69 @@
 sys.path.append(os.path.normpath(os.path.join(pyaedt_path, "..")))
 
 is_linux = os.name == "posix"
 is_windows = not is_linux
 pid = 0
 
 
-def add_pyaedt_to_aedt(aedt_version, is_student_version=False, use_sys_lib=False):
+def main():
+    args = parse_arguments()
+    add_pyaedt_to_aedt(
+        args.version, is_student_version=args.student, use_sys_lib=args.sys_lib, new_desktop_session=args.new_session
+    )
+
+
+def parse_arguments():
+    parser = argparse.ArgumentParser(description="Install PyAEDT and setup PyAEDT toolkits in AEDT.")
+    parser.add_argument(
+        "--version", "-v", default="231", metavar="XY.Z", help="AEDT three-digit version (e.g. 231). Default=231"
+    )
+    parser.add_argument(
+        "--student", "--student_version", action="store_true", help="Install toolkits for AEDT Student Version."
+    )
+    parser.add_argument("--sys_lib", "--syslib", action="store_true", help="Install toolkits in SysLib.")
+    parser.add_argument(
+        "--new_session", action="store_true", help="Start a new session of AEDT after installing PyAEDT."
+    )
+
+    args = parser.parse_args()
+    args = process_arguments(args, parser)
+    return args
+
+
+def process_arguments(args, parser):
+    if len(args.version) != 3:
+        parser.print_help()
+        parser.error("Version should be a three digit number (e.g. 231)")
+
+    args.version = "20" + args.version[-3:-1] + "." + args.version[-1:]
+    return args
+
+
+def add_pyaedt_to_aedt(aedt_version, is_student_version=False, use_sys_lib=False, new_desktop_session=False):
     from pyaedt import Desktop
+    from pyaedt.generic.general_methods import grpc_active_sessions
 
-    with Desktop(aedt_version, True, new_desktop_session=True, student_version=is_student_version) as d:
+    sessions = grpc_active_sessions(aedt_version, is_student_version)
+    if not sessions:
+        if not new_desktop_session:
+            print("Launching a new AEDT desktop session.")
+        new_desktop_session = True
+    with Desktop(
+        specified_version=aedt_version,
+        non_graphical=new_desktop_session,
+        new_desktop_session=new_desktop_session,
+        student_version=is_student_version,
+    ) as d:
         desktop = sys.modules["__main__"].oDesktop
         pers1 = os.path.join(desktop.GetPersonalLibDirectory(), "pyaedt")
         pid = desktop.GetProcessID()
         # Linking pyaedt in PersonalLib for IronPython compatibility.
         if os.path.exists(pers1):
-            d.logger.info("PersonalLib already mapped")
+            d.logger.info("PersonalLib already mapped.")
         else:
             if is_windows:
                 os.system('mklink /D "{}" "{}"'.format(pers1, pyaedt_path))
             else:
                 os.system('ln -s "{}" "{}"'.format(pyaedt_path, pers1))
 
         toolkits = ["Project"]
@@ -54,25 +100,25 @@
             ]
 
         for product in toolkits:
             if use_sys_lib:
                 try:
                     sys_dir = os.path.join(d.syslib, "Toolkits")
                     install_toolkit(sys_dir, product, aedt_version)
-                    d.logger.info("Installed toolkit for {} in sys lib".format(product))
+                    d.logger.info("Installed toolkit for {} in sys lib.".format(product))
 
                 except IOError:
                     pers_dir = os.path.join(d.personallib, "Toolkits")
                     install_toolkit(pers_dir, product, aedt_version)
-                    d.logger.info("Installed toolkit for {} in personal lib".format(product))
+                    d.logger.info("Installed toolkit for {} in personal lib.".format(product))
             else:
                 pers_dir = os.path.join(d.personallib, "Toolkits")
                 install_toolkit(pers_dir, product, aedt_version)
-                d.logger.info("Installed toolkit for {} in personal lib".format(product))
-    if pid:
+                d.logger.info("Installed toolkit for {} in personal lib.".format(product))
+    if pid and new_desktop_session:
         try:
             os.kill(pid, 9)
         except:
             pass
 
 
 def install_toolkit(toolkit_dir, product, aedt_version):
@@ -183,21 +229,8 @@
 def exe():
     if is_windows:
         return ".exe"
     return ""
 
 
 if __name__ == "__main__":
-    student_version = False
-    if len(sys.argv) < 2:
-        version = "2022.2"
-    elif sys.argv[1].endswith("sv"):
-        v = sys.argv[1][:-2]
-        version = "20" + v[-3:-1] + "." + v[-1:]
-        student_version = True
-    else:
-        v = sys.argv[1]
-        version = "20" + v[-3:-1] + "." + v[-1:]
-    sys_lib = True
-    if len(sys.argv) == 3:
-        sys_lib = True if sys.argv[2] == "1" else False
-    add_pyaedt_to_aedt(version, student_version, sys_lib)
+    main()
```

### Comparing `pyaedt-0.6.71/pyaedt/misc/amat.xml` & `pyaedt-0.6.72/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/console_setup.py` & `pyaedt-0.6.72/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.72/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.72/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.72/pyaedt/misc/install_extra_toolkits.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,21 @@
     "ChokeWizard": {
         "pip": "git+https://github.com/pyansys/pyaedt-choke-toolkit.git",
         "image": "pyansys.png",
         "toolkit_script": "ansys/aedt/toolkits/choke/choke_toolkit.py",
         "installation_path": "Project",
         "package_name": "ansys.aedt.toolkits.choke",
     },
+    "TemplateToolkit": {
+        "pip": "git+https://github.com/pyansys/pyaedt-toolkit-template.git",
+        "image": "pyansys.png",
+        "toolkit_script": "ansys/aedt/toolkits/template/template_toolkit.py",
+        "installation_path": "Project",
+        "package_name": "ansys.aedt.toolkits.template",
+    },
 }
 
 
 def write_toolkit_config(product_toolkit_dir, pyaedt_lib_dir, toolkitname, toolkit, force_write=False):
     """Write a toolkit configuration file and, if needed a button in Automation menu."""
     tab_config_file_path = os.path.join(product_toolkit_dir, "TabConfig.xml")
     if not os.path.isfile(tab_config_file_path) or force_write:
```

### Comparing `pyaedt-0.6.71/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.72/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/misc.py` & `pyaedt-0.6.72/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.72/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.72/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.72/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.72/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.72/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.72/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/misc/template.acf` & `pyaedt-0.6.72/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.72/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.72/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.72/pyaedt/modeler/advanced_cad/oms.py`

 * *Files 1% similar despite different names*

```diff
@@ -434,15 +434,15 @@
         utm_y_min = utm_center[1] - max_radius
         utm_y_max = utm_center[1] + max_radius
 
         sample_grid_size = grid_size  # meters
         num_samples = int(np.ceil(max_radius * 2 / sample_grid_size))
         x_samples = np.linspace(utm_x_min, utm_x_max, int(num_samples))
         y_samples = np.linspace(utm_y_min, utm_y_max, int(num_samples))
-        elevation_data = srtm.get_data(local_cache_dir="tmp_cache")
+        elevation_data = srtm.get_data()
 
         all_data = np.zeros((num_samples, num_samples))
         all_utm = np.zeros((num_samples, num_samples, 2))
         all_lat_lon = np.zeros((num_samples, num_samples, 2))
         logger.info("Terrain Points...")
         last_displayed = -1
         for n, x in enumerate(x_samples):
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.72/pyaedt/modeler/advanced_cad/parts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.72/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/Modeler.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/Primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,15 +529,15 @@
 
     @pyaedt_function_handler()
     def value_in_object_units(self, value):
         """Convert one or more strings for numerical lengths to floating point values.
 
         Parameters
         ----------
-        value : string or list of strings
+        value : str or list of str
             One or more strings for numerical lengths. For example, ``"10mm"``
             or ``["10mm", "12mm", "14mm"]``. When a list is given, the entire
             list is converted.
 
         Returns
         -------
         List of floats
@@ -558,15 +558,15 @@
             elif isinstance(element, str):
                 # element is an existing variable
                 si_value = self._app.evaluate_expression(element)
                 v = Variable("{}meter".format(si_value))
                 v.rescale_to(self.model_units)
                 num_val = v.numeric_value
             else:
-                raise ("Inputs to value_in_object_units must be strings or numbers.")
+                raise TypeError("Inputs to value_in_object_units must be strings or numbers.")
 
             numeric_list.append(num_val)
 
         if scalar:
             return numeric_list[0]
         else:
             return numeric_list
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/Primitives2D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -989,14 +989,18 @@
                 vArgParamVector.append(
                     ["NAME:UDMParam", "Name:=", name_param, "Value:=", str(val), "PropType2:=", 3, "PropFlag2:=", 2]
                 )
             elif str(val)[0] in "0123456789":
                 vArgParamVector.append(
                     ["NAME:UDMParam", "Name:=", name_param, "Value:=", str(val), "PropType2:=", 3, "PropFlag2:=", 4]
                 )
+            elif val in self._app.variable_manager.variables:
+                vArgParamVector.append(
+                    ["NAME:UDMParam", "Name:=", name_param, "Value:=", str(val), "PropType2:=", 3, "PropFlag2:=", 2]
+                )
             else:
                 vArgParamVector.append(
                     [
                         "NAME:UDMParam",
                         "Name:=",
                         name_param,
                         "Value:=",
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/components_3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/elements3d.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/object3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -1555,15 +1555,15 @@
         nclones : int, optional
             Number of clones. The default is ``2``.
         attachObject : bool, optional
             Whether to attach the object. The default is ``False``.
 
         Returns
         -------
-        list of :class:`pyaedt.modeler.cad.object3d.Object3d`
+        list of str
             List of names of the newly added objects.
 
         References
         ----------
 
         >>> oEditor.DuplicateAlongLine
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.72/pyaedt/modeler/cad/polylines.py`

 * *Files 0% similar despite different names*

```diff
@@ -530,16 +530,16 @@
                         if position_list[0] != position_list[-1]:
                             position_list.append(position_list[0])
                             current_segment = PolylineSegment("Line")
                     else:
                         break
                 else:
                     current_segment = segment_types[vertex_count]
-            except IndexError:
-                raise ("Number of segments inconsistent with the number of points!")
+            except Exception as e:
+                raise IndexError("Number of segments inconsistent with the number of points!")
 
             if current_segment:
                 seg_str = self._segment_array(
                     current_segment, start_index=index_count, start_point=position_list[pos_count]
                 )
                 segment_str.append(seg_str)
 
@@ -575,15 +575,15 @@
     def _evaluate_arc_angle_extra_points(self, segment, start_point):
         """Evaluates the extra points for the ArcAngle segment type.
         It also auto evaluates the arc_plane if it was not specified by the user.
         segment.extra_points[0] contains the arc mid point (on the arc).
         segment.extra_points[1] contains the arc end point.
         Both are function of the arc center, arc angle and arc plane.
         """
-        # from start-point and angle, calculate the mid- and end-points
+        # from start-point and angle, calculate the mid-point and end-points
         # Also identify the plane of the arc ("YZ", "ZX", "XY")
         plane_axes = {"YZ": [1, 2], "ZX": [2, 0], "XY": [0, 1]}
         c_xyz = self._primitives.value_in_object_units(segment.arc_center)
         p0_xyz = self._primitives.value_in_object_units(start_point)
 
         if segment.arc_plane:
             # Accept the user input for the plane of rotation - let the modeler fail if invalid
@@ -593,15 +593,15 @@
             if c_xyz[0] == p0_xyz[0]:
                 plane_def = ("YZ", plane_axes["YZ"])
             elif c_xyz[1] == p0_xyz[1]:
                 plane_def = ("ZX", plane_axes["ZX"])
             elif c_xyz[2] == p0_xyz[2]:
                 plane_def = ("XY", plane_axes["XY"])
             else:
-                raise ("Start point and arc-center do not lie on a common base plane.")
+                raise Exception("Start point and arc-center do not lie on a common base plane.")
             segment.arc_plane = plane_def[0]
 
         # Calculate the extra two points of the angular arc in the alpha-beta plane
         alph_index = plane_def[1][0]
         beta_index = plane_def[1][1]
         c_alph = c_xyz[alph_index]
         c_beta = c_xyz[beta_index]
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/calculators.py` & `pyaedt-0.6.72/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
         """Aedt oDefinitionManager.
 
         References
         ----------
 
         >>> oDefinitionManager = oProject.GetDefinitionManager()
         """
-
         return self._app.oproject.GetDefinitionManager()
 
     @property
     def o_component_manager(self):
         """Component manager object."""
         return self._app.o_component_manager
 
@@ -102,16 +101,19 @@
     @property
     def model_units(self):
         """Model units."""
         return self._modeler.model_units
 
     @property
     def schematic_units(self):
-        """Schematic units. Options are ``"mm"``, ``"mil"``, ``"cm"`` and all other metric and imperial units.
-        The default is ``"meter"``."""
+        """Schematic units.
+
+        Options are ``"mm"``, ``"mil"``, ``"cm"`` and all other metric and imperial units.
+        The default is ``"meter"``.
+        """
         return self._modeler.schematic_units
 
     @schematic_units.setter
     def schematic_units(self, value):
         self._modeler.schematic_units = value
 
     @property
@@ -128,16 +130,17 @@
             v = net.split(";")
             if v[0].replace("Wire@", "") not in nets:
                 nets.append(v[0].replace("Wire@", ""))
         return nets
 
     @pyaedt_function_handler()
     def _convert_point_to_meter(self, point):
-        """Convert numbers automatically to mils, rounding to the nearest 100 mil
-        which is minimum schematic snap unit."""
+        """Convert numbers automatically to mils.
+        It is rounded to the nearest 100 mil which is minimum schematic snap unit.
+        """
         xpos = point[0]
         ypos = point[1]
 
         if isinstance(point[0], (float, int)):
             xpos = (
                 round(point[0] * AEDT_UNITS["Length"][self.schematic_units] / AEDT_UNITS["Length"]["mil"], -2)
                 * AEDT_UNITS["Length"]["mil"]
@@ -321,15 +324,14 @@
         Returns
         -------
         :class:`pyaedt.modeler.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
-
         >>> oEditor.CreateGround
         """
         xpos, ypos = self._get_location(location)
         id = self.create_unique_id()
 
         name = self.oeditor.CreateGround(
             ["NAME:GroundProps", "Id:=", id],
@@ -362,23 +364,26 @@
         ----------
 
         >>> oModelManager.Add
         >>> oComponentManager.Add
         """
 
         def _parse_ports_name(file):
-            """Parse and interpret the option line in the touchstone file
+            """Parse and interpret the option line in the touchstone file.
+
             Parameters
             ----------
             file : str
                 Path of the Touchstone file.
+
             Returns
             -------
             List of str
                 Names of the ports in the touchstone file.
+
             """
             portnames = []
             line = file.readline()
             while not line.startswith("! Port"):
                 line = file.readline()
             while line.startswith("! Port"):
                 portnames.append(line.split(" = ")[1].strip())
@@ -735,35 +740,38 @@
                     nexxim[nexxim.index(el) + 1] = nexxim_data
         self.o_component_manager.Edit(
             name, ["Name:" + component_name, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]]
         )
         return True
 
     @pyaedt_function_handler()
-    def enable_global_netlist(self, component_name, global_netlist_list=[]):
+    def enable_global_netlist(self, component_name, global_netlist_list=None):
         """Enable Nexxim global net list.
 
         Parameters
         ----------
         component_name : str
             Name of the component.
         global_netlist_list : list
-            A list of lines to include. The default is ``[]``.
+            A list of lines to include. The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oComponentManager.GetData
         >>> oComponentManager.Edit
         """
+        if global_netlist_list is None:
+            global_netlist_list = []
+
         name = component_name
 
         properties = self.o_component_manager.GetData(name)
         if len(properties) > 0:
             nexxim = list(properties[len(properties) - 1][1])
             for el in nexxim:
                 if el == "GRef:=":
@@ -795,15 +803,14 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oSymbolManager.Add
         """
-
         numpins = len(pin_lists)
         h = int(numpins / 2)
         x1 = 0
         y2 = 0
         x2 = 0.00508
         y1 = 0.00254 * (h + 3)
         xp = -0.00254
@@ -911,15 +918,16 @@
     @pyaedt_function_handler()
     def refresh_all_ids(self):
         """Refresh all IDs and return the number of components.
 
         References
         ----------
 
-        >>> oEditor.GetAllElements()"""
+        >>> oEditor.GetAllElements()
+        """
         obj = self.oeditor.GetAllElements()
         if not obj:
             obj = []
         obj = [i for i in obj if "Wire" not in i[:4]]
         for el in obj:
             if not self.get_obj_id(el):
                 name = el.split(";")
@@ -939,15 +947,15 @@
     @pyaedt_function_handler()
     def add_id_to_component(self, id):
         """Add an ID to a component.
 
         Parameters
         ----------
         id : int
-            ID to assign the component.
+            ID to assign to the component.
 
         Returns
         -------
         int
             Number of components.
 
         """
@@ -977,14 +985,15 @@
         objname : str
             Name of the object.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
+
         """
         for el in self.components:
             if self.components[el].name == objname:
                 return el
         return None
 
     @pyaedt_function_handler()
@@ -1032,14 +1041,15 @@
         List
             List of axis values ``[x, y]``.
 
         References
         ----------
 
         >>> oEditor.GetComponentPinLocation
+
         """
         if isinstance(partid, str):
             x = _retry_ntimes(30, self.oeditor.GetComponentPinLocation, partid, pinname, True)
             y = _retry_ntimes(30, self.oeditor.GetComponentPinLocation, partid, pinname, False)
         else:
             x = _retry_ntimes(
                 30, self.oeditor.GetComponentPinLocation, self.components[partid].composed_name, pinname, True
@@ -1055,23 +1065,22 @@
 
         .. deprecated:: 0.6.56
            Use :func:`number_with_units` instead.
 
         Parameters
         ----------
         Value : str
-
+            Value of the quantity.
         sUnits :
             The default is ``None``.
 
         Returns
         -------
         type
 
-
         """
         warnings.warn("Use :func:`number_with_units` instead.", DeprecationWarning)
         return self._app.number_with_units(Value, sUnits)
 
     @pyaedt_function_handler()
     def number_with_units(self, value, units=None):
         """Convert a number to a string with units. If value is a string, it's returned as is.
@@ -1083,40 +1092,43 @@
         units : optional
             Units for formatting. The default is ``None``, which uses ``"meter"``.
 
         Returns
         -------
         str
            String concatenating the value and unit.
+
         """
         return self._app.number_with_units(value, units)
 
     @pyaedt_function_handler()
     def create_line(self, points_array, color=0, line_width=0):
         """Draw a graphical line.
 
         Parameters
         ----------
         points_array : list
             A nested list of point coordinates. For example,
             ``[[x1, y1], [x2, y2], ...]``.
         color : string or 3 item list, optional
-            Color or the line. The default is ``0``.
+            Color or the line. The default is ``"0"``.
         line_width : float, optional
             Width of the line. The default is ``0``.
+
         Returns
         -------
+        :class:`pyaedt.modeler.object3dcircuit.Line`
+            Line Object.
 
         >>> oEditor.CreateLine
         """
-
-        pointlist = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
+        points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
         id = self.create_unique_id()
         return self.oeditor.CreateLine(
-            ["NAME:LineData", "Points:=", pointlist, "LineWidth:=", line_width, "Color:=", color, "Id:=", id],
+            ["NAME:LineData", "Points:=", points, "LineWidth:=", line_width, "Color:=", color, "Id:=", id],
             ["NAME:Attributes", "Page:=", 1],
         )
 
     @pyaedt_function_handler()
     def create_wire(self, points_array, wire_name=""):
         """Create a wire.
 
@@ -1134,17 +1146,17 @@
             Wire Object.
 
         References
         ----------
 
         >>> oEditor.CreateWire
         """
-        pointlist = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
+        points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
         wire_id = self.create_unique_id()
-        arg1 = ["NAME:WireData", "Name:=", wire_name, "Id:=", wire_id, "Points:=", pointlist]
+        arg1 = ["NAME:WireData", "Name:=", wire_name, "Id:=", wire_id, "Points:=", points]
         arg2 = ["NAME:Attributes", "Page:=", 1]
         try:
             wire_id = _retry_ntimes(10, self.oeditor.CreateWire, arg1, arg2)
             w = Wire(self._modeler)
             for segment in self._app.oeditor.GetWireSegments(wire_id):
                 key = "SegmentID_{}".format(segment.split(" ")[3])
                 point1 = [float(x) for x in segment.split(" ")[1].split(",")]
@@ -1281,15 +1293,17 @@
 
         Parameters
         ----------
         filter_str : str
             Filter String to search.
 
         Returns
+        -------
         list
             List of matching component names.
+
         """
         c = []
         for el in list(self.components.keys()):
             if filter_string(el, filter_str):
                 c.append(el)
         return c
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
         object_name : str
             Name of the object.
 
         Returns
         -------
         EmitComponent
             The component when successful, None when failed.
+
         """
         for el in self.components:
             if self.components[el].name == object_name:
                 return el
         return None
 
     @pyaedt_function_handler()
@@ -261,15 +262,14 @@
         o :
             Object (component) to update.
 
         Returns
         -------
         type
             Object with properties.
-
         """
         o.update_property_tree()
         comp_type = o.root_prop_node.props["Type"]
         o._add_property("Type", comp_type)
         return o
 
 
@@ -346,18 +346,14 @@
 
         Parameters
         ----------
         component : EmitComponent or str
             The component or name of component to move this component to
             and connect. For example, "Radio1"
 
-        Returns
-        -------
-        None
-
         """
         if isinstance(component, EmitComponent):
             self.oeditor.PlaceComponent(self.name, component.name)
         else:
             self.oeditor.PlaceComponent(self.name, component)
 
     @pyaedt_function_handler()
@@ -644,15 +640,15 @@
         return orientation
 
     def get_position(self, units=""):
         """Get the position of this antenna.
 
         Parameters
         ----------
-        units : str
+        units : str, optional
             Units of the antenna position. If None specified, units are meters.
 
         Returns
         -------
         Tuple containing the X, Y, and Z offset values in specified units.
 
         """
@@ -708,26 +704,26 @@
         Parameters
         ----------
         None
 
         Returns
         -------
         List
-            List of the bands in the radio."""
+            List of the band nodes in the radio."""
         band_nodes = self.get_prop_nodes({"Type": "Band"})
         return band_nodes
 
     def band_start_frequency(self, band_node, units=""):
         """Get the start frequency of the band node.
 
         Parameters
         ----------
         band_node : Instance of the band node.
-        units : str
-            Units of the start frequency.
+        units : str, optional
+            If ``None`` specified, global units are used.
 
         Returns
         -------
         Float
             Start frequency of the band node."""
         if not units or units not in emit_consts.EMIT_VALID_UNITS["Frequency"]:
             units = self.units["Frequency"]
@@ -872,16 +868,16 @@
     def set_band_power_level(self, power, units=""):
         """Set the power of the fundamental for the given band.
 
         Parameters
         ----------
         power : float
             Peak amplitude of the fundamental [dBm].
-        units : str
-            Units of the input power.
+        units : str, optional
+            Units of the input power. If None specified, global units are used.
 
         Return
         ------
         None
         """
         if "Band" not in self.props["Type"]:
             raise TypeError("{} must be a band.".format(self.node_name))
@@ -897,16 +893,16 @@
 
     @pyaedt_function_handler()
     def get_band_power_level(self, units=""):
         """Get the power of the fundamental for the given band.
 
         Parameters
         ----------
-        units : str
-            Units to use for the power.
+        units : str, optional
+            Units to use for the power. If None specified, global units are used.
 
         Return
         ------
         Float
             Peak amplitude of the fundamental [units].
         """
         if "Band" not in self.props["Type"]:
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.72/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.72/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.72/pyaedt/modeler/modeler2d.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,27 +143,26 @@
 
     @pyaedt_function_handler()
     def objects_in_bounding_box(self, bounding_box, check_lines=True, check_sheets=True):
         """Given a 2D bounding box, check if sheets and lines are inside it.
 
         Parameters
         ----------
-        bounding_box : list.
+        bounding_box : list
             List of either the 4 or 6 coordinates of the bounding box vertices.
             Bounding box is provided as [xmin, ymin, zmin, xmax, ymax, zmax].
-        check_lines : bool, optional.
+        check_lines : bool, optional
             Whether to check line objects. The default is ``True``.
-        check_sheets : bool, optional.
+        check_sheets : bool, optional
             Whether to check sheet objects. The default is ``True``.
 
         Returns
         -------
         list of :class:`pyaedt.modeler.object3d`
         """
-
         if len(bounding_box) != 4 and len(bounding_box) != 6:
             raise ValueError("Bounding box must be a list of 4 or 6 elements.")
 
         if len(bounding_box) == 4:
             if self._app.design_type == "2D Extractor" or self._app.xy_plane:
                 bounding_box = [bounding_box[0], bounding_box[1], 0, bounding_box[2], bounding_box[3], 0]
             else:
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.72/pyaedt/modeler/modeler3d.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Primitives3D import Primitives3D
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Modeler3D(GeometryModeler, Primitives3D, object):
+
     """Provides the Modeler 3D application interface.
 
     This class is inherited in the caller application and is accessible through the modeler variable
     object. For example, ``hfss.modeler``.
 
     Parameters
     ----------
@@ -581,18 +582,16 @@
 
         References
         ----------
 
         >>> oEditor.CreateCylinder
         >>> oEditor.AssignMaterial
 
-
         Examples
         --------
-
         This example shows how to create a Coaxial Along X Axis waveguide.
 
         >>> from pyaedt import Hfss
         >>> app = Hfss()
         >>> position = [0,0,0]
         >>> coax = app.modeler.create_coaxial(
         ...    position, app.AXIS.X, innerradius=0.5, outerradius=0.8, dielradius=0.78, length=50
@@ -669,15 +668,14 @@
 
         >>> oEditor.CreateBox
         >>> oEditor.AssignMaterial
 
 
         Examples
         --------
-
         This example shows how to create a WG9 waveguide.
 
         >>> from pyaedt import Hfss
         >>> app = Hfss()
         >>> position = [0, 0, 0]
         >>> wg1 = app.modeler.create_waveguide(position, app.AXIS.,
         ...                                    wgmodel="WG9", wg_length=2000)
@@ -798,29 +796,28 @@
 
     @pyaedt_function_handler()
     def objects_in_bounding_box(self, bounding_box, check_solids=True, check_lines=True, check_sheets=True):
         """Given a bounding box checks if objects, sheets and lines are inside it.
 
         Parameters
         ----------
-        bounding_box : list.
+        bounding_box : list
             List of coordinates of bounding box vertices.
             Bounding box is provided as [xmin, ymin, zmin, xmax, ymax, zmax].
-        check_solids : bool, optional.
+        check_solids : bool, optional
             Check solid objects.
-        check_lines : bool, optional.
+        check_lines : bool, optional
             Check line objects.
-        check_sheets : bool, optional.
+        check_sheets : bool, optional
             Check sheet objects.
 
         Returns
         -------
         list of :class:`pyaedt.modeler.object3d`
         """
-
         if len(bounding_box) != 6:
             raise ValueError("Bounding box list must have dimension 6.")
 
         objects = []
         if check_solids:
             for obj in self.solid_objects:
                 bound = obj.bounding_box
@@ -1149,7 +1146,84 @@
                 else:
                     transparency = 0.0
                     color = [40, 40, 40]
                 for obj in added_objs:
                     self[obj].transparency = transparency
                     self[obj].color = color
         return scene
+
+    @pyaedt_function_handler
+    def objects_segmentation(
+        self, objects_list, segmentation_thickness=None, segments_number=None, apply_mesh_sheets=False
+    ):
+        """Get segmentation of an object given the segmentation thickness or number of segments.
+
+        Parameters
+        ----------
+        objects_list : list
+            List of objects to apply the segmentation to.
+            It can either be a list of strings (object names), integers (object IDs), or
+            a list of :class:`pyaedt.modeler.cad.object3d.Object3d` classes.
+        segmentation_thickness : float, optional
+            Segmentation thickness.
+            Model units are automatically assigned. The default is ``None``.
+        segments_number : int, optional
+            Number of segments to segment the object to. The default is ``None``.
+        apply_mesh_sheets : bool, optional
+            Whether to apply mesh sheets to selected objects.
+            Mesh sheets are needed in case the user would like to have additional layers
+            inside the objects for a finer mesh and more accurate results. The default is ``False``.
+
+        Returns
+        -------
+        dict or tuple
+            Depending on value ``apply_mesh_sheets`` it returns either a dictionary or a tuple.
+            If mesh sheets are applied the method returns a tuple where:
+            - First dictionary is the segments that the object has been divided into.
+            - Second dictionary is the mesh sheets eventually needed to apply the mesh.
+            to inside the object. Keys are the object names, and values are respectively
+            segments sheets and mesh sheets of the
+            :class:`pyaedt.modeler.cad.object3d.Object3d` class.
+            If mesh sheets are not applied the method returns only the dictionary of
+            segments that the object has been divided into.
+            ``False`` is returned if the method fails.
+        """
+        if not segmentation_thickness and not segments_number:
+            self.logger.error("Provide at least one option to segment the objects in the list.")
+            return False
+        elif segmentation_thickness and segments_number:
+            self.logger.error("Only one segmentation option can be selected.")
+            return False
+
+        objects_list = self.convert_to_selections(objects_list, True)
+
+        segment_sheets = {}
+        segment_objects = {}
+        for obj_name in objects_list:
+            obj = self[obj_name]
+            if segments_number:
+                segmentation_thickness = obj.top_edge_y.length / segments_number
+            elif segmentation_thickness:
+                segments_number = round(obj.top_edge_y.length / segmentation_thickness)
+            face_object = self.modeler.create_object_from_face(obj.bottom_face_z)
+            # segment sheets
+            segment_sheets[obj.name] = face_object.duplicate_along_line(
+                ["0", "0", segmentation_thickness], segments_number
+            )
+            segment_objects[obj.name] = []
+            for value in segment_sheets[obj.name]:
+                segment_objects[obj.name].append([x for x in self.sheet_objects if x.name == value][0])
+            if apply_mesh_sheets:
+                mesh_sheets = {}
+                mesh_objects = {}
+                # mesh sheets
+                self.move(face_object, [0, 0, segmentation_thickness / 4])
+                mesh_sheets[obj.name] = face_object.duplicate_along_line(
+                    [0, 0, (segmentation_thickness * 2.0) / 4.0], segments_number * 2
+                )
+                mesh_objects[obj.name] = []
+                for value in mesh_sheets[obj.name]:
+                    mesh_objects[obj.name].append([x for x in self.sheet_objects if x.name == value][0])
+        if apply_mesh_sheets:
+            return segment_objects, mesh_objects
+        else:
+            return segment_objects
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.72/pyaedt/modeler/modelerpcb.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.72/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1300,29 +1300,32 @@
 
         .. deprecated:: 0.6.56
            Use :func:`number_with_units` instead.
 
         Parameters
         ----------
         Value :
-
+            The value of the quantity.
         sUnits :
              The default is ``None``.
 
         Returns
         -------
         str
             String containing the value or value and the units if `sUnits` is not ``None``.
+
         """
         warnings.warn("Use :func:`number_with_units` instead.", DeprecationWarning)
         return self._app.number_with_units(Value, sUnits)
 
     @pyaedt_function_handler()
     def number_with_units(self, value, units=None):
-        """Convert a number to a string with units. If value is a string, it's returned as is.
+        """Convert a number to a string with units.
+
+        If value is a string, it's returned as is.
 
         Parameters
         ----------
         value : float, int, str
             Input  number or string.
         units : optional
             Units for formatting. The default is ``None``, which uses ``"meter"``.
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.72/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1027,14 +1027,15 @@
     def negative(self):
         """Get/Set the negative.
 
         Parameters
         ----------
         negative : bool, optional
             The default is ``False``.
+
         Returns
         -------
         type
 
         References
         ----------
 
@@ -1615,14 +1616,16 @@
         Parameters
         ----------
         new_position : List
             New point location.
 
         Returns
         -------
+        bool
+            ``True`` if the point was moved to the new location.
 
         """
         if self.point.Move(self._primitives.oeditor.Point().Set(new_position[0], new_position[1])):
             return True
 
 
 class ComponentsSubCircuit3DLayout(Objec3DLayout, object):
```

### Comparing `pyaedt-0.6.71/pyaedt/modeler/schematic.py` & `pyaedt-0.6.72/pyaedt/modeler/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,16 +36,19 @@
         self._schematic_units = "meter"
         self.o_def_manager = self._app.odefinition_manager
         Modeler.__init__(self, app)
         self.wire = Wire(self)
 
     @property
     def schematic_units(self):
-        """Schematic units. Options are ``"mm"``, ``"mil"``, ``"cm"`` and all other metric and imperial units.
-        The default is ``"meter"``."""
+        """Schematic units.
+
+        Options are ``"mm"``, ``"mil"``, ``"cm"`` and all other metric and imperial units.
+        The default is ``"meter"``.
+        """
         return self._schematic_units
 
     @schematic_units.setter
     def schematic_units(self, value):
         if value in list(AEDT_UNITS["Length"].keys()):
             self._schematic_units = value
         else:
```

### Comparing `pyaedt-0.6.71/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.72/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         elif view != "isometric":
             self.logger.warning("Wrong view setup. It has to be one of xy, xz, yz, isometric.")
 
         if scale_min and scale_max:
             model.range_min = scale_min
             model.range_max = scale_max
         if project_path:
-            model.plot(os.path.join(project_path, self._app.project_name + "." + imageformat))
+            model.plot(os.path.join(project_path, plotname + "." + imageformat))
         elif show:
             model.plot()
         return model
 
     @pyaedt_function_handler()
     def plot_field(
         self,
```

### Comparing `pyaedt-0.6.71/pyaedt/modules/Boundary.py` & `pyaedt-0.6.72/pyaedt/modules/Boundary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.72/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.72/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.72/pyaedt/modules/DesignXPloration.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.72/pyaedt/modules/LayerStackup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 This module provides all layer stackup functionalities for the Circuit and HFSS 3D Layout tools.
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.application.Variables import decompose_variable_value
+from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 @pyaedt_function_handler()
 def _str2bool(str0):
     """Convert a string to a Boolean value.
 
@@ -34,22 +35,23 @@
 
 
 def _conv_number(number, typen=float):
     """Convert a number.
 
     Parameters
     ----------
-    number
+    number : int, float
        Number represented a float.
-
-    typen :
+    typen : type
          The default is ``float``.
 
     Returns
     -------
+    int or float
+        Number converted either to ``int`` or ``float``.
 
     """
     if typen is float:
         try:
             return float(number)
         except:
             return number
@@ -62,54 +64,55 @@
 
 @pyaedt_function_handler()
 def _getIfromRGB(rgb):
     """Retrieve if from a specific layer color.
 
     Parameters
     ----------
-    rgb :
-
+    rgb : list
+        List representing the color. IT is made of 3 values: blue, green, and red.
 
     Returns
     -------
+    int
 
     """
     red = rgb[2]
     green = rgb[1]
     blue = rgb[0]
-    RGBint = (red << 16) + (green << 8) + blue
-    return RGBint
+    rgb_int = (red << 16) + (green << 8) + blue
+    return rgb_int
 
 
 @pyaedt_function_handler()
 def _getRGBfromI(value):
     """Retrieve the Integer from a specific layer color.
 
     Parameters
     ----------
     value : int
-
+        Integer value representing the layer color.
 
     Returns
     -------
     list
+
     """
     r = (value >> 16) & 0xFF
     g = (value >> 8) & 0xFF
     b = (value >> 0) & 0xFF
     return [r, g, b]
 
 
 class Layer(object):
     """Manages the stackup layer for the Circuit and HFSS 3D Layout tools.
 
     Parameters
     ----------
     app : :class:`pyaedt.modules.LayerStackup.Layers`
-
     layertype : string, optional
         The default is ``"signal"``.
     negative : bool, optional
         Whether the geometry on the layer is cut away
         from the layer. The default is ``False``.
 
     Examples
@@ -169,18 +172,19 @@
         self._usp = False
         self.hfssSp = {"si": True, "dt": 0, "dtv": 0.1}
         self.planaremSp = {"ifg": False, "vly": False}
         self._zones = None
 
     @property
     def color(self):
-        """Get/Set the property of the active layer. Color it is list of rgb values (0,255).
+        """Return or set the property of the active layer. Color it is list of rgb values (0,255).
 
         Returns
         -------
+        list
 
         """
         if isinstance(self._color, list):
             return self._color
         else:
             self._color = _getRGBfromI(self._color)
             return self._color
@@ -403,14 +407,27 @@
         self._thickness = self._arg_with_dim(val, self.thickness_units)
         self.update_stackup_layer()
         tck = decompose_variable_value(self._thickness)
         self._thickness = tck[0]
         self._thickness_units = tck[1]
 
     @property
+    def upper_elevation(self):
+        """Get the active layer upper elevation value with units.
+
+        Returns
+        -------
+        float
+        """
+        return (
+            unit_converter(self.thickness, input_units=self.thickness_units, output_units=self.LengthUnit)
+            + self.lower_elevation
+        )
+
+    @property
     def thickness_units(self):
         """Get the active layer thickness units value.
 
         Returns
         -------
         str
         """
@@ -429,40 +446,40 @@
     @lower_elevation.setter
     def lower_elevation(self, val):
         self._lower_elevation = val
         self.update_stackup_layer()
 
     @property
     def roughness(self):
-        """Get/Set the active layer roughness (with units).
+        """Return or set the active layer roughness (with units).
 
         Returns
         -------
         str
         """
         return self._roughness
 
     @roughness.setter
-    def roughness(self, val):
-        self._roughness = val
+    def roughness(self, value):
+        self._roughness = value
         self.update_stackup_layer()
 
     @property
     def bottom_roughness(self):
-        """Get/Set the active layer bottom roughness (with units).
+        """Return or set the active layer bottom roughness (with units).
 
         Returns
         -------
         str
         """
         return self._botroughness
 
     @bottom_roughness.setter
-    def bottom_roughness(self, val):
-        self._botroughness = val
+    def bottom_roughness(self, value):
+        self._botroughness = value
         self.update_stackup_layer()
 
     @property
     def top_roughness(self):
         """Get/Set the active layer top roughness (with units).
 
         Returns
@@ -873,21 +890,23 @@
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
         """Argument with dimensions.
 
         Parameters
         ----------
-        value :
-
+        value : str, float
+            Value of the quantity.
         units :
-             The default is ``None``.
+            Unit of the quantity. The default is ``None``.
 
         Returns
         -------
+        str
+            String containing both the value and the unit properly formatted.
 
         """
         if units is None:
             units = self.LengthUnit
         if type(value) is str:
             try:
                 float(value)
@@ -1135,15 +1154,16 @@
     @property
     def oeditor(self):
         """Editor.
 
         References
         ----------
 
-        >>> oEditor = oDesign.SetActiveEditor("Layout")"""
+        >>> oEditor = oDesign.SetActiveEditor("Layout")
+        """
         return self._modeler.oeditor
 
     @property
     def zones(self):
         """List of all available zones.
 
         Returns
@@ -1188,15 +1208,14 @@
            List of drawing layers.
 
         References
         ----------
 
         >>> oEditor.GetAllLayerNames()
         """
-
         return [v for k, v in self.layers.items() if v.type not in ["signal", "via", "dielectric"]]
 
     @property
     def stackup_layers(self):
         """All stackup layers.
 
         Returns
@@ -1205,27 +1224,25 @@
            List of stackup layers.
 
         References
         ----------
 
         >>> oEditor.GetAllLayerNames()
         """
-
         return [v for k, v in self.layers.items() if v.type in ["signal", "via", "dielectric"]]
 
     @property
     def all_signal_layers(self):
         """All signal layers.
 
         Returns
         -------
         List of :class:`pyaedt.modules.LayerStackup.Layer`
             List of signal layers.
         """
-
         return [v for k, v in self.layers.items() if v.type == "signal"]
 
     @property
     def signals(self):
         """All signal layers.
 
         Returns
@@ -1266,15 +1283,14 @@
            Drawing layers.
 
         References
         ----------
 
         >>> oEditor.GetAllLayerNames()
         """
-
         return {k: v for k, v in self.layers.items() if v.type in ["signal", "via", "dielectric"]}
 
     @property
     def all_diel_layers(self):
         """All dielectric layers.
 
         Returns
@@ -1286,15 +1302,15 @@
 
     @pyaedt_function_handler()
     def layer_id(self, name):
         """Retrieve a layer ID.
 
         Parameters
         ----------
-        name :  str
+        name : str
             Name of the layer.
 
         Returns
         -------
         :class:`pyaedt.modules.LayerStackup.Layer`
             Layer objecy if the layer name exists.
         """
@@ -1305,15 +1321,15 @@
 
     @property
     def layers(self):
         """Refresh all layers in the current stackup.
 
         Returns
         -------
-         Dict[int,  :class:`pyaedt.modules.LayerStackup.Layer`]
+         Dict[int, :class:`pyaedt.modules.LayerStackup.Layer`]
             Number of layers in the current stackup.
         """
         layers = OrderedDict({})
         for el in self.all_layers:
             o = Layer(self, "signal")
             o.name = el
             infos = self.oeditor.GetLayerInfo(el)
@@ -1336,16 +1352,19 @@
                 o._is_visible_shape = _str2bool(infosdict["IsVisibleShape"])
                 o._is_visible_hole = _str2bool(infosdict["IsVisibleHole"])
             o._color = _getRGBfromI(int(infosdict["Color"][:-1]))
             if o.type in ["signal", "dielectric", "via"]:
                 o._index = int(infosdict["Index"])
                 tck = decompose_variable_value(infosdict["LayerThickness"])
                 o._thickness = tck[0]
-                o._thickness_units = tck[1]
-                o._lower_elevation = decompose_variable_value(infosdict["LowerElevation0"])[0]
+                o._thickness_units = tck[1] if tck[1] else "meter"
+                tck = decompose_variable_value(infosdict["LowerElevation0"])
+
+                o._lower_elevation = tck[0]
+                o.LengthUnit = tck[1] if tck[1] else "meter"
                 o._fillmaterial = infosdict["FillMaterial0"]
                 o._material = infosdict["Material0"]
                 if "EtchFactor" in infosdict:
                     o._useetch = True
                     o._etch = decompose_variable_value(infosdict["EtchFactor"])[0]
                 if "Roughness0 Type" in infosdict:
                     o._user = True
@@ -1395,26 +1414,20 @@
         newlayer.name = layername
         newlayer._thickness = thickness
 
         if elevation == "0mm":
             el = (
                 0
                 if list(self.layers.values())[0].type not in ["dielectric", "signal", "via"]
-                else "{}+{}".format(
-                    list(self.layers.values())[0].lower_elevation, list(self.layers.values())[0].thickness
+                else "{}{}".format(
+                    list(self.layers.values())[0].upper_elevation, list(self.layers.values())[0].LengthUnit
                 )
             )
             if el:
-                self._app.variable_manager.set_variable(
-                    "pyaedt_evaluator",
-                    expression=el,
-                    readonly=True,
-                    hidden=True,
-                )
-                newlayer._lower_elevation = self._app.get_evaluated_value("pyaedt_evaluator")
+                newlayer._lower_elevation = el
             else:
                 newlayer._lower_elevation = "0mm"
         else:
             newlayer._lower_elevation = elevation
         newlayer._material = material
         newlayer.create_stackup_layer()
```

### Comparing `pyaedt-0.6.71/pyaedt/modules/Material.py` & `pyaedt-0.6.72/pyaedt/modules/Material.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.72/pyaedt/modules/MaterialLib.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/Mesh.py` & `pyaedt-0.6.72/pyaedt/modules/Mesh.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.72/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.72/pyaedt/modules/MeshIcepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.72/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.72/pyaedt/modules/PostProcessor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1200,38 +1200,47 @@
 
         >>> oModule.ExportReportDataToFile
         >>> oModule.ExportToFile
         """
         return self.export_report_to_file(project_dir, plot_name, extension=".csv")
 
     @pyaedt_function_handler()
-    def export_report_to_jpg(self, project_dir, plot_name):
+    def export_report_to_jpg(self, project_dir, plot_name, width=0, height=0):
         """Export the SParameter plot to a JPG file.
 
         Parameters
         ----------
         project_dir : str
             Path to the project directory.
         plot_name : str
             Name of the plot to export.
+        width : int, optional
+            Image width. Default is ``0`` which takes Desktop size or 500 pixel in case of non-graphical mode.
+        height : int, optional
+            Image height. Default is ``0`` which takes Desktop size or 500 pixel in case of non-graphical mode.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ExportImageToFile
         """
         # path
         npath = project_dir
         file_name = os.path.join(npath, plot_name + ".jpg")  # name of the image file
-        self.oreportsetup.ExportImageToFile(plot_name, file_name, 0, 0)
+        if settings.non_graphical:
+            if width == 0:
+                width = 500
+            if height == 0:
+                height = 500
+        self.oreportsetup.ExportImageToFile(plot_name, file_name, width, height)
         return True
 
     @pyaedt_function_handler()
     def _get_report_inputs(
         self,
         expressions,
         setup_sweep_name=None,
@@ -3154,14 +3163,19 @@
         if self._app.design_type in ["HFSS 3D Layout Design", "Circuit Design", "Maxwell Circuit", "Twin Builder"]:
             if width == 0:
                 width = 1920
             if height == 0:
                 height = 1080
             self.oeditor.ExportImage(full_name, width, height)
         else:
+            if settings.non_graphical:
+                if width == 0:
+                    width = 500
+                if height == 0:
+                    height = 500
             self.oeditor.ExportModelImageToFile(full_name, width, height, arg)
         return full_name
 
     @pyaedt_function_handler()
     def get_far_field_data(
         self, expression="GainTotal", setup_sweep_name="", domain="Infinite Sphere1", families_dict=None
     ):
@@ -3327,18 +3341,18 @@
 
     @pyaedt_function_handler()
     def power_budget(self, units="W", temperature=22):
         """Power budget calculation.
 
         Parameters
         ----------
-        units : str
-            Output power units.
-        temperature : float
-            Temperature to calculate the power.
+        units : str, optional
+            Output power units. The default is ``"W"``.
+        temperature : float, optional
+            Temperature to calculate the power. The default is ``22``.
 
         Returns
         -------
         dict, float
             Dictionary with the power introduced on each boundary and total power.
 
         References
@@ -3622,15 +3636,14 @@
         incident_phi=0,
         is_vertical_polarization=False,
     ):
         """Create a Creeping Wave Plane Wave Visual Ray Tracing and return the class object.
 
         Parameters
         ----------
-
         max_frequency : str, optional
             Maximum Frequency. Default is ``"1GHz"``.
         ray_density : int, optional
             Ray Density. Default is ``2``.
         sample_density : int, optional
             Sample density. Default is ``10``.
         ray_cutoff : int, optional
@@ -3670,15 +3683,14 @@
         irregular_surface_tolerance=50,
         custom_location=None,
     ):
         """Create a Creeping Wave Point Source Visual Ray Tracing and return the class object.
 
         Parameters
         ----------
-
         max_frequency : str, optional
             Maximum Frequency. Default is ``"1GHz"``.
         ray_density : int, optional
             Ray Density. Default is ``2``.
         sample_density : int, optional
             Sample density. Default is ``10``.
         ray_cutoff : int, optional
@@ -3725,15 +3737,14 @@
         ray_index_step=1,
         ray_box=None,
     ):
         """Create an SBR Plane Wave Visual Ray Tracing and return the class object.
 
         Parameters
         ----------
-
         max_frequency : str, optional
             Maximum Frequency. Default is ``"1GHz"``.
         ray_density : int, optional
             Ray Density. Default is ``2``.
         number_of_bounces : int, optional
             Maximum number of bounces. Default is ``5``.
         multi_bounce : bool, optional
```

### Comparing `pyaedt-0.6.71/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.72/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.72/pyaedt/modules/SolveSetup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 This module provides all functionalities for creating and editing setups in AEDT.
 It is based on templates to allow for easy creation and modification of setup properties.
 
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
+import copy
 import logging
 import os.path
 from random import randrange
 import time
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import pyaedt_function_handler
+from pyaedt.modules.SetupTemplates import MaxwellTransient
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSweeps import SetupProps
 from pyaedt.modules.SolveSweeps import SweepHFSS
 from pyaedt.modules.SolveSweeps import SweepHFSS3DLayout
 from pyaedt.modules.SolveSweeps import SweepMatrix
 from pyaedt.modules.SolveSweeps import identify_setup
 
@@ -1642,20 +1644,20 @@
     def export_to_json(self, file_path, overwrite=False):
         """Export all setup properties into a json file.
 
         Parameters
         ----------
         file_path : str
             File path of the json file.
-        overwrite : bool
+        overwrite : bool, optional
             Whether to overwrite the file if it already exists.
         """
         if os.path.isdir(file_path):  # pragma no cover
             if not overwrite:  # pragma no cover
-                raise logging.error("File {} already exists. Configure file is not exported".format(file_path))
+                logging.error("File {} already exists. Configure file is not exported".format(file_path))
         return self.props._export_properties_to_json(file_path)
 
 
 class SetupHFSS(Setup, object):
     """Initializes, creates, and updates an HFSS setup.
 
     Parameters
@@ -2581,14 +2583,84 @@
         else:
             self.props["SweepRanges"]["Subrange"] = [self.props["SweepRanges"]["Subrange"], props]
         self.props["SaveAllFields"] = save_all_fields
         self.update()
         self.auto_update = legacy_update
         return True
 
+    @pyaedt_function_handler()
+    def enable_control_program(self, control_program_path, control_program_args=" ", call_after_last_step=False):
+        """Enable control program option is solution setup.
+        Provide externally created executable files, or Python (*.py) scripts that are called after each time step,
+        and allow you to control the source input, circuit elements, mechanical quantities, time step,
+        and stopping criteria, based on the updated solutions.
+
+        Parameters
+        ----------
+        control_program_path : str
+            File path of control program.
+        control_program_args : str, optional
+            Arguments to pass to control program.
+            Default value is ``" "``.
+        call_after_last_step : bool, optional
+            If ``True`` the control program is called after the simulation is completed.
+            Default value is ``False``.
+
+        Returns
+        -------
+        bool
+            ``True`` if successful, ``False`` if it fails.
+
+        Notes
+        -----
+        By default a control program script will be called by the pre-installed Python interpreter:
+        ``<install_path>\Win64\commonfiles\CPython\37\winx64\Release\python\python.exe``.
+        However, the user can specify a custom Python interpreter to be used by setting following environment variable:
+        ``EM_CTRL_PROG_PYTHON_PATH=<path_to\python.exe>``
+
+        References
+        ----------
+        >>> oModule.EditSetup
+        """
+        if self.p_app.solution_type not in ["Transient", "TransientXY", "TransientZ"]:
+            self._app.logger.error("Control Program is only available in Maxwell 2D and 3D Transient solutions.")
+            return False
+
+        if not os.path.exists(control_program_path):
+            self._app.logger.error("Control Program file does not exist.")
+            return False
+
+        if not isinstance(control_program_args, str):
+            self._app.logger.error("Control Program arguments have to be a string.")
+            return False
+
+        self.props = copy.deepcopy(MaxwellTransient)
+        self.props["UseControlProgram"] = True
+        self.props["ControlProgramName"] = control_program_path
+        self.props["ControlProgramArg"] = control_program_args
+        self.props["CallCtrlProgAfterLastStep"] = call_after_last_step
+
+        self.p_app.oanalysis.EditSetup(
+            self.name,
+            [
+                "NAME:" + self.name,
+                "Enabled:=",
+                True,
+                "UseControlProgram:=",
+                True,
+                "ControlProgramName:=",
+                control_program_path,
+                "ControlProgramArg:=",
+                control_program_args,
+                "CallCtrlProgAfterLastStep:=",
+                call_after_last_step,
+            ],
+        )
+        return True
+
 
 class SetupQ3D(Setup, object):
     """Initializes, creates, and updates an Q3D setup.
 
     Parameters
     ----------
     app : :class:`pyaedt.application.Analysis3D.FieldAnalysis3D`
```

### Comparing `pyaedt-0.6.71/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.72/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.72/pyaedt/modules/monitor_icepak.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/report_templates.py` & `pyaedt-0.6.72/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/modules/solutions.py` & `pyaedt-0.6.72/pyaedt/modules/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,16 @@
             except:
                 self.units_sweeps[intrinsic] = None
         self.init_solutions_data()
         self._ifft = None
 
     @property
     def enable_pandas_output(self):
-        """Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
+        """
+        Set/Get a flag to use Pandas to export dict and lists. This applies to Solution data output.
         If ``True`` the property or method will return a pandas object in CPython environment.
         Default is ``False``.
 
         Returns
         -------
         bool
         """
@@ -209,34 +210,36 @@
                 if v not in self._sweeps_names:
                     self._sweeps_names.append(v)
         self._sweeps_names.extend((reversed(names)))
 
     @staticmethod
     @pyaedt_function_handler()
     def _quantity(unit):
-        """
+        """Get the corresponding AEDT units.
 
         Parameters
         ----------
-        unit :
-
+        unit : str
+            The unit to be looked among the available AEDT units.
 
         Returns
         -------
+            str
+            The AEDT units.
 
         """
         for el in AEDT_UNITS:
             keys_units = [i.lower() for i in list(AEDT_UNITS[el].keys())]
             if unit.lower() in keys_units:
                 return el
         return None
 
     @pyaedt_function_handler()
     def init_solutions_data(self):
-        "Initialize the database and store info in variables."
+        """Initialize the database and store info in variables."""
         self._solutions_real = self._init_solution_data_real()
         self._solutions_imag = self._init_solution_data_imag()
         self._solutions_mag = self._init_solution_data_mag()
         self._solutions_phase = self._init_solution_data_phase()
 
     @pyaedt_function_handler()
     def _init_solution_data_mag(self):
@@ -1264,15 +1267,16 @@
         row_max = np.max(rows)
         col_min = np.min(cols)
         col_max = np.max(cols)
         return [col_min, col_max, row_min, row_max]
 
     @pyaedt_function_handler()
     def array_center_and_edge(self):
-        """Find the center and edge of our array, assumes all ports in far field
+        """
+        Find the center and edge of our array, assuming all ports in far field
         mapping file are active ports.
 
         Returns
         -------
         bool
         """
         AMax = 0
@@ -1995,18 +1999,14 @@
         title : str, optional
             Plot title. Default `"3D Plot"`.
         convert_to_db : bool, optional
             Either if the quantity has to be converted in db or not. Default is `True`.
         export_image_path : str, optional
             Full path to image file. Default is None to not export.
 
-
-        Returns
-        -------
-
         """
         data = self.beamform(phi_scan, theta_scan)
 
         if convert_to_db:
             ff_data = 10 * np.log10(data[qty_str])
             # renormalize to 0 and 1
             ff_max_dB = np.max(ff_data)
@@ -2434,20 +2434,20 @@
 
         self.ff._get_far_field_mesh(self.qty_str, self.convert_to_db)
 
         self.output.overwrite(self.ff.mesh)
         return
 
     def update_phi(self, phi):
-        """Updates the Pyvista Plot with new phi value."""
+        """Update the Pyvista Plot with new phi value."""
         self._phi = phi
         self._update_both()
 
     def update_theta(self, theta):
-        """Updates the Pyvista Plot with new theta value."""
+        """Update the Pyvista Plot with new theta value."""
         self._theta = theta
         self._update_both()
 
 
 class Update2BeamForms:
     def __init__(self, ff, max_value=1):
         self.max_value = max_value
@@ -2469,25 +2469,25 @@
         current_max = np.max(self.ff.mesh["FarFieldData"])
         delta = self.max_value - current_max
         self.ff.mesh["FarFieldData"] = self.ff.mesh["FarFieldData"] - delta
         self.output.overwrite(self.ff.mesh)
         return
 
     def update_phi1(self, phi1):
-        """Updates the Pyvista Plot with new phi1 value."""
+        """Update the Pyvista Plot with new phi1 value."""
         self._phi1 = phi1
         self._update_both()
 
     def update_theta1(self, theta1):
-        """Updates the Pyvista Plot with new theta1 value."""
+        """Update the Pyvista Plot with new theta1 value."""
         self._theta1 = theta1
         self._update_both()
 
     def update_phi2(self, phi2):
-        """Updates the Pyvista Plot with new phi2 value."""
+        """Update the Pyvista Plot with new phi2 value."""
         self._phi2 = phi2
         self._update_both()
 
     def update_theta2(self, theta2):
         """Updates the Pyvista Plot with new theta2 value."""
         self._theta2 = theta2
         self._update_both()
@@ -2495,15 +2495,14 @@
 
 class FieldPlot:
     """Creates and edits field plots.
 
     Parameters
     ----------
     postprocessor : :class:`pyaedt.modules.PostProcessor.PostProcessor`
-
     objlist : list
         List of objects.
     solutionName : str
         Name of the solution.
     quantityName : str
         Name of the plot or the name of the object.
     intrinsincList : dict, optional
@@ -2769,15 +2768,15 @@
         ]
 
     @property
     def surfacePlotInstructionLineTraces(self):
         """Surface plot settings for field line traces.
 
         ..note::
-            ``Specify seeding points on selections`` is by default set to ''by sampling''.
+            ``Specify seeding points on selections`` is by default set to ``by sampling``.
 
         Returns
         -------
         list
             List of plot settings for line traces.
 
         """
@@ -3152,41 +3151,44 @@
 
 class VRTFieldPlot:
     """Creates and edits VRT field plots for SBR+ and Creeping Waves.
 
     Parameters
     ----------
     postprocessor : :class:`pyaedt.modules.PostProcessor.PostProcessor`
-
-    objlist : list
-        List of objects.
-    solutionName : str
-        Name of the solution.
-    quantity_name : str
+    is_creeping_wave : bool
+        Whether it is a creeping wave model or not.
+    quantity_name : str, optional
         Name of the plot or the name of the object.
-    intrinsincList : dict, optional
+    max_frequency : str, optional
+        Maximum Frequency. The default is ``"1GHz"``.
+    ray_density : int, optional
+        Ray Density. The default is ``2``.
+    bounces : int, optional
+        Maximum number of bounces. The default is ``5``.
+    intrinsinc_list : dict, optional
         Name of the intrinsic dictionary. The default is ``{}``.
 
     """
 
     def __init__(
         self,
         postprocessor,
         is_creeping_wave=False,
         quantity_name="QuantityName_SBR",
         max_frequency="1GHz",
         ray_density=2,
         bounces=5,
-        intrinsincList={},
+        intrinsinc_list={},
     ):
         self.is_creeping_wave = is_creeping_wave
         self._postprocessor = postprocessor
         self._ofield = postprocessor.ofieldsreporter
         self.quantity_name = quantity_name
-        self.intrinsics = intrinsincList
+        self.intrinsics = intrinsinc_list
         self.name = "Field_Plot"
         self.plot_folder = "Field_Plot"
         self.max_frequency = max_frequency
         self.ray_density = ray_density
         self.number_of_bounces = bounces
         self.multi_bounce_ray_density_control = False
         self.mbrd_max_subdivision = 2
@@ -3365,15 +3367,14 @@
         except:
             return False
 
     @pyaedt_function_handler()
     def update(self):
         """Update the field plot.
 
-
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         try:
             if self.is_creeping_wave:
```

### Comparing `pyaedt-0.6.71/pyaedt/q3d.py` & `pyaedt-0.6.72/pyaedt/q3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -2100,16 +2100,15 @@
             port,
             aedt_process_id,
         )
         self.MATRIXOPERATIONS = MATRIXOPERATIONSQ2D()
 
     @pyaedt_function_handler()
     def create_rectangle(self, position, dimension_list, name="", matname=""):
-        """
-        Create a rectangle.
+        """Create a rectangle.
 
         Parameters
         ----------
         position : list
             List of ``[x, y]`` coordinates for the starting point of the rectangle.
         dimension_list : list
             List of ``[width, height]`` dimensions.
```

### Comparing `pyaedt-0.6.71/pyaedt/rmxprt.py` & `pyaedt-0.6.72/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.72/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.72/pyaedt/sbrplus/hdm_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
                 res = res[0]
         self.idx = end
         return res
 
     def _parse_list(self, type=None, base=None, size=1):
         """
         Parser for vector or list. 'vector's are to be interpreted in the linear algebra sense,
-        and converted to numpy.array. 'list's are python lists. Only simple base types can be
+        and converted to numpy.array. 'list's are Python lists. Only simple base types can be
         interpreted as a numpy array
         """
         assert base != None
         res = []
         bt = self.parser_types[base]
 
         if bt["type"] == "internal":
```

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.72/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.72/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.72/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/siwave.py` & `pyaedt-0.6.72/pyaedt/siwave.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyaedt/twinbuilder.py` & `pyaedt-0.6.72/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.71/pyproject.toml` & `pyaedt-0.6.72/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -21,101 +21,101 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 
 dependencies = [
-    "cffi == 1.15.0;platform_system=='Linux'",
+    "cffi == 1.15.1;platform_system=='Linux'",
     "pywin32 >= 303;platform_system=='Windows'",
     "pythonnet == 3.0.1",
-    "rpyc==5.3.0",
+    "rpyc==5.3.1",
     "psutil",
     "dotnetcore2 ==3.1.23;platform_system=='Linux'",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "ipython==8.8.0",
+    "ipython==8.12.0",
     "joblib==1.2.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
-    "numpy==1.24.1; python_version > '3.7'",
-    "openpyxl==3.0.10",
+    "numpy==1.24.3; python_version > '3.7'",
+    "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==1.5.3; python_version > '3.7'",
-    "pytest==7.2.2",
+    "pandas==2.0.1; python_version > '3.7'",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
-    "pytest-xdist==3.2.0",
-    "pyvista==0.37.0",
-    "scikit-learn==1.2.0",
+    "pytest-xdist==3.2.1",
+    "pyvista==0.38.5",
+    "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
-    "ansys-sphinx-theme==0.8.0",
-    "imageio==2.26.1",
+    "ansys-sphinx-theme==0.9.8",
+    "imageio==2.28.0",
     "imageio-ffmpeg==0.4.8",
-    "ipython==8.8.0",
-    "ipywidgets==8.0.4",
+    "ipython==8.12.0",
+    "ipywidgets==8.0.6",
     "joblib==1.2.0",
-    "jupyterlab==3.5.2",
+    "jupyterlab==3.6.3",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
-    "nbsphinx==0.8.12",
+    "nbsphinx==0.9.1",
     "numpydoc==1.5.0",
     "osmnx",
-    "pypandoc==1.10",
+    "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.37.0",
+    "pyvista==0.38.5",
     "recommonmark==0.7.1",
-    "scikit-learn==1.2.0",
-    "Sphinx==5.3.0",
+    "scikit-learn==1.2.2",
+    "Sphinx==6.2.1",
     "sphinx-autobuild==2021.3.14",
-    "sphinx-autodoc-typehints==1.21.7",
-    "sphinx-copybutton==0.5.1",
-    "sphinx-gallery==0.11.1",
+    "sphinx-autodoc-typehints==1.23.0",
+    "sphinx-copybutton==0.5.2",
+    "sphinx-gallery==0.13.0",
     "sphinx-notfound-page==0.8.3",
     "sphinxcontrib-websupport==1.2.4",
     "SRTM.py",
     "utm",
     "scikit-rf",
-    "openpyxl==3.0.10",
+    "openpyxl==3.1.2",
 ]
 full = [
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
-    "numpy==1.24.1; python_version > '3.7'",
+    "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==1.5.3; python_version > '3.7'",
+    "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.37.0",
+    "pyvista==0.38.5",
     "SRTM.py",
     "utm",
     "scikit-rf",
-    "openpyxl==3.0.10",
+    "openpyxl==3.1.2",
 ]
 all = [
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
-    "numpy==1.24.1; python_version > '3.7'",
+    "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
-    "pandas==1.5.3; python_version > '3.7'",
+    "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.37.0",
+    "pyvista==0.38.5",
     "SRTM.py",
     "utm",
     "scikit-rf",
-    "openpyxl==3.0.10",
+    "openpyxl==3.1.2",
 ]
 
 [tool.flit.module]
 name = "pyaedt"
 
 [project.urls]
 "Bug Tracker" = "https://github.com/pyansys/pyaedt/issues"
```

### Comparing `pyaedt-0.6.71/PKG-INFO` & `pyaedt-0.6.72/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,97 +1,97 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.71
+Version: 0.6.72
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: cffi == 1.15.0;platform_system=='Linux'
+Requires-Dist: cffi == 1.15.1;platform_system=='Linux'
 Requires-Dist: pywin32 >= 303;platform_system=='Windows'
 Requires-Dist: pythonnet == 3.0.1
-Requires-Dist: rpyc==5.3.0
+Requires-Dist: rpyc==5.3.1
 Requires-Dist: psutil
 Requires-Dist: dotnetcore2 ==3.1.23;platform_system=='Linux'
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
-Requires-Dist: numpy==1.24.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
-Requires-Dist: pandas==1.5.3 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.37.0 ; extra == "all"
+Requires-Dist: pyvista==0.38.5 ; extra == "all"
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
-Requires-Dist: openpyxl==3.0.10 ; extra == "all"
-Requires-Dist: ansys-sphinx-theme==0.8.0 ; extra == "doc"
-Requires-Dist: imageio==2.26.1 ; extra == "doc"
+Requires-Dist: openpyxl==3.1.2 ; extra == "all"
+Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: imageio==2.28.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
-Requires-Dist: ipython==8.8.0 ; extra == "doc"
-Requires-Dist: ipywidgets==8.0.4 ; extra == "doc"
+Requires-Dist: ipython==8.12.0 ; extra == "doc"
+Requires-Dist: ipywidgets==8.0.6 ; extra == "doc"
 Requires-Dist: joblib==1.2.0 ; extra == "doc"
-Requires-Dist: jupyterlab==3.5.2 ; extra == "doc"
+Requires-Dist: jupyterlab==3.6.3 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
-Requires-Dist: nbsphinx==0.8.12 ; extra == "doc"
+Requires-Dist: nbsphinx==0.9.1 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
-Requires-Dist: pypandoc==1.10 ; extra == "doc"
+Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.37.0 ; extra == "doc"
+Requires-Dist: pyvista==0.38.5 ; extra == "doc"
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
-Requires-Dist: scikit-learn==1.2.0 ; extra == "doc"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
+Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
-Requires-Dist: sphinx-autodoc-typehints==1.21.7 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: sphinx-gallery==0.11.1 ; extra == "doc"
+Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
 Requires-Dist: sphinx-notfound-page==0.8.3 ; extra == "doc"
 Requires-Dist: sphinxcontrib-websupport==1.2.4 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: scikit-rf ; extra == "doc"
-Requires-Dist: openpyxl==3.0.10 ; extra == "doc"
+Requires-Dist: openpyxl==3.1.2 ; extra == "doc"
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
-Requires-Dist: numpy==1.24.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
-Requires-Dist: pandas==1.5.3 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.37.0 ; extra == "full"
+Requires-Dist: pyvista==0.38.5 ; extra == "full"
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
-Requires-Dist: openpyxl==3.0.10 ; extra == "full"
-Requires-Dist: ipython==8.8.0 ; extra == "tests"
+Requires-Dist: openpyxl==3.1.2 ; extra == "full"
+Requires-Dist: ipython==8.12.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
 Requires-Dist: matplotlib==3.5.3 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: numpy==1.24.1 ; extra == "tests" and ( python_version > '3.7')
-Requires-Dist: openpyxl==3.0.10 ; extra == "tests"
+Requires-Dist: numpy==1.24.3 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
-Requires-Dist: pandas==1.5.3 ; extra == "tests" and ( python_version > '3.7')
-Requires-Dist: pytest==7.2.2 ; extra == "tests"
+Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
-Requires-Dist: pytest-xdist==3.2.0 ; extra == "tests"
-Requires-Dist: pyvista==0.37.0 ; extra == "tests"
-Requires-Dist: scikit-learn==1.2.0 ; extra == "tests"
+Requires-Dist: pytest-xdist==3.2.1 ; extra == "tests"
+Requires-Dist: pyvista==0.38.5 ; extra == "tests"
+Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Source Code, https://github.com/pyansys/pyaedt
 Provides-Extra: all
@@ -136,67 +136,69 @@
 .. |pre-commit| image:: https://results.pre-commit.ci/badge/github/pyansys/pyaedt/main.svg
    :target: https://results.pre-commit.ci/latest/github/pyansys/pyaedt/main
    :alt: pre-commit.ci status
 
 
 What is PyAEDT?
 ---------------
-PyAEDT is a Python library that interacts directly with the AEDT API
-to make scripting simpler for the end user. Its architecture
-can be reused for all AEDT 3D products (HFSS, Icepak, Maxwell 3D, and
-Q3D Extractor), 2D tools, and Ansys Mechanical. It also provides support for circuit
-tools like Nexxim and system simulation tools like Twin Builder. Finally it provides
-scripting capabilities in Ansys layout tools like HFSS 3D Layout and EDB. Its class
-and method structures simplify operation for the end user while reusing information
-as much as possible across the API.
+PyAEDT is a Python library that interacts directly with the API for
+Ansys Electronics Desktop (AEDT) to make scripting simpler. The architecture
+for PyAEDT can be reused for all AEDT 3D products (HFSS, Icepak, Maxwell 3D,
+and Q3D Extractor), 2D tools, and Ansys Mechanical. PyAEDT also provides
+support for circuit tools like Nexxim and system simulation tools like
+Twin Builder. Finally, PyAEDT provides scripting capabilities in Ansys layout
+tools like HFSS 3D Layout and EDB. The PyAEDT class and method structures
+simplify operation while reusing information as much as possible across
+the API.
 
 Install on CPython from PyPI
 ----------------------------
-You can install PyAEDT on CPython 3.7 through 3.10 from PyPI:
+You can install PyAEDT on CPython 3.7 through 3.10 from PyPI with this command:
 
 .. code:: python
 
     pip install pyaedt
 
-Install PyAEDT with all extra packages (matplotlib, numpy, pandas, pyvista):
+To install PyAEDT with all extra packages (Matplotlib, NumPy, Pandas, and PyVista),
+use this command:
 
 .. code:: python
 
     pip install pyaedt[full]
 
-You can also install PyAEDT from Conda-Forge:
+You can also install PyAEDT from Conda-Forge with this command:
 
 .. code:: python
 
     conda install -c conda-forge pyaedt
 
-PyAEDT remains compatible with Ironpython and can be still used in AEDT Framework.
+PyAEDT remains compatible with IronPython and can be still used in the AEDT Framework.
 
 About PyAnsys
 -------------
 
 PyAEDT is part of the larger `PyAnsys <https://docs.pyansys.com>`_
 effort to facilitate the use of Ansys technologies directly from Python.
 
 PyAEDT is intended to consolidate and extend all existing
-functionalities around scripting for Ansys Electronics Desktop (AEDT)
-to allow reuse of existing code, sharing of best practices, and increased
-collaboration.
+functionalities around scripting for AEDT to allow reuse of existing code,
+sharing of best practices, and increased collaboration.
 
 
 About AEDT
 ----------
 
-The Ansys Electronics Desktop (AEDT) is a platform that enables true electronics system design.
-`AEDT <https://www.ansys.com/products/electronics>`_ provides access to the Ansys gold-standard
-electro-magnetics simulation solutions such as Ansys HFSS,
-Ansys Maxwell, Ansys Q3D Extractor, Ansys Siwave, and Ansys Icepak using electrical CAD (ECAD) and
+`AEDT <https://www.ansys.com/products/electronics>`_ is a platform that enables true
+electronics system design. AEDT provides access to the Ansys gold-standard
+electro-magnetics simulation solutions, such as Ansys HFSS, Ansys Maxwell,
+Ansys Q3D Extractor, Ansys Siwave, and Ansys Icepak using electrical CAD (ECAD) and
 Mechanical CAD (MCAD) workflows.
-In addition, it includes direct links to the complete Ansys portfolio of thermal, fluid,
-and Mechanical solvers for comprehensive multiphysics analysis.
+
+In addition, AEDT includes direct links to the complete Ansys portfolio of thermal, fluid,
+and mechanical solvers for comprehensive multiphysics analysis.
 Tight integration among these solutions provides unprecedented ease of use for setup and
 faster resolution of complex simulations for design and optimization.
 
 .. image:: https://images.ansys.com/is/image/ansys/ansys-electronics-technology-collage?wid=941&op_usm=0.9,1.0,20,0&fit=constrain,0
   :width: 800
   :alt: AEDT Applications
   :target: https://www.ansys.com/products/electronics
@@ -215,50 +217,54 @@
 - Nexxim
 - EDB
 - Twin Builder
 
 
 Documentation and issues
 ------------------------
-In addition to installation and usage information, the PyAEDT
-documentation provides `API reference <https://aedt.docs.pyansys.com/release/0.6/API/index.html>`_,
-`Examples <https://aedt.docs.pyansys.com/release/0.6/examples/index.html>`_, and `Contribute 
-<https://aedt.docs.pyansys.com/release/0.6/Contributing.html>`_ sections.
+Documentation for the latest stable release of PyAEDT is hosted at
+`PyAEDT Documentation <https://aedt.docs.pyansys.com/version/stable/>`_.
+
+In the upper right corner of the documentation's title bar, there is an option
+for switching from viewing the documentation for the latest stable release
+to viewing the documentation for the development version or previously
+released versions.
 
 On the `PyAEDT Issues <https://github.com/pyansys/PyAEDT/issues>`_ page, you can
-create issues to submit questions, report bugs, and request new features. To reach
-the project support team, email `pyansys.support@ansys.com <pyansys.support@ansys.com>`_.
+create issues to submit questions, report bugs, and request new features.
+
+To reach the project support team, email `pyansys.core@ansys.com <pyansys.core@ansys.com>`_.
 
 Dependencies
 ------------
-To run PyAEDT, you must have a local licenced copy of AEDT.
-PyAEDT supports AEDT versions 2022 R1 or newer.
+To run PyAEDT, you must have a local licensed copy of AEDT.
+PyAEDT supports AEDT versions 2022 R1 and later.
 
 Student version
 ---------------
 
-PyAEDT supports AEDT Student version 2022 R1 and later. For more information, see
-`Student Version page <https://www.ansys.com/academic/students/ansys-e
-lectronics-desktop-student>`_.
+PyAEDT supports AEDT Student versions 2022 R1 and later. For more information, see
+`Ansys Electronics Desktop Student  - Free Software Download <https://www.ansys.com/academic/students/ansys-e
+lectronics-desktop-student>`_ on the Ansys website.
 
 
 Why PyAEDT?
 -----------
 A quick and easy approach for automating a simple operation in the 
-AEDT UI is to record and reuse a script. However, disadvantages of 
-this approach are:
+AEDT UI is to record and reuse a script. However, here are some disadvantages of 
+this approach:
 
 - Recorded code is dirty and difficult to read and understand.
 - Recorded scripts are difficult to reuse and adapt.
 - Complex coding is required by many global users of AEDT.
 
-The main advantages of PyAEDT are:
+Here are the main advantages that PyAEDT provides:
 
 - Automatic initialization of all AEDT objects, such as desktop
-  objects like the editor, boundaries, and so on
+  objects like the editor, boundaries, and more
 - Error management
 - Log management
 - Variable management
 - Compatibility with IronPython and CPython
 - Simplification of complex API syntax using data objects while
   maintaining PEP8 compliance.
 - Code reusability across different solvers
@@ -268,17 +274,17 @@
 
 Example workflow
 -----------------
 1. Initialize the ``Desktop`` class with the version of AEDT to use.
 2. Initialize the application to use within AEDT.
 
 
-Connect to AEDT from Python IDE
--------------------------------
-PyAEDT works both inside AEDT and as a standalone application.
+Connect to AEDT from a Python IDE
+---------------------------------
+PyAEDT works both inside AEDT and as a standalone app.
 This Python library automatically detects whether it is running
 in an IronPython or CPython environment and initializes AEDT accordingly.
 PyAEDT also provides advanced error management. Usage examples follow.
 
 Explicit AEDT declaration and error management
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
@@ -316,15 +322,15 @@
 
 
 Remote application call
 ~~~~~~~~~~~~~~~~~~~~~~~
 You can make a remote application call on a CPython server
 or any Windows client machine.
 
-On a CPython Server:
+On a CPython server:
 
 .. code:: python
 
     # Launch PyAEDT remote server on CPython
 
     from pyaedt.common_rpc import pyaedt_service_manager
     pyaedt_service_manager()
@@ -369,10 +375,10 @@
 
 This module makes no commercial claim over Ansys whatsoever.
 PyAEDT extends the functionality of AEDT by adding
 an additional Python interface to AEDT without changing the core
 behavior or license of the original software. The use of the
 interactive control of PyAEDT requires a legally licensed
 local copy of AEDT. For more information about AEDT, 
-visit the `AEDT page <https://www.ansys.com/products/electronics>`_ 
-on the Ansys website.
+see the `Ansys Electronics <https://www.ansys.com/products/electronics>`_ 
+page on the Ansys website.
```

