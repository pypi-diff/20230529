# Comparing `tmp/pyaedt-0.6.77.tar.gz` & `tmp/pyaedt-0.6.78.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.6.77.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.6.78.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.6.77.tar` & `pyaedt-0.6.78.tar`

### file list

```diff
@@ -1,252 +1,252 @@
--rw-r--r--   0        0        0     1111 2023-05-18 13:27:42.185924 pyaedt-0.6.77/LICENSE
--rw-r--r--   0        0        0     9947 2023-05-18 13:27:42.185924 pyaedt-0.6.77/README.md
--rw-r--r--   0        0        0     2687 2023-05-26 13:07:30.590320 pyaedt-0.6.77/pyaedt/__init__.py
--rw-r--r--   0        0        0    26683 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6965 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    88296 2023-05-26 11:47:35.471641 pyaedt-0.6.77/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    41313 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    17062 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3088 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    19848 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4427 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4592 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   128774 2023-05-26 06:18:30.528988 pyaedt-0.6.77/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6115 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    75522 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    12462 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    36747 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    62954 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/circuit.py
--rw-r--r--   0        0        0    10034 2023-05-18 13:27:43.889057 pyaedt-0.6.77/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    64532 2023-05-26 11:47:35.471641 pyaedt-0.6.77/pyaedt/desktop.py
--rw-r--r--   0        0        0    15104 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.deps.json
--rw-r--r--   0        0        0    23552 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.dll
--rw-r--r--   0        0        0     1092 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysTemplate.json
--rw-r--r--   0        0        0   204800 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
--rw-r--r--   0        0        0   577445 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
--rw-r--r--   0        0        0     9836 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Images/Ansys.png
--rw-r--r--   0        0        0   238592 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
--rw-r--r--   0        0        0   115712 2023-05-18 13:27:43.904685 pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
--rw-r--r--   0        0        0   705296 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
--rw-r--r--   0        0        0   712253 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
--rw-r--r--   0        0        0    80384 2023-05-18 13:27:43.920373 pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
--rw-r--r--   0        0        0   546816 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.dll
--rw-r--r--   0        0        0   367616 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
--rw-r--r--   0        0        0   536367 2023-05-18 13:27:43.935986 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
--rw-r--r--   0        0        0  1229824 2023-05-18 13:27:43.951639 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
--rw-r--r--   0        0        0  3285773 2023-05-18 13:27:43.967239 pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
--rw-r--r--   0        0        0   120664 2023-05-18 13:27:43.967239 pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.dll
--rw-r--r--   0        0        0  1505294 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.xml
--rw-r--r--   0        0        0     5632 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
--rw-r--r--   0        0        0   160754 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
--rw-r--r--   0        0        0    23386 2023-05-25 14:36:21.414077 pyaedt-0.6.77/pyaedt/downloads.py
--rw-r--r--   0        0        0   143745 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/edb.py
--rw-r--r--   0        0        0      333 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/__init__.py
--rw-r--r--   0        0        0    92784 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/components.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/__init__.py
--rw-r--r--   0        0        0    32909 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/components_data.py
--rw-r--r--   0        0        0    40096 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/control_file.py
--rw-r--r--   0        0        0      937 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/design_options.py
--rw-r--r--   0        0        0      324 2023-05-18 13:27:43.982863 pyaedt-0.6.77/pyaedt/edb_core/edb_data/edb_builder.py
--rw-r--r--   0        0        0      867 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/edbvalue.py
--rw-r--r--   0        0        0    12194 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_extent_info.py
--rw-r--r--   0        0        0    65633 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
--rw-r--r--   0        0        0    20334 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/layer_data.py
--rw-r--r--   0        0        0     4777 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/nets_data.py
--rw-r--r--   0        0        0    61164 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/padstacks_data.py
--rw-r--r--   0        0        0    32351 2023-05-26 06:18:30.544561 pyaedt-0.6.77/pyaedt/edb_core/edb_data/primitives_data.py
--rw-r--r--   0        0        0    99879 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/simulation_configuration.py
--rw-r--r--   0        0        0    36335 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
--rw-r--r--   0        0        0    33757 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/edb_data/sources.py
--rw-r--r--   0        0        0     4147 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/edb_data/utilities.py
--rw-r--r--   0        0        0     2425 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/edb_data/variables.py
--rw-r--r--   0        0        0     3258 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/general.py
--rw-r--r--   0        0        0    66636 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/hfss.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/__init__.py
--rw-r--r--   0        0        0      673 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom.py
--rw-r--r--   0        0        0     1283 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom_item.py
--rw-r--r--   0        0        0     2213 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/characteristics.py
--rw-r--r--   0        0        0      524 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/refdes.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/__init__.py
--rw-r--r--   0        0        0      768 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/color.py
--rw-r--r--   0        0        0     2118 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/content.py
--rw-r--r--   0        0        0      938 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_color.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
--rw-r--r--   0        0        0     1029 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_line.py
--rw-r--r--   0        0        0      416 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_color.py
--rw-r--r--   0        0        0      548 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_line.py
--rw-r--r--   0        0        0      523 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/fill.py
--rw-r--r--   0        0        0      284 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/layer_ref.py
--rw-r--r--   0        0        0     2844 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
--rw-r--r--   0        0        0     1183 2023-05-18 13:27:43.998437 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
--rw-r--r--   0        0        0     1319 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
--rw-r--r--   0        0        0     1516 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
--rw-r--r--   0        0        0      960 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
--rw-r--r--   0        0        0     1964 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
--rw-r--r--   0        0        0     1158 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
--rw-r--r--   0        0        0     7759 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
--rw-r--r--   0        0        0      921 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
--rw-r--r--   0        0        0     1079 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
--rw-r--r--   0        0        0     4699 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
--rw-r--r--   0        0        0     1440 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
--rw-r--r--   0        0        0      875 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
--rw-r--r--   0        0        0     2775 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
--rw-r--r--   0        0        0      887 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
--rw-r--r--   0        0        0     4104 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
--rw-r--r--   0        0        0     2567 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
--rw-r--r--   0        0        0     1002 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
--rw-r--r--   0        0        0     8010 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
--rw-r--r--   0        0        0      663 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
--rw-r--r--   0        0        0     1162 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
--rw-r--r--   0        0        0     1626 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
--rw-r--r--   0        0        0      838 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
--rw-r--r--   0        0        0    11386 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
--rw-r--r--   0        0        0     1033 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_header.py
--rw-r--r--   0        0        0      683 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/ecad.py
--rw-r--r--   0        0        0     2008 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/spec.py
--rw-r--r--   0        0        0     1624 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/history_record.py
--rw-r--r--   0        0        0    21750 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ipc2581.py
--rw-r--r--   0        0        0      966 2023-05-18 13:27:44.014060 pyaedt-0.6.77/pyaedt/edb_core/ipc2581/logistic_header.py
--rw-r--r--   0        0        0    49117 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/layout.py
--rw-r--r--   0        0        0    33295 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/materials.py
--rw-r--r--   0        0        0    43733 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/nets.py
--rw-r--r--   0        0        0    46664 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/padstack.py
--rw-r--r--   0        0        0    57186 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/siwave.py
--rw-r--r--   0        0        0   109024 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/edb_core/stackup.py
--rw-r--r--   0        0        0    11359 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/emit.py
--rw-r--r--   0        0        0     3555 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3291 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/EmitConstants.py
--rw-r--r--   0        0        0     1091 2023-05-19 17:43:56.955082 pyaedt-0.6.77/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0        2 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-05-19 05:07:06.470308 pyaedt-0.6.77/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    12244 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0    14317 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    11758 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     3257 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0    83440 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28645 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    21891 2023-05-26 06:18:30.560187 pyaedt-0.6.77/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0     3395 2023-05-19 12:41:50.180833 pyaedt-0.6.77/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    70263 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0    25808 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     6989 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0     9795 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    62325 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    11301 2023-05-18 13:27:44.029696 pyaedt-0.6.77/pyaedt/generic/process.py
--rw-r--r--   0        0        0    20326 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3466 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    60408 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/generic/toolkit.py
--rw-r--r--   0        0        0    17095 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0      438 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/generic/wpf_template.xaml
--rw-r--r--   0        0        0   252844 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/hfss.py
--rw-r--r--   0        0        0    82916 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   168413 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/icepak.py
--rw-r--r--   0        0        0   118475 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7803 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24312 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3035 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     3695 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     2380 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0       53 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10210 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     3731 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-05-18 13:27:44.045311 pyaedt-0.6.77/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     3818 2023-05-19 06:53:58.810568 pyaedt-0.6.77/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0      678 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      953 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0      868 2023-05-18 13:27:44.060935 pyaedt-0.6.77/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14105 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20047 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16838 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   120884 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0   194589 2023-05-26 06:18:30.575810 pyaedt-0.6.77/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   116603 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    11385 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   127894 2023-05-24 13:32:35.806883 pyaedt-0.6.77/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.076561 pyaedt-0.6.77/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    31587 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49055 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59074 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53129 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12641 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    42625 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    32776 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8210 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    63096 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15147 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    32011 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68135 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6950 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    52598 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    31323 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    49890 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    65637 2023-05-26 06:18:30.591447 pyaedt-0.6.77/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23685 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    30094 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   114711 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71549 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-05-18 13:27:44.092187 pyaedt-0.6.77/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    51963 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40461 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0    82899 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    28359 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    53222 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    11972 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    26101 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   173003 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    64104 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   119428 2023-05-26 11:30:35.579837 pyaedt-0.6.77/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    33255 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    28705 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   103329 2023-05-26 06:18:30.607060 pyaedt-0.6.77/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   125077 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    95904 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/q3d.py
--rw-r--r--   0        0        0    10577 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    40721 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9425 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-05-18 13:27:44.107810 pyaedt-0.6.77/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7630 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    10426 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyaedt/siwave.py
--rw-r--r--   0        0        0    10527 2023-05-18 13:27:44.123438 pyaedt-0.6.77/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     4134 2023-05-26 06:18:30.622693 pyaedt-0.6.77/pyproject.toml
--rw-r--r--   0        0        0    15129 1970-01-01 00:00:00.000000 pyaedt-0.6.77/PKG-INFO
+-rw-r--r--   0        0        0     1111 2023-05-16 06:59:23.102429 pyaedt-0.6.78/LICENSE
+-rw-r--r--   0        0        0     9947 2023-05-16 06:59:23.102429 pyaedt-0.6.78/README.md
+-rw-r--r--   0        0        0     2691 2023-05-29 08:06:46.309364 pyaedt-0.6.78/pyaedt/__init__.py
+-rw-r--r--   0        0        0    26683 2023-05-24 15:53:22.079958 pyaedt-0.6.78/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6965 2023-05-16 06:59:25.180542 pyaedt-0.6.78/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    88300 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    41317 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    17066 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3088 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    19852 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4431 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4596 2023-05-29 06:50:09.584617 pyaedt-0.6.78/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   128778 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6115 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    75524 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    12464 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    36749 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    62954 2023-05-23 13:08:30.544249 pyaedt-0.6.78/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10034 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    64534 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/desktop.py
+-rw-r--r--   0        0        0    15104 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.deps.json
+-rw-r--r--   0        0        0    23552 2023-05-16 06:59:25.196166 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.dll
+-rw-r--r--   0        0        0     1092 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysTemplate.json
+-rw-r--r--   0        0        0   204800 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll
+-rw-r--r--   0        0        0   577445 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml
+-rw-r--r--   0        0        0     9836 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Images/Ansys.png
+-rw-r--r--   0        0        0   238592 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll
+-rw-r--r--   0        0        0   115712 2023-05-16 06:59:25.211792 pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll
+-rw-r--r--   0        0        0   705296 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll
+-rw-r--r--   0        0        0   712253 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml
+-rw-r--r--   0        0        0    80384 2023-05-16 06:59:25.227417 pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll
+-rw-r--r--   0        0        0   546816 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.dll
+-rw-r--r--   0        0        0   367616 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll
+-rw-r--r--   0        0        0   536367 2023-05-16 06:59:25.243041 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml
+-rw-r--r--   0        0        0  1229824 2023-05-16 06:59:25.258665 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll
+-rw-r--r--   0        0        0  3285773 2023-05-16 06:59:25.274293 pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml
+-rw-r--r--   0        0        0   120664 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.dll
+-rw-r--r--   0        0        0  1505294 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.xml
+-rw-r--r--   0        0        0     5632 2023-05-16 06:59:25.289918 pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll
+-rw-r--r--   0        0        0   160754 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml
+-rw-r--r--   0        0        0    23386 2023-05-25 10:01:32.202746 pyaedt-0.6.78/pyaedt/downloads.py
+-rw-r--r--   0        0        0   143749 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb.py
+-rw-r--r--   0        0        0      333 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/__init__.py
+-rw-r--r--   0        0        0    92788 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/components.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/__init__.py
+-rw-r--r--   0        0        0    32911 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/components_data.py
+-rw-r--r--   0        0        0    40100 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/control_file.py
+-rw-r--r--   0        0        0      937 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/design_options.py
+-rw-r--r--   0        0        0      324 2023-05-16 06:59:25.305543 pyaedt-0.6.78/pyaedt/edb_core/edb_data/edb_builder.py
+-rw-r--r--   0        0        0      867 2023-05-25 15:57:26.266409 pyaedt-0.6.78/pyaedt/edb_core/edb_data/edbvalue.py
+-rw-r--r--   0        0        0    12198 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_extent_info.py
+-rw-r--r--   0        0        0    65637 2023-05-29 06:50:09.600210 pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py
+-rw-r--r--   0        0        0    20336 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/layer_data.py
+-rw-r--r--   0        0        0     4781 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/nets_data.py
+-rw-r--r--   0        0        0    61168 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/padstacks_data.py
+-rw-r--r--   0        0        0    32355 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/primitives_data.py
+-rw-r--r--   0        0        0    99883 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/simulation_configuration.py
+-rw-r--r--   0        0        0    36339 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py
+-rw-r--r--   0        0        0    33759 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/edb_data/sources.py
+-rw-r--r--   0        0        0     4147 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/edb_data/utilities.py
+-rw-r--r--   0        0        0     2425 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/edb_data/variables.py
+-rw-r--r--   0        0        0     3258 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/general.py
+-rw-r--r--   0        0        0    66640 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/hfss.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/__init__.py
+-rw-r--r--   0        0        0      673 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom.py
+-rw-r--r--   0        0        0     1283 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom_item.py
+-rw-r--r--   0        0        0     2213 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/characteristics.py
+-rw-r--r--   0        0        0      524 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/refdes.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/__init__.py
+-rw-r--r--   0        0        0      768 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/color.py
+-rw-r--r--   0        0        0     2118 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/content.py
+-rw-r--r--   0        0        0      938 2023-05-16 06:59:25.321165 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_color.py
+-rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_fill.py
+-rw-r--r--   0        0        0     1029 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_line.py
+-rw-r--r--   0        0        0      416 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_color.py
+-rw-r--r--   0        0        0      548 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_line.py
+-rw-r--r--   0        0        0      523 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/fill.py
+-rw-r--r--   0        0        0      284 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/layer_ref.py
+-rw-r--r--   0        0        0     2844 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/__init__.py
+-rw-r--r--   0        0        0     1183 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py
+-rw-r--r--   0        0        0     1319 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py
+-rw-r--r--   0        0        0     1516 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py
+-rw-r--r--   0        0        0      960 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py
+-rw-r--r--   0        0        0     1964 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py
+-rw-r--r--   0        0        0     1158 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py
+-rw-r--r--   0        0        0     7763 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py
+-rw-r--r--   0        0        0      921 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py
+-rw-r--r--   0        0        0     1079 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py
+-rw-r--r--   0        0        0     4703 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py
+-rw-r--r--   0        0        0     1440 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py
+-rw-r--r--   0        0        0      875 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py
+-rw-r--r--   0        0        0     2775 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py
+-rw-r--r--   0        0        0      887 2023-05-16 06:59:25.336792 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py
+-rw-r--r--   0        0        0     4104 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py
+-rw-r--r--   0        0        0     2567 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py
+-rw-r--r--   0        0        0     1002 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py
+-rw-r--r--   0        0        0     8010 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py
+-rw-r--r--   0        0        0      663 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py
+-rw-r--r--   0        0        0     1162 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py
+-rw-r--r--   0        0        0     1626 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py
+-rw-r--r--   0        0        0      838 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py
+-rw-r--r--   0        0        0    11390 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py
+-rw-r--r--   0        0        0     1033 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_header.py
+-rw-r--r--   0        0        0      683 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/ecad.py
+-rw-r--r--   0        0        0     2008 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/spec.py
+-rw-r--r--   0        0        0     1624 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/history_record.py
+-rw-r--r--   0        0        0    21750 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ipc2581.py
+-rw-r--r--   0        0        0      966 2023-05-16 06:59:25.352417 pyaedt-0.6.78/pyaedt/edb_core/ipc2581/logistic_header.py
+-rw-r--r--   0        0        0    49121 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/layout.py
+-rw-r--r--   0        0        0    33299 2023-05-29 06:50:09.615842 pyaedt-0.6.78/pyaedt/edb_core/materials.py
+-rw-r--r--   0        0        0    43737 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/nets.py
+-rw-r--r--   0        0        0    46668 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/padstack.py
+-rw-r--r--   0        0        0    57190 2023-05-29 06:50:09.631460 pyaedt-0.6.78/pyaedt/edb_core/siwave.py
+-rw-r--r--   0        0        0   109028 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/edb_core/stackup.py
+-rw-r--r--   0        0        0    11363 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/emit.py
+-rw-r--r--   0        0        0     3555 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3291 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/EmitConstants.py
+-rw-r--r--   0        0        0     1091 2023-05-20 16:14:01.011451 pyaedt-0.6.78/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0        2 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-05-19 04:27:23.959058 pyaedt-0.6.78/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    12248 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0    14317 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    11758 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.368043 pyaedt-0.6.78/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     3257 2023-05-26 11:30:36.599404 pyaedt-0.6.78/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0    83444 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28645 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    21891 2023-05-24 15:53:22.126810 pyaedt-0.6.78/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0     3395 2023-05-19 12:41:48.802021 pyaedt-0.6.78/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    69591 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0    25808 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     6989 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0     9795 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    62327 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    11301 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/process.py
+-rw-r--r--   0        0        0    20326 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3466 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    60412 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/generic/toolkit.py
+-rw-r--r--   0        0        0    17095 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0      438 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/generic/wpf_template.xaml
+-rw-r--r--   0        0        0   252848 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/hfss.py
+-rw-r--r--   0        0        0    82916 2023-05-16 06:59:25.383677 pyaedt-0.6.78/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   168417 2023-05-29 06:50:09.647120 pyaedt-0.6.78/pyaedt/icepak.py
+-rw-r--r--   0        0        0   118479 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7803 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24316 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3035 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     3695 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     2380 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0       53 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10210 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     3731 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     3818 2023-05-19 12:41:48.802021 pyaedt-0.6.78/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-05-16 06:59:25.399290 pyaedt-0.6.78/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0      678 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      953 2023-05-16 06:59:25.414915 pyaedt-0.6.78/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0      868 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14107 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20051 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16840 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   120888 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0   194593 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   116607 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    11387 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   127894 2023-05-24 13:33:05.690067 pyaedt-0.6.78/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.430540 pyaedt-0.6.78/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    31589 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49057 2023-05-29 06:50:09.662736 pyaedt-0.6.78/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    59078 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    53131 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12645 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    42629 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    32780 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8212 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    63100 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15149 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.78/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    32013 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68135 2023-05-19 10:14:06.395089 pyaedt-0.6.78/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6952 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    52600 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    31327 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    49892 2023-05-29 06:50:09.678333 pyaedt-0.6.78/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.446165 pyaedt-0.6.78/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    65639 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23689 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    30094 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   114715 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71549 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    51967 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40465 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0    82903 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    28363 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    53226 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    11976 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    26105 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-05-16 06:59:25.461791 pyaedt-0.6.78/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   173007 2023-05-29 06:50:09.693947 pyaedt-0.6.78/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    64104 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   119432 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    33257 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    28709 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   103333 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   125079 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    95908 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10581 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    40721 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9425 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-05-16 06:59:25.477419 pyaedt-0.6.78/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7632 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    10430 2023-05-29 06:50:09.709572 pyaedt-0.6.78/pyaedt/siwave.py
+-rw-r--r--   0        0        0    10527 2023-05-16 06:59:25.493150 pyaedt-0.6.78/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     4426 2023-05-29 07:58:53.347931 pyaedt-0.6.78/pyproject.toml
+-rw-r--r--   0        0        0    15568 1970-01-01 00:00:00.000000 pyaedt-0.6.78/PKG-INFO
```

### Comparing `pyaedt-0.6.77/LICENSE` & `pyaedt-0.6.78/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/README.md` & `pyaedt-0.6.78/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/__init__.py` & `pyaedt-0.6.78/pyaedt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,32 +8,33 @@
 os.environ["ANSYSEM_FEATURE_SF159726_SCRIPTOBJECT_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_SF222134_CABLE_MODELING_ENHANCEMENTS_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_F395486_RIGID_FLEX_BENDING_ENABLE"] = "1"
 os.environ["ANSYSEM_FEATURE_S432616_LAYOUT_COMPONENT_IN_3D_ENABLE"] = "1"
 
 pyaedt_path = os.path.dirname(__file__)
 
-__version__ = "0.6.77"
+__version__ = "0.6.78"
 
 version = __version__
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
 import pyaedt.generic.general_methods as general_methods
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_folder_name
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import generate_unique_project_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import online_help
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 
 from pyaedt.aedt_logger import pyaedt_logger  # isort:skip
 
 try:
     from pyaedt.generic.design_types import Hfss3dLayout
```

### Comparing `pyaedt-0.6.77/pyaedt/aedt_logger.py` & `pyaedt-0.6.78/pyaedt/aedt_logger.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.6.78/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/application/Analysis.py` & `pyaedt-0.6.78/pyaedt/application/Analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AXIS
 from pyaedt.generic.constants import GRAVITY
 from pyaedt.generic.constants import PLANE
 from pyaedt.generic.constants import SETUPS
 from pyaedt.generic.constants import SOLUTIONS
 from pyaedt.generic.constants import VIEW
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import filter_tuple
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import MaxwellParameters
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.DesignXPloration import OptimizationSetups
 from pyaedt.modules.DesignXPloration import ParametricSetups
 from pyaedt.modules.SolveSetup import Setup
 from pyaedt.modules.SolveSetup import SetupHFSS
```

### Comparing `pyaedt-0.6.77/pyaedt/application/Analysis3D.py` & `pyaedt-0.6.78/pyaedt/application/Analysis3D.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import ntpath
 import os
 import warnings
 
 from pyaedt import settings
 from pyaedt.application.Analysis import Analysis
 from pyaedt.generic.configurations import Configurations
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class FieldAnalysis3D(Analysis, object):
     """Manages 3D field analysis setup in HFSS, Maxwell 3D, and Q3D.
 
     This class is automatically initialized by an application call from one of
```

### Comparing `pyaedt-0.6.77/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.6.78/pyaedt/application/Analysis3DLayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 
 from pyaedt.application.Analysis import Analysis
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSetup import Setup3DLayout
 
 
 class FieldAnalysis3DLayout(Analysis):
     """Manages 3D field analysis setup in HFSS 3D Layout.
```

### Comparing `pyaedt-0.6.77/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.6.78/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.6.78/pyaedt/application/AnalysisNexxim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyaedt.application.Analysis import Analysis
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modules.Boundary import CurrentSinSource
 from pyaedt.modules.Boundary import Excitations
 from pyaedt.modules.Boundary import PowerIQSource
 from pyaedt.modules.Boundary import PowerSinSource
 from pyaedt.modules.Boundary import Sources
```

### Comparing `pyaedt-0.6.77/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.6.78/pyaedt/application/AnalysisRMxprt.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyaedt.application.Analysis import Analysis
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class FieldAnalysisRMxprt(Analysis):
     """Manages RMXprt field analysis setup. (To be implemented.)
 
     This class is automatically initialized by an application call (like HFSS,
```

### Comparing `pyaedt-0.6.77/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.6.78/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from pyaedt.application.Analysis import Analysis
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSetup import SetupCircuit
 
 
 class AnalysisTwinBuilder(Analysis):
     """Provides the Twin Builder Analysis Setup (TwinBuilder).
```

### Comparing `pyaedt-0.6.77/pyaedt/application/Design.py` & `pyaedt-0.6.78/pyaedt/application/Design.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,22 +37,23 @@
 from pyaedt.desktop import exception_to_desktop
 from pyaedt.desktop import get_version_env_variable
 from pyaedt.desktop import release_desktop
 from pyaedt.generic.DataHandlers import variation_string_to_dict
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import unit_system
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_project_locked
 from pyaedt.generic.general_methods import is_windows
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import read_csv
 from pyaedt.generic.general_methods import read_tab
 from pyaedt.generic.general_methods import read_xlsx
 from pyaedt.generic.general_methods import settings
 from pyaedt.generic.general_methods import write_csv
 from pyaedt.modules.Boundary import BoundaryObject
```

### Comparing `pyaedt-0.6.77/pyaedt/application/JobManager.py` & `pyaedt-0.6.78/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/application/Variables.py` & `pyaedt-0.6.78/pyaedt/application/Variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 from __future__ import absolute_import  # noreorder
 from __future__ import division
 
 import os
 import re
 import types
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import _resolve_unit_system
 from pyaedt.generic.constants import unit_system
 from pyaedt.generic.general_methods import is_array
 from pyaedt.generic.general_methods import is_number
```

### Comparing `pyaedt-0.6.77/pyaedt/application/aedt_objects.py` & `pyaedt-0.6.78/pyaedt/application/aedt_objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 
 
 class AedtObjects(object):
     def __init__(self, project=None, design=None, is_inherithed=False):
         self._odesktop = sys.modules["__main__"].oDesktop
         if not is_inherithed:
```

### Comparing `pyaedt-0.6.77/pyaedt/application/design_solutions.py` & `pyaedt-0.6.78/pyaedt/application/design_solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import copy
 
-from pyaedt.generic.general_methods import property
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 solutions_defaults = {
     "Maxwell 2D": "Magnetostatic",
     "Maxwell 3D": "Magnetostatic",
     "Twin Builder": "TR",
     "Circuit Design": "NexximLNA",
```

### Comparing `pyaedt-0.6.77/pyaedt/circuit.py` & `pyaedt-0.6.78/pyaedt/circuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/common_rpc.py` & `pyaedt-0.6.78/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/desktop.py` & `pyaedt-0.6.78/pyaedt/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,16 +31,16 @@
     os.environ["ANS_NODEPCHECK"] = str(1)
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
 
+# from pyaedt import property
 from pyaedt import __version__
-from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import active_sessions
 from pyaedt.generic.general_methods import com_active_sessions
 from pyaedt.generic.general_methods import grpc_active_sessions
 from pyaedt.generic.general_methods import inside_desktop
```

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.deps.json` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.deps.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysReport.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysReport.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/AnsysTemplate.json` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/ICSharpCode.SharpZipLib.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Images/Ansys.png` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Images/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.DocumentObjectModel.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/MigraDocCore.Rendering.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/Newtonsoft.Json.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.Charting.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/PdfSharpCore.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/PdfSharpCore.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.Fonts.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/SixLabors.ImageSharp.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/System.Runtime.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/System.Runtime.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/PdfSharpCore.resources.dll`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml` & `pyaedt-0.6.78/pyaedt/dlls/PDFReport/de/System.Collections.NonGeneric.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/downloads.py` & `pyaedt-0.6.78/pyaedt/downloads.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb.py` & `pyaedt-0.6.78/pyaedt/edb.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,23 +46,24 @@
 from pyaedt.generic.clr_module import Convert
 from pyaedt.generic.clr_module import List
 from pyaedt.generic.clr_module import Tuple
 from pyaedt.generic.clr_module import _clr
 from pyaedt.generic.clr_module import edb_initialized
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SolverType
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import env_path
 from pyaedt.generic.general_methods import env_path_student
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
 from pyaedt.generic.general_methods import is_windows
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.process import SiwaveSolve
 from pyaedt.misc.misc import list_installed_ansysem
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/components.py` & `pyaedt-0.6.78/pyaedt/edb_core/components.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.sources import Source
 from pyaedt.edb_core.edb_data.sources import SourceType
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.padstack import EdbPadstacks
 from pyaedt.generic.clr_module import String
 from pyaedt.generic.clr_module import _clr
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import get_filename_without_extension
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 def resistor_value_parser(RValue):
     """Convert a resistor value.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/components_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/components_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,16 +9,16 @@
     try:
         import numpy as np
     except ImportError:
         warnings.warn(
             "The NumPy module is required to run some functionalities of EDB.\n"
             "Install with \n\npip install numpy\n\nRequires CPython."
         )
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import get_filename_without_extension
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EDBComponentDef(object):
     """Manages EDB functionalities for component definitions.
 
     Parameters
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/control_file.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/control_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import copy
 import os
 import re
 import sys
 
 from pyaedt import pyaedt_logger
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import env_path
 from pyaedt.generic.general_methods import env_value
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_linux
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc import list_installed_ansysem
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/design_options.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/design_options.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/edbvalue.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/edbvalue.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_extent_info.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_extent_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class HfssExtentInfo:
     """Manages EDB functionalities for HFSS extent information.
 
     Parameters
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/hfss_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Tuple
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbFrequencySweep(object):
     """Manages EDB methods for frequency sweep."""
 
     def __init__(self, sim_setup, frequency_sweep=None, name=None, edb_sweep_data=None):
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/layer_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/layer_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import absolute_import
 
 import re
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 
 
 class LayerEdbClass(object):
     """Manages Edb Layers. Replaces EDBLayer."""
 
     def __init__(self, pclass, name):
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/nets_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/nets_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EDBNetsData(object):
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/padstacks_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/padstacks_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 from pyaedt import is_ironpython
 from pyaedt.edb_core.edb_data.edbvalue import EdbValue
 from pyaedt.edb_core.general import PadGeometryTpe
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import String
 from pyaedt.generic.clr_module import _clr
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EDBPadProperties(object):
     """Manages EDB functionalities for pad properties.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/primitives_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/primitives_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import math
 
 from pyaedt.edb_core.general import convert_py_list_to_net_list
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EDBPrimitives(object):
     """Manages EDB functionalities for a primitives.
     It Inherits EDB Object properties.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/simulation_configuration.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/simulation_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from pyaedt.generic.clr_module import Dictionary
 from pyaedt.generic.constants import BasisOrder
 from pyaedt.generic.constants import CutoutSubdesignType
 from pyaedt.generic.constants import RadiationBoxType
 from pyaedt.generic.constants import SolverType
 from pyaedt.generic.constants import SweepType
 from pyaedt.generic.constants import validate_enum_class_value
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class SimulationConfigurationBatch(object):
     """Contains all Cutout and Batch analysis settings.
     The class is part of `SimulationConfiguration` class as a property.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/siwave_simulation_setup_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pyaedt.edb_core.edb_data.hfss_simulation_setup_data import EdbFrequencySweep
 from pyaedt.edb_core.general import convert_netdict_to_pydict
 from pyaedt.edb_core.general import convert_pydict_to_netdict
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_linux
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class SiwaveAdvancedSettings(object):
     def __init__(self, parent):
         self._parent = parent
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/sources.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.edb_core.edb_data.nets_data import EDBNetsData
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.generic.constants import NodeType
 from pyaedt.generic.constants import SourceType
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/utilities.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/utilities.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/edb_data/variables.py` & `pyaedt-0.6.78/pyaedt/edb_core/edb_data/variables.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/general.py` & `pyaedt-0.6.78/pyaedt/edb_core/general.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/hfss.py` & `pyaedt-0.6.78/pyaedt/edb_core/hfss.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 from pyaedt.edb_core.edb_data.simulation_configuration import SimulationConfiguration
 from pyaedt.edb_core.edb_data.sources import ExcitationBundle
 from pyaedt.edb_core.edb_data.sources import ExcitationDifferential
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.edb_core.general import convert_pytuple_to_nettuple
 from pyaedt.generic.constants import RadiationBoxType
 from pyaedt.generic.constants import SweepType
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbHfss(object):
     """Manages EDB method to configure Hfss setup accessible from `Edb.hfss` property.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/bom_item.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/bom_item.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/characteristics.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/characteristics.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/bom/refdes.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/bom/refdes.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/color.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/content.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/content.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_color.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_color.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_fill.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/dictionary_line.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/dictionary_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/entry_line.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/entry_line.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/fill.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/fill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/content/standard_geometries_dictionary.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/assembly_drawing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/cad_data.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/component.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/drill.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/feature.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/layer_feature.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 
 from pyaedt.edb_core.ipc2581.ecad.cad_data.feature import Feature
 from pyaedt.edb_core.ipc2581.ecad.cad_data.feature import FeatureType
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class LayerFeature(object):
     """Class describing IPC2581 layer feature."""
 
     def __init__(self, ipc):
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/logical_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/outline.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/package.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import math
 
 from pyaedt.edb_core.ipc2581.content.entry_line import EntryLine
 from pyaedt.edb_core.ipc2581.ecad.cad_data.assembly_drawing import AssemblyDrawing
 from pyaedt.edb_core.ipc2581.ecad.cad_data.outline import Outline
 from pyaedt.edb_core.ipc2581.ecad.cad_data.pin import Pin
 from pyaedt.edb_core.ipc2581.ecad.cad_data.polygon import PolyStep
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Package(object):
     """Class describing an IPC2581 package definition."""
 
     def __init__(self, ipc):
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_hole_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_instance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/padstack_pad_def.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/path.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/phy_net.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/pin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/polygon.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/profile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_group.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/stackup_layer.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_data/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 from pyaedt.edb_core.ipc2581.ecad.cad_data.component import Component
 from pyaedt.edb_core.ipc2581.ecad.cad_data.layer_feature import LayerFeature
 from pyaedt.edb_core.ipc2581.ecad.cad_data.logical_net import LogicalNet
 from pyaedt.edb_core.ipc2581.ecad.cad_data.package import Package
 from pyaedt.edb_core.ipc2581.ecad.cad_data.padstack_def import PadstackDef
 from pyaedt.edb_core.ipc2581.ecad.cad_data.phy_net import PhyNet
 from pyaedt.edb_core.ipc2581.ecad.cad_data.profile import Profile
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Step(object):
     def __init__(self, caddata, edb, units, ipc):
         self.design_name = caddata.design_name
         self._pedb = edb
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/cad_header.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/cad_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/ecad.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/ecad.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ecad/spec.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ecad/spec.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/history_record.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/history_record.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/ipc2581.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/ipc2581.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/ipc2581/logistic_header.py` & `pyaedt-0.6.78/pyaedt/edb_core/ipc2581/logistic_header.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/layout.py` & `pyaedt-0.6.78/pyaedt/edb_core/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 import math
 import warnings
 
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.edb_data.utilities import EDBStatistics
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Tuple
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbLayout(object):
     """Manages EDB methods for primitives management accessible from `Edb.modeler` property.
 
     Examples
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/materials.py` & `pyaedt-0.6.78/pyaedt/edb_core/materials.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import difflib
 import logging
 import warnings
 
 from pyaedt import is_ironpython
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import _clr
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 logger = logging.getLogger(__name__)
 
 
 class Material(object):
     """Manages EDB methods for material property management."""
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/nets.py` & `pyaedt-0.6.78/pyaedt/edb_core/nets.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 import warnings
 
 from pyaedt.edb_core.edb_data.nets_data import EDBNetsData
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.edb_data.primitives_data import EDBPrimitives
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.constants import CSS4_COLORS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbNets(object):
     """Manages EDB methods for nets management accessible from `Edb.nets` property.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/padstack.py` & `pyaedt-0.6.78/pyaedt/edb_core/padstack.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 import math
 import warnings
 
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstack
 from pyaedt.edb_core.edb_data.padstacks_data import EDBPadstackInstance
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.clr_module import Array
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EdbPadstacks(object):
     """Manages EDB methods for nets management accessible from `Edb.padstacks` property.
 
     Examples
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/siwave.py` & `pyaedt-0.6.78/pyaedt/edb_core/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,18 @@
 from pyaedt.edb_core.edb_data.sources import DCTerminal
 from pyaedt.edb_core.edb_data.sources import PinGroup
 from pyaedt.edb_core.edb_data.sources import ResistorSource
 from pyaedt.edb_core.edb_data.sources import VoltageSource
 from pyaedt.edb_core.general import convert_py_list_to_net_list
 from pyaedt.generic.constants import SolverType
 from pyaedt.generic.constants import SweepType
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class EdbSiwave(object):
     """Manages EDB methods related to Siwave Setup accessible from `Edb.siwave` property.
```

### Comparing `pyaedt-0.6.77/pyaedt/edb_core/stackup.py` & `pyaedt-0.6.78/pyaedt/edb_core/stackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,18 @@
 import math
 import os.path
 import warnings
 
 from pyaedt import generate_unique_name
 from pyaedt.edb_core.edb_data.layer_data import LayerEdbClass
 from pyaedt.edb_core.general import convert_py_list_to_net_list
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import ET
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc.aedtlib_personalib_install import write_pretty_xml
 
 pd = None
 np = None
 if not is_ironpython:
     try:
```

### Comparing `pyaedt-0.6.77/pyaedt/emit.py` & `pyaedt-0.6.78/pyaedt/emit.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 
 from pyaedt import emit_core
 from pyaedt import generate_unique_project_name
 from pyaedt.application.Design import Design
 from pyaedt.emit_core import EmitConstants
 from pyaedt.emit_core.Couplings import CouplingsEmit
 from pyaedt.emit_core.results.results import Results
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.schematic import ModelerEmit
 
 
 class Emit(Design, object):
     """Provides the Emit application interface.
```

### Comparing `pyaedt-0.6.77/pyaedt/emit_core/Couplings.py` & `pyaedt-0.6.78/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/emit_core/EmitConstants.py` & `pyaedt-0.6.78/pyaedt/emit_core/EmitConstants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/emit_core/__init__.py` & `pyaedt-0.6.78/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/emit_core/results/results.py` & `pyaedt-0.6.78/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/emit_core/results/revision.py` & `pyaedt-0.6.78/pyaedt/emit_core/results/revision.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 
 import pyaedt.emit_core.EmitConstants as emitConsts
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Revision:
     """
     Provides the ``Revision`` object.
```

### Comparing `pyaedt-0.6.77/pyaedt/generic/DataHandlers.py` & `pyaedt-0.6.78/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.6.78/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/clr_module.py` & `pyaedt-0.6.78/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/configurations.py` & `pyaedt-0.6.78/pyaedt/generic/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 from pyaedt import Icepak
 from pyaedt import __version__
 from pyaedt import generate_unique_folder_name
 from pyaedt import get_pyaedt_app
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _create_json_file
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import CoordinateSystem
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import BoundaryProps
 from pyaedt.modules.Boundary import NativeComponentObject
```

### Comparing `pyaedt-0.6.77/pyaedt/generic/constants.py` & `pyaedt-0.6.78/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/design_types.py` & `pyaedt-0.6.78/pyaedt/generic/design_types.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/filesystem.py` & `pyaedt-0.6.78/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/general_methods.py` & `pyaedt-0.6.78/pyaedt/generic/general_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -1714,52 +1714,30 @@
 
     def developer_forum(self):
         """Open the Discussions page on the Ansys Developer site."""
         url = "https://developer.ansys.com/"
         self._launch_ur(url)
 
 
-class Property(property):
-    @pyaedt_function_handler()
-    def __get__(self, obj, *args, **kwargs):
-        """Get value."""
-        # if obj is None:
-        #     return self
-        if self.fget is None:
-            raise AttributeError("unreadable attribute")
-        return self.fget(obj)
-
-    @pyaedt_function_handler()
-    def __set__(self, obj, value):
-        """Set value."""
-        if self.fset is None:
-            raise AttributeError("can't set attribute")
-        self.fset(obj, value)
-
-    @pyaedt_function_handler()
-    def __delete__(self, obj):
-        """Delete value."""
-        if self.fdel is None:
-            raise AttributeError("can't delete attribute")
-        self.fdel(obj)
-
-    @pyaedt_function_handler()
-    def getter(self, fget):
-        """Property getter."""
-        return self.__class__.__base__(fget, self.fset, self.fdel, self.__doc__)
-
-    @pyaedt_function_handler()
-    def setter(self, fset):
-        """Property setter."""
-        return self.__class__.__base__(self.fget, fset, self.fdel, self.__doc__)
-
-    @pyaedt_function_handler()
-    def deleter(self, fdel):
-        """Property deleter."""
-        return self.__class__.__base__(self.fget, self.fset, fdel, self.__doc__)
+# class Property(property):
+#
+#     @pyaedt_function_handler()
+#     def getter(self, fget):
+#         """Property getter."""
+#         return self.__class__.__base__(fget, self.fset, self.fdel, self.__doc__)
+#
+#     @pyaedt_function_handler()
+#     def setter(self, fset):
+#         """Property setter."""
+#         return self.__class__.__base__(self.fget, fset, self.fdel, self.__doc__)
+#
+#     @pyaedt_function_handler()
+#     def deleter(self, fdel):
+#         """Property deleter."""
+#         return self.__class__.__base__(self.fget, self.fset, fdel, self.__doc__)
 
 
 class Settings(object):
     """Manages all PyAEDT environment variables and global settings."""
 
     def __init__(self):
         self._enable_logger = True
@@ -2232,10 +2210,10 @@
         return self._enable_debug_logger
 
     @enable_debug_logger.setter
     def enable_debug_logger(self, val):
         self._enable_debug_logger = val
 
 
-property = Property
+# property = Property
 settings = Settings()
 online_help = Help()
```

### Comparing `pyaedt-0.6.77/pyaedt/generic/ibis_reader.py` & `pyaedt-0.6.78/pyaedt/generic/ibis_reader.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/near_field_import.py` & `pyaedt-0.6.78/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/pdf.py` & `pyaedt-0.6.78/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/plot.py` & `pyaedt-0.6.78/pyaedt/generic/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from datetime import datetime
 import math
 import os
 import tempfile
 import time
 import warnings
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import CSS4_COLORS
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.77/pyaedt/generic/process.py` & `pyaedt-0.6.78/pyaedt/generic/process.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/python_optimizers.py` & `pyaedt-0.6.78/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/report_file_parser.py` & `pyaedt-0.6.78/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/generic/toolkit.py` & `pyaedt-0.6.78/pyaedt/generic/toolkit.py`

 * *Files 0% similar despite different names*

```diff
@@ -78,15 +78,16 @@
 
 from pyaedt import is_ironpython
 from pyaedt import is_linux
 from pyaedt import is_windows
 from pyaedt.desktop import Desktop
 import pyaedt.edb_core.edb_data.simulation_configuration
 from pyaedt.generic.clr_module import _clr
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 if is_linux and is_ironpython:
     import subprocessdotnet as subprocess
 else:
     import subprocess
```

### Comparing `pyaedt-0.6.77/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.6.78/pyaedt/generic/touchstone_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/hfss.py` & `pyaedt-0.6.78/pyaedt/hfss.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,18 +10,19 @@
 import warnings
 
 from pyaedt import settings
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.constants import INFINITE_SPHERE_TYPE
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
 from pyaedt.generic.general_methods import parse_excitation_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import FarFieldSetup
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.Boundary import NearFieldSetup
```

### Comparing `pyaedt-0.6.77/pyaedt/hfss3dlayout.py` & `pyaedt-0.6.78/pyaedt/hfss3dlayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/icepak.py` & `pyaedt-0.6.78/pyaedt/icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 
 import re
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.configurations import ConfigurationsIcepak
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import NativeComponentObject
 from pyaedt.modules.monitor_icepak import Monitor
```

### Comparing `pyaedt-0.6.77/pyaedt/maxwell.py` & `pyaedt-0.6.78/pyaedt/maxwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,17 +7,18 @@
 import json
 import os
 import re
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.generic.DataHandlers import float_units
 from pyaedt.generic.constants import SOLUTIONS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import MaxwellParameters
 from pyaedt.modules.SetupTemplates import SetupKeys
```

### Comparing `pyaedt-0.6.77/pyaedt/maxwellcircuit.py` & `pyaedt-0.6.78/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/mechanical.py` & `pyaedt-0.6.78/pyaedt/mechanical.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """This module contains the ``Mechanical`` class."""
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.application.Analysis3D import FieldAnalysis3D
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 
 class Mechanical(FieldAnalysis3D, object):
     """Provides the Mechanical application interface.
```

### Comparing `pyaedt-0.6.77/pyaedt/misc/Console.py_build` & `pyaedt-0.6.78/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.6.78/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.6.78/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.6.78/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.6.78/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/amat.xml` & `pyaedt-0.6.78/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/console_setup.py` & `pyaedt-0.6.78/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.6.78/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.6.78/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.6.78/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.6.78/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/misc.py` & `pyaedt-0.6.78/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.6.78/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.6.78/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.6.78/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.6.78/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.6.78/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/misc/template.acf` & `pyaedt-0.6.78/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/actors.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.modeler.advanced_cad.multiparts import Actor
 from pyaedt.modeler.advanced_cad.multiparts import MultiPartComponent
 
 
 def read_actors(fn, actor_lib):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 import os
 
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.filesystem import get_json_files
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.advanced_cad.parts import Antenna
 from pyaedt.modeler.advanced_cad.parts import Part
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class MultiPartComponent(object):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/parts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import os
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Part(object):
     """Manages 3D component placement and definition.
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.6.78/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,17 +11,18 @@
     try:
         import numpy as np
     except ImportError:
         pass
 
 from pyaedt import constants
 from pyaedt import pyaedt_path
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import is_ironpython
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.MaterialLib import Material
 
 LAYERS = {"s": "signal", "g": "ground", "d": "dielectric"}
 
 
 def _replace_by_underscore(character, string):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/Modeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 import copy
 import math
 import os
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.geometry_operators import GeometryOperators
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,19 +9,20 @@
 import os
 import random
 import string
 import time
 
 from pyaedt.application.Variables import Variable
 from pyaedt.application.Variables import decompose_variable_value
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import is_number
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.components_3d import UserDefinedComponent
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import Plane
 from pyaedt.modeler.cad.elements3d import Point
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.cad.polylines import Polyline
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives2D.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyaedt.generic.general_methods import property
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Primitives import Primitives
 
 
 class Primitives2D(Primitives, object):
     """Manages primitives in 2D tools.
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/Primitives3D.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/components_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import random
 import re
 import warnings
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.general_methods import _uname
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import _dict2arg
 
 
 class UserDefinedComponentParameters(dict):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/elements3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import absolute_import
 
 from collections import OrderedDict
 
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import clamp
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 @pyaedt_function_handler()
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/object3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 """
 from __future__ import absolute_import  # noreorder
 
 import os
 import re
 
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _to_boolean
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import clamp
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import rgb_color_codes
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import BinaryTreeNode
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.6.78/pyaedt/modeler/cad/polylines.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import absolute_import
 
 import math
 import warnings
 
+# from pyaedt import property
 from pyaedt import _retry_ntimes
-from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import PLANE
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.object3d import Object3d
 from pyaedt.modeler.geometry_operators import GeometryOperators
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/calculators.py` & `pyaedt-0.6.78/pyaedt/modeler/calculators.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import math
 
 from pyaedt import constants
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import SpeedOfLight
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class TransmissionLine(object):
     """Provides base methods common to transmission line calculation.
 
     Parameters
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import os
 import random
 import warnings
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import filter_string
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import recursive_glob
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modeler.circuits.object3dcircuit import Wire
 
 
 class CircuitComponents(object):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import defaultdict
 
 from pyaedt.emit_core import EmitConstants as emit_consts
 import pyaedt.generic.constants as consts
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class EmitComponents(object):
     """EmitComponents class.
 
     This is the class for managing all EMIT components.
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyaedt.generic.general_methods import property
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 
 
 class MaxwellCircuitComponents(CircuitComponents):
     """MaxwellCircuitComponents class.
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import random
 import re
 import warnings
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 from pyaedt.modeler.circuits.PrimitivesCircuit import ComponentCatalog
 from pyaedt.modeler.circuits.object3dcircuit import CircuitComponent
 from pyaedt.modules.Boundary import Excitations
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pyaedt.generic.general_methods import property
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.circuits.PrimitivesCircuit import CircuitComponents
 from pyaedt.modeler.circuits.PrimitivesCircuit import ComponentCatalog
 
 
 class TwinBuilderComponents(CircuitComponents):
     """TwinBuilderComponents class.
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.6.78/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 
 from collections import OrderedDict
 import math
 
+# from pyaedt import property
 from pyaedt import _retry_ntimes
-from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import _arg2dict
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.cad.elements3d import _dict2arg
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.6.78/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modeler/modeler2d.py` & `pyaedt-0.6.78/pyaedt/modeler/modeler2d.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from warnings import warn
 
-from pyaedt.generic.general_methods import property
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.cad.Primitives2D import Primitives2D
 
 
 class ModelerRMxprt(Modeler):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/modeler3d.py` & `pyaedt-0.6.78/pyaedt/modeler/modeler3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 import copy
 import datetime
 import json
 import os.path
 import warnings
 
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import GeometryModeler
 from pyaedt.modeler.cad.Primitives3D import Primitives3D
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Modeler3D(GeometryModeler, Primitives3D, object):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.6.78/pyaedt/modeler/modelerpcb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import os
 import re
 from warnings import warn
 
 from pyaedt import settings
 from pyaedt.edb import Edb
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import get_filename_without_extension
 from pyaedt.generic.general_methods import inside_desktop
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.pcb.Primitives3DLayout import Primitives3DLayout
 from pyaedt.modeler.pcb.object3dlayout import ComponentsSubCircuit3DLayout
 from pyaedt.modules.LayerStackup import Layers
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.6.78/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import sys
 import warnings
 
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import _uname
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Primitives import default_materials
 from pyaedt.modeler.geometry_operators import GeometryOperators
 from pyaedt.modeler.pcb.object3dlayout import Circle3dLayout
 from pyaedt.modeler.pcb.object3dlayout import Components3DLayout
 from pyaedt.modeler.pcb.object3dlayout import ComponentsSubCircuit3DLayout
 from pyaedt.modeler.pcb.object3dlayout import Line3dLayout
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.6.78/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 
 """
 from __future__ import absolute_import  # noreorder
 
 import math
 import re
 
+# from pyaedt import property
 from pyaedt import _retry_ntimes
-from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 class Objec3DLayout(object):
```

### Comparing `pyaedt-0.6.77/pyaedt/modeler/schematic.py` & `pyaedt-0.6.78/pyaedt/modeler/schematic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 import random
 import re
 
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.Modeler import Modeler
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponent
 from pyaedt.modeler.circuits.PrimitivesEmit import EmitComponents
 from pyaedt.modeler.circuits.PrimitivesMaxwellCircuit import MaxwellCircuitComponents
 from pyaedt.modeler.circuits.PrimitivesNexxim import NexximComponents
 from pyaedt.modeler.circuits.PrimitivesTwinBuilder import TwinBuilderComponents
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.6.78/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modules/Boundary.py` & `pyaedt-0.6.78/pyaedt/modules/Boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from collections import OrderedDict
 import copy
 import re
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.DataHandlers import random_string
 from pyaedt.generic.constants import CATEGORIESQ3D
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import _dim_arg
 from pyaedt.generic.general_methods import filter_tuple
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 from pyaedt.modules.CircuitTemplates import SourceKeys
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/CableModeling.py` & `pyaedt-0.6.78/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.6.78/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.6.78/pyaedt/modules/DesignXPloration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from collections import OrderedDict
 import copy
 import csv
 
 from pyaedt.generic.DataHandlers import _arg2dict
 from pyaedt.generic.DataHandlers import _dict2arg
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.OptimetricsTemplates import defaultdoeSetup
 from pyaedt.modules.OptimetricsTemplates import defaultdxSetup
 from pyaedt.modules.OptimetricsTemplates import defaultoptiSetup
 from pyaedt.modules.OptimetricsTemplates import defaultparametricSetup
 from pyaedt.modules.OptimetricsTemplates import defaultsensitivitySetup
 from pyaedt.modules.OptimetricsTemplates import defaultstatisticalSetup
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/LayerStackup.py` & `pyaedt-0.6.78/pyaedt/modules/LayerStackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import unit_converter
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 @pyaedt_function_handler()
 def _str2bool(str0):
     """Convert a string to a Boolean value.
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/Material.py` & `pyaedt-0.6.78/pyaedt/modules/Material.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 * `SufaceMaterial`
 
 """
 from collections import OrderedDict
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import CSS4_COLORS
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class MatProperties(object):
     """Contains a list of constant names for all materials with
     mappings to their internal XML names.
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/MaterialLib.py` & `pyaedt-0.6.78/pyaedt/modules/MaterialLib.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,19 +11,20 @@
 import os
 import re
 import sys
 
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.generic.DataHandlers import _arg2dict
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _create_json_file
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Material import MatProperties
 from pyaedt.modules.Material import Material
 from pyaedt.modules.Material import OrderedDict
 from pyaedt.modules.Material import SurfaceMaterial
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/Mesh.py` & `pyaedt-0.6.78/pyaedt/modules/Mesh.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 from collections import OrderedDict
 import os
 import shutil
 
 from pyaedt.application.design_solutions import model_names
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import MethodNotSupportedError
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.generic.general_methods import settings
 from pyaedt.modeler.cad.elements3d import EdgePrimitive
 from pyaedt.modeler.cad.elements3d import FacePrimitive
 from pyaedt.modeler.cad.elements3d import VertexPrimitive
 
 meshers = {
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.6.78/pyaedt/modules/Mesh3DLayout.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 
 """
 from __future__ import absolute_import  # noreorder
 
 from collections import OrderedDict
 
 from pyaedt.generic.DataHandlers import _dict2arg
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Mesh import MeshProps
 
 
 class Mesh3DOperation(PropsManager, object):
     """Mesh3DOperation class.
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.6.78/pyaedt/modules/MeshIcepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from collections import OrderedDict
 
 from pyaedt import settings
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.Mesh import MeshOperation
 from pyaedt.modules.Mesh import meshers
 
 
 class IcepakMesh(object):
     """Manages Icepak meshes.
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.6.78/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modules/PostProcessor.py` & `pyaedt-0.6.78/pyaedt/modules/PostProcessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,19 +13,20 @@
 import string
 
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.DataHandlers import json_to_dict
 from pyaedt.generic.constants import unit_converter
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _retry_ntimes
 from pyaedt.generic.general_methods import check_and_download_file
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 import pyaedt.modules.report_templates as rt
 from pyaedt.modules.solutions import FieldPlot
 from pyaedt.modules.solutions import SolutionData
 from pyaedt.modules.solutions import VRTFieldPlot
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.6.78/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/modules/SolveSetup.py` & `pyaedt-0.6.78/pyaedt/modules/SolveSetup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,18 @@
 import os.path
 from random import randrange
 import time
 import warnings
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import AEDT_UNITS
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import PropsManager
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modules.SetupTemplates import SetupKeys
 from pyaedt.modules.SolveSweeps import SetupProps
 from pyaedt.modules.SolveSweeps import SweepHFSS
 from pyaedt.modules.SolveSweeps import SweepHFSS3DLayout
 from pyaedt.modules.SolveSweeps import SweepMatrix
 from pyaedt.modules.SolveSweeps import identify_setup
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.6.78/pyaedt/modules/SolveSweeps.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import copy
 from difflib import SequenceMatcher
 import json
 import os
 import sys
 import warnings
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.LoadAEDTFile import load_entire_aedt_file
 from pyaedt.modules.SetupTemplates import Sweep3DLayout
 from pyaedt.modules.SetupTemplates import SweepHfss3D
 from pyaedt.modules.SetupTemplates import SweepSiwave
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.6.78/pyaedt/modules/monitor_icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 
 from pyaedt.generic.DataHandlers import _dict2arg
 from pyaedt.generic.constants import SI_UNITS
 from pyaedt.generic.constants import unit_system
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class Monitor:
     """Provides Icepak monitor methods."""
 
     def __init__(self, p_app):
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/report_templates.py` & `pyaedt-0.6.78/pyaedt/modules/report_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 import copy
 import os
 import re
 
 from pyaedt.generic.constants import LineStyle
 from pyaedt.generic.constants import SymbolStyle
 from pyaedt.generic.constants import TraceType
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators
 
 
 def _props_with_default(dict_in, key, default_value=None):
     return dict_in[key] if dict_in.get(key, None) is not None else default_value
```

### Comparing `pyaedt-0.6.77/pyaedt/modules/solutions.py` & `pyaedt-0.6.78/pyaedt/modules/solutions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from collections import OrderedDict
 import itertools
 import math
 import os
 import sys
 import time
 
+# from pyaedt import property
 from pyaedt import get_pyaedt_app
 from pyaedt import is_ironpython
-from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt import settings
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.constants import db10
 from pyaedt.generic.constants import db20
 from pyaedt.generic.constants import unit_converter
 from pyaedt.generic.general_methods import check_and_download_folder
```

### Comparing `pyaedt-0.6.77/pyaedt/q3d.py` & `pyaedt-0.6.78/pyaedt/q3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 
 from pyaedt import is_ironpython
 from pyaedt import settings
 from pyaedt.application.Analysis3D import FieldAnalysis3D
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.constants import MATRIXOPERATIONSQ2D
 from pyaedt.generic.constants import MATRIXOPERATIONSQ3D
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import generate_unique_name
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.modeler.geometry_operators import GeometryOperators as go
 from pyaedt.modules.Boundary import BoundaryObject
 from pyaedt.modules.Boundary import Matrix
 from pyaedt.modules.SetupTemplates import SetupKeys
 
 if not is_ironpython:
```

### Comparing `pyaedt-0.6.77/pyaedt/rmxprt.py` & `pyaedt-0.6.78/pyaedt/rmxprt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains these classes: ``RMXprtModule`` and ``Rmxprt``."""
 from __future__ import absolute_import  # noreorder
 
 from pyaedt.application.AnalysisRMxprt import FieldAnalysisRMxprt
-from pyaedt.generic.general_methods import property
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 
 
 class RMXprtModule(object):
     """Provides RMxprt module properties."""
 
     component = None
```

### Comparing `pyaedt-0.6.77/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.6.78/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.6.78/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.6.78/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.6.78/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyaedt/sbrplus/plot.py` & `pyaedt-0.6.78/pyaedt/sbrplus/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import math
 import os
 import warnings
 
 import numpy as np
 import pyvista as pv
 
-from pyaedt import property
+# from pyaedt import property
 from pyaedt import pyaedt_function_handler
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.plot import CommonPlotter
 from pyaedt.generic.plot import ObjClass
 
 
 class HDMPlotter(CommonPlotter):
```

### Comparing `pyaedt-0.6.77/pyaedt/siwave.py` & `pyaedt-0.6.78/pyaedt/siwave.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,18 +9,19 @@
 
 import os
 import pkgutil
 import sys
 import time
 
 from pyaedt.generic.clr_module import _clr
+
+# from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import _pythonver
 from pyaedt.generic.general_methods import is_ironpython
 from pyaedt.generic.general_methods import is_windows
-from pyaedt.generic.general_methods import property
 from pyaedt.generic.general_methods import pyaedt_function_handler
 from pyaedt.misc import list_installed_ansysem
 
 
 class Siwave(object):
     """Initializes SIwave based on the inputs provided and manages SIwave release and closing.
```

### Comparing `pyaedt-0.6.77/pyaedt/twinbuilder.py` & `pyaedt-0.6.78/pyaedt/twinbuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.6.77/pyproject.toml` & `pyaedt-0.6.78/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,16 @@
     "openpyxl==3.1.2",
     "osmnx",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "pytest==7.3.1",
     "pytest-cov==4.0.0",
     "pytest-xdist==3.3.1",
-    "pyvista==0.39.1",
+    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.38.0; python_version <= '3.7'",
     "scikit-learn==1.2.2",
     "SRTM.py",
     "utm",
     "scikit-rf",
 
 ]
 doc = [
@@ -67,15 +68,16 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "nbsphinx==0.9.2",
     "numpydoc==1.5.0",
     "osmnx",
     "pypandoc==1.11",
     "pytest-sphinx==0.5.0",
-    "pyvista==0.39.1",
+    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.38.0; python_version <= '3.7'",
     "recommonmark==0.7.1",
     "scikit-learn==1.2.2",
     "Sphinx==7.0.1",
     "sphinx-autobuild==2021.3.14",
     "sphinx-autodoc-typehints==1.23.0",
     "sphinx-copybutton==0.5.2",
     "sphinx-gallery==0.13.0",
@@ -91,30 +93,32 @@
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.39.1",
+    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 all = [
     "imageio==2.29.0",
     "matplotlib==3.5.3; python_version <= '3.7'",
     "matplotlib==3.7.1; python_version > '3.7'",
     "numpy==1.21.6; python_version <= '3.7'",
     "numpy==1.24.3; python_version > '3.7'",
     "pandas==1.3.5; python_version <= '3.7'",
     "pandas==2.0.1; python_version > '3.7'",
     "osmnx",
-    "pyvista==0.39.1",
+    "pyvista==0.39.1; python_version > '3.7'",
+    "pyvista==0.38.0; python_version <= '3.7'",
     "SRTM.py",
     "utm",
     "scikit-rf",
     "openpyxl==3.1.2",
 ]
 
 [tool.flit.module]
```

### Comparing `pyaedt-0.6.77/PKG-INFO` & `pyaedt-0.6.78/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.6.77
+Version: 0.6.78
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -25,15 +25,16 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "all" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "all"
-Requires-Dist: pyvista==0.39.1 ; extra == "all"
+Requires-Dist: pyvista==0.39.1 ; extra == "all" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.38.0 ; extra == "all" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "all"
 Requires-Dist: utm ; extra == "all"
 Requires-Dist: scikit-rf ; extra == "all"
 Requires-Dist: openpyxl==3.1.2 ; extra == "all"
 Requires-Dist: ansys-sphinx-theme==0.9.9 ; extra == "doc"
 Requires-Dist: imageio==2.29.0 ; extra == "doc"
 Requires-Dist: imageio-ffmpeg==0.4.8 ; extra == "doc"
@@ -44,15 +45,16 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: nbsphinx==0.9.2 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
 Requires-Dist: osmnx ; extra == "doc"
 Requires-Dist: pypandoc==1.11 ; extra == "doc"
 Requires-Dist: pytest-sphinx==0.5.0 ; extra == "doc"
-Requires-Dist: pyvista==0.39.1 ; extra == "doc"
+Requires-Dist: pyvista==0.39.1 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.38.0 ; extra == "doc" and ( python_version <= '3.7')
 Requires-Dist: recommonmark==0.7.1 ; extra == "doc"
 Requires-Dist: scikit-learn==1.2.2 ; extra == "doc"
 Requires-Dist: Sphinx==7.0.1 ; extra == "doc"
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc"
 Requires-Dist: sphinx-autodoc-typehints==1.23.0 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.13.0 ; extra == "doc"
@@ -66,15 +68,16 @@
 Requires-Dist: matplotlib==3.5.3 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: matplotlib==3.7.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: numpy==1.21.6 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: numpy==1.24.3 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: pandas==1.3.5 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "full" and ( python_version > '3.7')
 Requires-Dist: osmnx ; extra == "full"
-Requires-Dist: pyvista==0.39.1 ; extra == "full"
+Requires-Dist: pyvista==0.39.1 ; extra == "full" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.38.0 ; extra == "full" and ( python_version <= '3.7')
 Requires-Dist: SRTM.py ; extra == "full"
 Requires-Dist: utm ; extra == "full"
 Requires-Dist: scikit-rf ; extra == "full"
 Requires-Dist: openpyxl==3.1.2 ; extra == "full"
 Requires-Dist: ipython==8.13.0 ; extra == "tests"
 Requires-Dist: imageio==2.29.0 ; extra == "tests"
 Requires-Dist: joblib==1.2.0 ; extra == "tests"
@@ -85,15 +88,16 @@
 Requires-Dist: openpyxl==3.1.2 ; extra == "tests"
 Requires-Dist: osmnx ; extra == "tests"
 Requires-Dist: pandas==1.3.5 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: pandas==2.0.1 ; extra == "tests" and ( python_version > '3.7')
 Requires-Dist: pytest==7.3.1 ; extra == "tests"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "tests"
 Requires-Dist: pytest-xdist==3.3.1 ; extra == "tests"
-Requires-Dist: pyvista==0.39.1 ; extra == "tests"
+Requires-Dist: pyvista==0.39.1 ; extra == "tests" and ( python_version > '3.7')
+Requires-Dist: pyvista==0.38.0 ; extra == "tests" and ( python_version <= '3.7')
 Requires-Dist: scikit-learn==1.2.2 ; extra == "tests"
 Requires-Dist: SRTM.py ; extra == "tests"
 Requires-Dist: utm ; extra == "tests"
 Requires-Dist: scikit-rf ; extra == "tests"
 Project-URL: Bug Tracker, https://github.com/pyansys/pyaedt/issues
 Project-URL: Documentation, https://aedt.docs.pyansys.com
 Project-URL: Source Code, https://github.com/pyansys/pyaedt
```

