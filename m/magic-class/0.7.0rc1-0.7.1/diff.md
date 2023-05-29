# Comparing `tmp/magic_class-0.7.0rc1.tar.gz` & `tmp/magic_class-0.7.1.tar.gz`

## Comparing `magic_class-0.7.0rc1.tar` & `magic_class-0.7.1.tar`

### file list

```diff
@@ -1,133 +1,137 @@
--rw-r--r--   0        0        0     2645 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/__init__.py
--rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_app.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_register_types.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/command_palette.py
--rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/core.py
--rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/core.pyi
--rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/help.py
--rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/plot_api.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/signature.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/testing.py
--rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/undo.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/__init__.py
--rw-r--r--   0        0        0    46952 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_base.py
--rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_dock_widget.py
--rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_function_gui.py
--rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_gui_modes.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_icon.py
--rw-r--r--   0        0        0    21903 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_macro.py
--rw-r--r--   0        0        0    13059 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_macro_utils.py
--rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_message_box.py
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/_napari_type.py
--rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/class_gui.py
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/keybinding.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/menu_gui.py
--rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/mgui_ext.py
--rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/runner.py
--rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/toolbar.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/_gui/utils.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/_doc.py
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/_shared_utils.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/__init__.py
--rw-r--r--   0        0        0     7973 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/progress.py
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/dask/resource.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/__init__.py
--rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/_magicgui.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/types.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/utils.py
--rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/viewer.py
--rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/napari/widgets.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/__init__.py
--rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/tests/__init__.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pandas/tests/test_viewer.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/__init__.py
--rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/_viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/tests/__init__.py
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/polars/tests/test_viewer.py
--rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/_const.py
--rw-r--r--   0        0        0     6254 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/components.py
--rw-r--r--   0        0        0    22882 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/graph_items.py
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/mouse_event.py
--rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/plot_api.py
--rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/widgets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/__init__.py
--rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/__init__.py
--rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/_qt.py
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/qtconsole/widgets.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/__init__.py
--rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/_base.py
--rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/camera.py
--rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layer2d.py
--rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layer3d.py
--rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/layerlist.py
--rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/plot_api.py
--rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/widgets2d.py
--rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/widgets3d.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/tests/__init__.py
--rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vispy/tests/test_vispy2d.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/__init__.py
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/components.py
--rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/const.py
--rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/volume.py
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/ext/vtk/widgets.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/__init__.py
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_define.py
--rw-r--r--   0        0        0    29294 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_fields.py
--rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_group.py
--rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/fields/_property.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/__init__.py
--rw-r--r--   0        0        0     8480 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_dispatch.py
--rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_partial.py
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/functools/_wraps.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/logging/__init__.py
--rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/logging/core.py
--rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/stylesheets/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_bound.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_choices.py
--rw-r--r--   0        0        0     1372 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_const.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_expr.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_optional.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_path.py
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/types/_union.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/__init__.py
--rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_click.py
--rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_functions.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/_recent.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qt.py
--rw-r--r--   0        0        0    31513 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qthreading.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/utils/qtsignal.py
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/__init__.py
--rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/_html.py
--rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/_mpl_canvas.py
--rw-r--r--   0        0        0    25094 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/codeedit.py
--rw-r--r--   0        0        0    10457 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/color.py
--rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/containers.py
--rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/eval.py
--rw-r--r--   0        0        0    19319 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/logger.py
--rw-r--r--   0        0        0    18103 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/misc.py
--rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/plot.py
--rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/separator.py
--rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/toggle_switch.py
--rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/utils.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/__init__.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/dict.py
--rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/list.py
--rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/object.py
--rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/pywidgets/tree.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/tests/__init__.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/widgets/tests/test_eval.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/__init__.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_abstractapi.py
--rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_confirm.py
--rw-r--r--   0        0        0     8771 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_misc.py
--rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/magicclass/wrappers/_preview.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/.gitignore
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/LICENSE
--rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/README.md
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7383 2020-02-02 00:00:00.000000 magic_class-0.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     2642 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/__init__.py
+-rw-r--r--   0        0        0     1247 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_app.py
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_register_types.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/command_palette.py
+-rw-r--r--   0        0        0    23018 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/core.py
+-rw-r--r--   0        0        0     6684 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/core.pyi
+-rw-r--r--   0        0        0    11386 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/help.py
+-rw-r--r--   0        0        0     4152 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/plot_api.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/signature.py
+-rw-r--r--   0        0        0     5419 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/undo.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/__init__.py
+-rw-r--r--   0        0        0    47075 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_base.py
+-rw-r--r--   0        0        0     1487 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_dock_widget.py
+-rw-r--r--   0        0        0     9730 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_function_gui.py
+-rw-r--r--   0        0        0     3466 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_gui_modes.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_icon.py
+-rw-r--r--   0        0        0    23956 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_macro.py
+-rw-r--r--   0        0        0    12944 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_macro_utils.py
+-rw-r--r--   0        0        0    10935 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_message_box.py
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/_napari_type.py
+-rw-r--r--   0        0        0    26462 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/class_gui.py
+-rw-r--r--   0        0        0     5412 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/keybinding.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/menu_gui.py
+-rw-r--r--   0        0        0    13434 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/mgui_ext.py
+-rw-r--r--   0        0        0     3033 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/runner.py
+-rw-r--r--   0        0        0    11803 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/toolbar.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/_gui/utils.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/__init__.py
+-rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/_doc.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/_shared_utils.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/dask/__init__.py
+-rw-r--r--   0        0        0     8005 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/dask/progress.py
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/dask/resource.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/__init__.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/_magicgui.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/types.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/utils.py
+-rw-r--r--   0        0        0     2947 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/viewer.py
+-rw-r--r--   0        0        0     1728 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/napari/widgets.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pandas/__init__.py
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pandas/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pandas/tests/__init__.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pandas/tests/test_viewer.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/polars/__init__.py
+-rw-r--r--   0        0        0     6190 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/polars/_viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/polars/tests/__init__.py
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/polars/tests/test_viewer.py
+-rw-r--r--   0        0        0     2167 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/_const.py
+-rw-r--r--   0        0        0     6918 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/components.py
+-rw-r--r--   0        0        0    24189 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/graph_items.py
+-rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/mouse_event.py
+-rw-r--r--   0        0        0     3635 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/plot_api.py
+-rw-r--r--   0        0        0    32686 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/widgets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/tests/__init__.py
+-rw-r--r--   0        0        0     4055 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/qtconsole/__init__.py
+-rw-r--r--   0        0        0     3433 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/qtconsole/_qt.py
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/qtconsole/widgets.py
+-rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/__init__.py
+-rw-r--r--   0        0        0     4202 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/_base.py
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/camera.py
+-rw-r--r--   0        0        0     6911 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/layer2d.py
+-rw-r--r--   0        0        0    20691 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/layer3d.py
+-rw-r--r--   0        0        0      698 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/layerlist.py
+-rw-r--r--   0        0        0     3451 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/plot_api.py
+-rw-r--r--   0        0        0    11628 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/widgets2d.py
+-rw-r--r--   0        0        0    10544 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/widgets3d.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/tests/__init__.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vispy/tests/test_vispy2d.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vtk/__init__.py
+-rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vtk/components.py
+-rw-r--r--   0        0        0     1055 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vtk/const.py
+-rw-r--r--   0        0        0     5108 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vtk/volume.py
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/ext/vtk/widgets.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/fields/__init__.py
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/fields/_define.py
+-rw-r--r--   0        0        0    29154 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/fields/_fields.py
+-rw-r--r--   0        0        0    14681 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/fields/_group.py
+-rw-r--r--   0        0        0    10491 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/fields/_property.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/functools/__init__.py
+-rw-r--r--   0        0        0     6368 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/functools/_dispatch.py
+-rw-r--r--   0        0        0     3772 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/functools/_partial.py
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/functools/_wraps.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/logging/__init__.py
+-rw-r--r--   0        0        0     4980 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/logging/core.py
+-rw-r--r--   0        0        0     1268 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/stylesheets/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/testing/__init__.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/testing/_function_gui_test.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/testing/_gui_test.py
+-rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_bound.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_choices.py
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_const.py
+-rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_expr.py
+-rw-r--r--   0        0        0     2881 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_optional.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_path.py
+-rw-r--r--   0        0        0     2105 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/types/_union.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/__init__.py
+-rw-r--r--   0        0        0     3206 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/_click.py
+-rw-r--r--   0        0        0     7065 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/_functions.py
+-rw-r--r--   0        0        0     2901 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/_recent.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/qt.py
+-rw-r--r--   0        0        0    32376 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/qthreading.py
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/utils/qtsignal.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/__init__.py
+-rw-r--r--   0        0        0     7197 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/_html.py
+-rw-r--r--   0        0        0     8380 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/_mpl_canvas.py
+-rw-r--r--   0        0        0     2476 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/_union.py
+-rw-r--r--   0        0        0    25634 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/codeedit.py
+-rw-r--r--   0        0        0    12065 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/color.py
+-rw-r--r--   0        0        0    14327 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/colormap.py
+-rw-r--r--   0        0        0    23314 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/containers.py
+-rw-r--r--   0        0        0    11197 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/eval.py
+-rw-r--r--   0        0        0    20883 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/logger.py
+-rw-r--r--   0        0        0    16683 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/misc.py
+-rw-r--r--   0        0        0    15329 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/plot.py
+-rw-r--r--   0        0        0     3245 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/separator.py
+-rw-r--r--   0        0        0     4566 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/toggle_switch.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/utils.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/pywidgets/__init__.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/pywidgets/dict.py
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/pywidgets/list.py
+-rw-r--r--   0        0        0     3858 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/pywidgets/object.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/pywidgets/tree.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/tests/__init__.py
+-rw-r--r--   0        0        0     1033 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/widgets/tests/test_eval.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/wrappers/__init__.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/wrappers/_abstractapi.py
+-rw-r--r--   0        0        0     3801 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/wrappers/_confirm.py
+-rw-r--r--   0        0        0     9206 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/wrappers/_misc.py
+-rw-r--r--   0        0        0     6151 2020-02-02 00:00:00.000000 magic_class-0.7.1/magicclass/wrappers/_preview.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 magic_class-0.7.1/.gitignore
+-rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 magic_class-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4206 2020-02-02 00:00:00.000000 magic_class-0.7.1/README.md
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 magic_class-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 magic_class-0.7.1/PKG-INFO
```

### Comparing `magic_class-0.7.0rc1/magicclass/__init__.py` & `magic_class-0.7.1/magicclass/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.7.0rc1"
+__version__ = "0.7.1"
 
 from .core import (
     magicclass,
     magicmenu,
     magiccontext,
     magictoolbar,
     Parameters,
```

### Comparing `magic_class-0.7.0rc1/magicclass/_app.py` & `magic_class-0.7.1/magicclass/_app.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_register_types.py` & `magic_class-0.7.1/magicclass/_register_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 import macrokit as mk
 from macrokit import Expr, Head, symbol
 from enum import Enum
 import pathlib
 import datetime
-from magicclass.types import Color, Path, ExprStr
-from magicclass.widgets import ColorEdit, EvalLineEdit
+from magicclass.types import Color, Colormap, Path, ExprStr
+from magicclass.widgets import ColorEdit, EvalLineEdit, ColormapEdit
 from magicclass._gui._base import MagicTemplate
 
 # classes
 _datetime = Expr(Head.getattr, [datetime, datetime.datetime])
 _date = Expr(Head.getattr, [datetime, datetime.date])
 _time = Expr(Head.getattr, [datetime, datetime.time])
 _timedelta = Expr(Head.getattr, [datetime, datetime.timedelta])
@@ -53,11 +53,12 @@
     else:
         return Expr(Head.getattr, [find_myname(parent), gui._my_symbol])
 
 
 import magicgui as mgui
 
 mgui.register_type(Color, widget_type=ColorEdit)
+mgui.register_type(Colormap, widget_type=ColormapEdit)
 mgui.register_type(Path.Save, widget_type="FileEdit", mode="w")
 mgui.register_type(Path.Dir, widget_type="FileEdit", mode="d")
 mgui.register_type(Path.Multiple, widget_type="FileEdit", mode="rm")
 mgui.register_type(ExprStr, widget_type=EvalLineEdit)
```

### Comparing `magic_class-0.7.0rc1/magicclass/command_palette.py` & `magic_class-0.7.1/magicclass/command_palette.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/core.py` & `magic_class-0.7.1/magicclass/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/core.pyi` & `magic_class-0.7.1/magicclass/core.pyi`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/help.py` & `magic_class-0.7.1/magicclass/help.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/plot_api.py` & `magic_class-0.7.1/magicclass/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/signature.py` & `magic_class-0.7.1/magicclass/signature.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,38 @@
 from __future__ import annotations
-from typing import Any, Callable, TypedDict
+
+from typing import Any, Callable, TypedDict, overload, Literal, TYPE_CHECKING
 from typing_extensions import _AnnotatedAlias, get_args
+
 from magicgui.signature import MagicSignature
 from magicgui.widgets import FunctionGui
 import inspect
+
+from macrokit import Mock
 from magicclass.utils import get_signature
 
+if TYPE_CHECKING:
+    from magicclass._gui import BaseGui
+
 
-class AdditionalOptions(TypedDict):
+class ConfirmDict(TypedDict):
+    text: str
+    condition: str | Mock | Callable
+    callback: Callable[[str, BaseGui], Any]
+
+
+class AdditionalOptions(TypedDict, total=False):
     record: bool
     keybinding: str
     into: str
     copyto: str
     moveto: str
     gui: bool
     on_called: list[Callable]
+    confirm: ConfirmDict
 
 
 def upgrade_signature(
     func,
     gui_options: dict = None,
     caller_options: dict = None,
     additional_options: AdditionalOptions = None,
@@ -72,15 +86,31 @@
         caller_options=new_caller_options,
         additional_options=new_additional_options,
     )
 
     return func
 
 
-def get_additional_option(obj: Any, option: str, default: Any = None):
+# fmt: off
+@overload
+def get_additional_option(obj: Any, option: Literal["preview"], default: Any = None) -> tuple[str, bool, Callable]: ...
+@overload
+def get_additional_option(obj: Any, option: Literal["confirm"], default: Any = None) -> ConfirmDict: ...
+@overload
+def get_additional_option(obj: Any, option: Literal["gui"], default: Any = None) -> bool: ...
+@overload
+def get_additional_option(obj: Any, option: Literal["record"], default: Any = None) -> str: ...
+@overload
+def get_additional_option(obj: Any, option: Literal["setup"], default: Any = None) -> Callable: ...
+@overload
+def get_additional_option(obj: Any, option: str, default: Any = None) -> Any: ...
+# fmt: on
+
+
+def get_additional_option(obj, option, default=None):
     """Safely get an additional option from any objects."""
     if isinstance(obj, FunctionGui):
         sig = getattr(obj._function, "__signature__", None)
     else:
         sig = getattr(obj, "__signature__", None)
     if isinstance(sig, MagicMethodSignature):
         opt = sig.additional_options
```

### Comparing `magic_class-0.7.0rc1/magicclass/undo.py` & `magic_class-0.7.1/magicclass/undo.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_base.py` & `magic_class-0.7.1/magicclass/_gui/_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     Iterator,
     TypeVar,
     overload,
     MutableSequence,
 )
 from types import MethodType
 from abc import ABCMeta
-from typing_extensions import _AnnotatedAlias, Literal
+from typing_extensions import _AnnotatedAlias
 import inspect
 import warnings
 from qtpy.QtWidgets import QWidget, QDockWidget
 
 from psygnal import Signal
 from magicgui.signature import MagicParameter
 from magicgui.widgets import (
@@ -61,14 +61,15 @@
     is_instance_method,
     method_as_getter,
     eval_attribute,
 )
 from magicclass.widgets import Separator, FreeWidget
 from magicclass.fields import MagicField, MagicValueField, field, vfield
 from magicclass.signature import (
+    ConfirmDict,
     MagicMethodSignature,
     get_additional_option,
     split_annotated_type,
     upgrade_signature,
 )
 from magicclass.wrappers import abstractapi
 from magicclass.types import BoundLiteral, MGUI_SIMPLE_TYPES
@@ -1052,29 +1053,32 @@
     if isinstance(func.__signature__, MagicMethodSignature):
         func.__signature__.additional_options = getattr(
             func_sig, "additional_options", {}
         )
     return func
 
 
+class MagicGuiBuildError(RuntimeError):
+    """Error raised when magicgui cannot build a gui."""
+
+
 def _build_mgui(widget_: Action | PushButtonPlus, func: Callable, parent: BaseGui):
     """Build a magicgui from a function for the give button/action."""
     if widget_.mgui is not None:
         return widget_.mgui
     try:
         sig = getattr(func, "__signature__", None)
         if isinstance(sig, MagicMethodSignature):
             opt = sig.additional_options
         else:
             opt = {}
 
         # confirmation
-        conf = opt.get("confirm", None)
-        if conf is not None:
-            func = _implement_confirmation(func, parent, **conf)
+        if "confirm" in opt:
+            func = _implement_confirmation(func, parent, opt["confirm"])
 
         # Wrap function to deal with errors in a right way.
         func = parent._error_mode.wrap_handler(func, parent=parent)
 
         call_button = opt.get("call_button", None)
         layout = opt.get("layout", "vertical")
         labels = opt.get("labels", True)
@@ -1098,15 +1102,15 @@
 
     except Exception as e:
         msg = (
             "Exception was raised during building magicgui from method "
             f"{func.__name__}.\n{e.__class__.__name__}: {e}"
         )
         widget_.mgui = None
-        raise type(e)(msg)
+        raise MagicGuiBuildError(msg)
 
     return _connect_functiongui_event(mgui, opt)
 
 
 def _connect_functiongui_event(
     mgui: FunctionGuiPlus, opt: dict[str, Any]
 ) -> FunctionGui:
@@ -1307,29 +1311,28 @@
         raise RuntimeError(popup_mode)
     return _prep
 
 
 def _implement_confirmation(
     method: MethodType,
     self: BaseGui,
-    text: str,
-    condition: Callable[[BaseGui], bool] | str,
-    callback: Callable[[str, BaseGui], None],
+    opt: ConfirmDict,
 ):
     """Implement confirmation callback to a method."""
     sig = inspect.signature(method)
 
     @wraps(method)
     def _method(*args, **kwargs):
         if self[method.__name__].running:
             arguments = sig.bind(*args, **kwargs)
             arguments.apply_defaults()
             all_args = arguments.arguments
             all_args.update(self=self)
             need_confirmation = False
+            condition = opt["condition"]
             if isinstance(condition, str):
                 try:
                     need_confirmation = eval(condition, {}, all_args)
                 except Exception as e:
                     msg = e.args[0]
                     e.args = (
                         f"Exception happened on evaluating condition {condition!r}.\n"
@@ -1341,14 +1344,16 @@
             else:
                 warnings.warn(
                     f"Condition {condition} should be callable or string but got type "
                     f"{type(condition)}. No confirmation was executed.",
                     UserWarning,
                 )
             if need_confirmation:
+                callback = opt["callback"]
+                text = opt["text"]
                 callback(text.format(**all_args), self)
 
         return method(*args, **kwargs)
 
     if hasattr(method, "__signature__"):
         _method.__signature__ = method.__signature__
```

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_dock_widget.py` & `magic_class-0.7.1/magicclass/_gui/_dock_widget.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_function_gui.py` & `magic_class-0.7.1/magicclass/_gui/_function_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_gui_modes.py` & `magic_class-0.7.1/magicclass/_gui/_gui_modes.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_icon.py` & `magic_class-0.7.1/magicclass/_gui/_icon.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_macro.py` & `magic_class-0.7.1/magicclass/_gui/_macro.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 from pathlib import Path
 
 from typing import TYPE_CHECKING, Any, Callable, Iterable, overload
 import warnings
 from qtpy import QtWidgets as QtW, QtCore
 from macrokit import Symbol, Expr, Head, BaseMacro, parse
-from magicgui.widgets import FileEdit, LineEdit
+from magicgui.widgets import FileEdit, LineEdit, EmptyWidget, PushButton
+from magicclass.utils.qthreading import thread_worker
 
 from magicclass.widgets import CodeEdit, TabbedContainer, ScrollableContainer, Dialog
 from magicclass.utils import move_to_screen_center
 from magicclass.undo import ImplementsUndo, RedoAction, UndoCallback
 from magicclass._gui.runner import CommandRunnerMenu
 
 if TYPE_CHECKING:
@@ -436,16 +437,20 @@
     def _pop_undo(self) -> ImplementsUndo:
         return self._stack_undo.pop()
 
     @property
     def undo_stack(self) -> dict[str, list[Expr]]:
         """Return a copy of undo stack info."""
         n_undo = len(self._stack_undo)
+        if n_undo == 0:
+            undo = []
+        else:
+            undo = [expr.copy() for expr in self.args[-n_undo:]]
         return dict(
-            undo=[expr.copy() for expr in self.args[-n_undo:]],
+            undo=undo,
             redo=[expr.copy() for expr, _ in self._stack_redo],
         )
 
     def undo(self):
         """Undo the last operation if undo is defined."""
         if len(self._stack_undo) == 0:
             return
@@ -474,15 +479,16 @@
                 parent = self._gui_parent
                 if (viewer := parent.parent_viewer) is not None:
                     ns.setdefault(Symbol.var("viewer"), viewer)
                 with self.blocked():
                     expr.eval(ns)
             elif redo_action.matches("custom"):
                 redo_action: RedoAction.Custom
-                redo_action.run()
+                with self.blocked():
+                    redo_action.run()
             else:
                 raise ValueError(f"Redo is not defined for {undo}")
         except Exception as e:
             self._stack_redo.append((expr, undo))
             raise e
         else:
             self.append(expr)
@@ -532,37 +538,80 @@
         ui = self._gui_parent
         ns.setdefault("ui", ui)
         if (viewer := ui.parent_viewer) is not None:
             ns.setdefault("viewer", viewer)
         return lambda: subset.eval(ns)
 
     def repeat_method(
-        self, index: int = -1, same_args: bool = False, wait: bool = False
+        self,
+        index: int = -1,
+        *,
+        same_args: bool = False,
+        blocking: bool = True,
+        raise_parse_error: bool = True,
+        check_nargs: bool = False,
     ) -> None:
-        _object, _args, _kwargs = self[index].split_call()
-        _ui, *_attributes, _last = _object.split_getattr()
+        """
+        Repeat the method call at the given index.
+
+        Parameters
+        ----------
+        index : int, default is -1
+            Index of the method call to repeat.
+        same_args : bool, default is False
+            If True, method will be called with the same arguments as before. Otherwise,
+            magicgui widget will be opened.
+        blocking : bool, default is True
+            If True, the method will be called in blocking mode if it is a thread worker.
+            Note that programatically calling "repeat_method" in non-blocking mode will
+            cause unexpected macro recording.
+        check_nargs : bool, default is False
+            If False, the method will be called even if it has no arguments. Otherwise,
+            raise ValueError. This option is useful to avoid calling long-running commands.
+        """
+        try:
+            _object, _args, _kwargs = self[index].split_call()
+            _ui, *_attributes, _last = _object.split_getattr()
+        except ValueError as e:
+            if raise_parse_error:
+                raise e
+            else:
+                return None
         ui = self._gui_parent
         assert _ui == ui._my_symbol
         ins = ui
         for attr in _attributes:
             ins = getattr(ins, attr.name)
 
         wdt: Clickable = ins[_last.name]
-        if not wait:
+        if wdt.mgui is None:
+            raise ValueError(f"Method {_object} is not called yet.")
+        if check_nargs and not same_args:
+            n_widget_args = sum(
+                not isinstance(w, EmptyWidget)
+                for w in wdt.mgui
+                if not isinstance(w, PushButton)
+            )
+            if n_widget_args == 0:
+                raise ValueError(f"Method {_object} does not have any arguments.")
+
+        if not blocking:
             if same_args:
-                wdt.mgui.call_button.changed()
+                wdt.mgui.call_button.changed()  # click the call button
             else:
-                wdt.changed()
+                wdt.changed()  # click the button to open magicgui
         else:
             if same_args:
-                wdt.mgui()
+                wdt.mgui()  # call the method
             else:
-                raise NotImplementedError(
-                    "wait=True and same_args=False is not implemented yet."
-                )
+                if isinstance(wdt.mgui._function, thread_worker):
+                    raise ValueError(
+                        "same_args=False is not supported for blocking=True."
+                    )
+                wdt.changed()  # save as blocking=False for non-thread worker
         return None
 
     def _on_macro_added(self, expr=None):
         line = str(self.args[-1])
         if wdt := self.widget.native_macro:
             wdt.append(line)
         if wdt := self.widget.recorded_macro:
```

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_macro_utils.py` & `magic_class-0.7.1/magicclass/_gui/_macro_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -226,16 +226,14 @@
 def _define_macro_recorder(sig: inspect.Signature, func: Callable):
     if isinstance(sig, MagicMethodSignature):
         opt = sig.additional_options
         _auto_call = opt.get("auto_call", False)
     else:
         _auto_call = False
 
-    _qualname = getattr(func, "__qualname__", None)
-
     if sig.return_annotation is inspect.Parameter.empty:
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
             kwargs = dict(bound.arguments.items())
             expr = Expr.parse_method(bgui, func, (), kwargs)
             if _auto_call:
@@ -294,16 +292,14 @@
     base_func = func.func
     if isinstance(sig, MagicMethodSignature):
         opt = sig.additional_options
         _auto_call = opt.get("auto_call", False)
     else:
         _auto_call = False
 
-    _qualname = getattr(base_func, "__qualname__", None)
-
     if sig.return_annotation is inspect.Parameter.empty:
 
         def _record_macro(bgui: MagicTemplate, out, *args, **kwargs):
             bound = sig.bind(*args, **kwargs)
             bound.apply_defaults()
             kwargs = bound.arguments
             expr = Expr.parse_method(bgui, base_func, (), kwargs)
```

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_message_box.py` & `magic_class-0.7.1/magicclass/_gui/_message_box.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/_napari_type.py` & `magic_class-0.7.1/magicclass/_gui/_napari_type.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/class_gui.py` & `magic_class-0.7.1/magicclass/_gui/class_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/keybinding.py` & `magic_class-0.7.1/magicclass/_gui/keybinding.py`

 * *Files 6% similar despite different names*

```diff
@@ -189,24 +189,30 @@
 def strs2keycombo(*args: tuple[str | Key, ...]) -> KeyCombo:
     *modifiers, key = args
     if len(modifiers) > 2:
         raise ValueError("More than two modifiers found.")
     return tuple(Key.to_qtmodifier(m) for m in modifiers) + (Key.to_qtkey(key),)
 
 
-def as_shortcut(key_combo: tuple) -> QKeySequence:
+def _as_shortcut_old(key_combo: tuple) -> QKeySequence:
     if not isinstance(key_combo, tuple):
         raise TypeError(f"Unsupported key combo: {key_combo!r}.")
 
     key0 = key_combo[0]
     if len(key_combo) == 1 and isinstance(key0, str) and not hasattr(Key, key0.lower()):
         qtkeycombo = parse_key_combo(*key_combo)
     else:
         qtkeycombo = strs2keycombo(*key_combo)
     return QKeySequence(_bit_sum(qtkeycombo))
 
 
+def as_shortcut(key_combo) -> QKeySequence:
+    if isinstance(key_combo, str):
+        return QKeySequence(key_combo)
+    return _as_shortcut_old(key_combo)
+
+
 def register_shortcut(keys, parent: QWidget, target: Callable):
     """Register a callback to a key-binding globally."""
     shortcut = QShortcut(as_shortcut(keys), parent)
     shortcut.activated.connect(target)
     return None
```

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/menu_gui.py` & `magic_class-0.7.1/magicclass/_gui/menu_gui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/mgui_ext.py` & `magic_class-0.7.1/magicclass/_gui/mgui_ext.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/runner.py` & `magic_class-0.7.1/magicclass/_gui/runner.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/toolbar.py` & `magic_class-0.7.1/magicclass/_gui/toolbar.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/_gui/utils.py` & `magic_class-0.7.1/magicclass/_gui/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/_doc.py` & `magic_class-0.7.1/magicclass/ext/_doc.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/dask/progress.py` & `magic_class-0.7.1/magicclass/ext/dask/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,39 +18,39 @@
     from magicclass._gui import BaseGui
 
 
 class DaskProgressBar(DefaultProgressBar, DaskCallback):
     """A progress bar widget for dask computation."""
 
     computed = Signal(object)
-    new_cycle = Signal(int)
 
     def __init__(
         self,
         max: int = 100,
         minimum: float = 0.5,
         dt: float = 0.1,
     ):
         self._minimum = minimum
         self._dt = dt
         self._frac = 0.0
         self._n_computation = 0
         super().__init__(max=max)
         self._computed_signal = QtSignal()
         self._computed_signal.connect(self._on_computed)
+        self._new_cycle_signal = QtSignal()
 
     def __enter__(self):
         self._n_computation = 0
         self._on_timer_updated()
         return super().__enter__()
 
     def _start(self, dsk):
         self._state = None
         self._frac = 0.0
-        self.new_cycle.emit(self._n_computation)
+        self._new_cycle_signal.emit(self._n_computation)
         self._n_computation += 1
         self._timer.reset()
         self._start_thread()
         return None
 
     def _on_computed(self, result):
         s = self._state
@@ -188,15 +188,15 @@
                 arguments.apply_defaults()
                 _descs = lambda: descs(**_filter_args(descs, arguments.arguments))
             else:
                 _descs = lambda: iter(descs)
             self._progress["desc"] = next(_descs(), "<No description>")
             it = _descs()
 
-            @pbar.new_cycle.connect
+            @pbar._new_cycle_signal.connect
             def _(i: int):
                 pbar.set_description(next(it, "<No description>"))
 
         pbar.native.setParent(gui.native, self.__class__._WINDOW_FLAG)
         move_to_screen_center(pbar.native)
 
         worker = create_worker(
```

### Comparing `magic_class-0.7.0rc1/magicclass/ext/dask/resource.py` & `magic_class-0.7.1/magicclass/ext/dask/resource.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/napari/_magicgui.py` & `magic_class-0.7.1/magicclass/ext/napari/_magicgui.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/napari/types.py` & `magic_class-0.7.1/magicclass/ext/napari/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Annotated, Iterable, Tuple, List
+from typing import TYPE_CHECKING, Annotated, Iterable
 
 # for now...
 if TYPE_CHECKING:
     import pandas as pd
 
     Features = pd.DataFrame
     FeatureColumn = pd.Series
@@ -49,10 +49,10 @@
     ``tuple[pd.DataFrame, tuple[str, str]]``.
     """
 
     def __new__(cls, *args, **kwargs):
         raise TypeError(f"Type {cls.__name__} cannot be instantiated.")
 
 
-class FeatureInfoInstance(Tuple["pd.DataFrame", List[str]]):
+class FeatureInfoInstance(tuple["pd.DataFrame", list[str]]):
     def __new__(cls, *args, **kwargs):
         raise TypeError(f"Type {cls.__name__} cannot be instantiated.")
```

### Comparing `magic_class-0.7.0rc1/magicclass/ext/napari/utils.py` & `magic_class-0.7.1/magicclass/ext/napari/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/napari/viewer.py` & `magic_class-0.7.1/magicclass/ext/napari/viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/napari/widgets.py` & `magic_class-0.7.1/magicclass/ext/napari/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pandas/_viewer.py` & `magic_class-0.7.1/magicclass/ext/pandas/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pandas/tests/test_viewer.py` & `magic_class-0.7.1/magicclass/ext/pandas/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/polars/_viewer.py` & `magic_class-0.7.1/magicclass/ext/polars/_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/polars/tests/test_viewer.py` & `magic_class-0.7.1/magicclass/ext/polars/tests/test_viewer.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/__init__.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/components.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/components.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
-from typing import Sequence, Tuple
+from typing import Sequence, Tuple, TYPE_CHECKING
 import numpy as np
 import pyqtgraph as pg
 from psygnal import Signal
 from .._shared_utils import convert_color_code, to_rgba
 
+if TYPE_CHECKING:
+    from qtpy.QtWidgets import QGraphicsTextItem
+
 
 class GraphicComponent:
     native: pg.GraphicsObject
 
     @property
     def visible(self) -> bool:
         """Linear region visibility."""
@@ -80,17 +83,18 @@
 
     @border.setter
     def border(self, value):
         value = convert_color_code(value)
         self.native.setPen(pg.mkPen(value))
         self.native._updateView()
 
+
 class Grid(GraphicComponent):
     native: pg.GridItem
-    
+
     def __init__(self) -> None:
         self.native = pg.GridItem()
 
 
 class TextItem(GraphicComponent):
     """A text item with napari-like API."""
 
@@ -101,24 +105,26 @@
     ) -> None:
         self.native = pg.TextItem(
             text, color=convert_color_code(color), anchor=anchor, angle=angle
         )
 
     @property
     def color(self):
+        """Text color."""
         rgba = self.native.color.getRgb()
         return np.array(rgba) / 255
 
     @color.setter
     def color(self, value):
         value = convert_color_code(value)
         self.native.setText(self.text, value)
 
     @property
     def background_color(self):
+        """Text background color"""
         return to_rgba(self.native.fill)
 
     @background_color.setter
     def background_color(self, value):
         value = convert_color_code(value)
         self.native.fill = pg.mkBrush(value)
         self.native._updateView()
@@ -131,38 +137,54 @@
     def border(self, value):
         value = convert_color_code(value)
         self.native.border = pg.mkPen(value)
         self.native._updateView()
 
     @property
     def text(self):
+        """Text string."""
         return self.native.toPlainText()
 
     @text.setter
     def text(self, value: str):
         self.native.setText(value)
 
     @property
     def pos(self) -> np.ndarray:
         pos = self.native.pos()
         return np.array([pos.x(), pos.y()])
 
     @pos.setter
     def pos(self, value):
+        """Text position in the canvas."""
         self.native.setPos(*value)
 
     @property
     def anchor(self) -> np.ndarray:
+        """Anchor relative to the text position."""
         anchor = self.native.anchor
         return np.array([anchor.x(), anchor.y()])
 
     @anchor.setter
     def anchor(self, value):
         self.native.setAnchor(value)
 
+    @property
+    def font_size(self) -> int:
+        """Text font size."""
+        item: QGraphicsTextItem = self.native.textItem
+        return item.font().pointSize()
+
+    @font_size.setter
+    def font_size(self, size: int) -> int:
+        item: QGraphicsTextItem = self.native.textItem
+        font = item.font()
+        font.setPointSize(size)
+        item.setFont(font)
+
 
 class ScaleBar(GraphicComponent):
     """A scale bar with napari-like API"""
 
     native: pg.ScaleBar
 
     def __init__(self):
```

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/graph_items.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/graph_items.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     @zorder.setter
     def zorder(self, value: float):
         self.native.setZValue(value)
 
 
 class PlotDataLayer(LayerItem):
-    native: pg.PlotCurveItem | pg.ScatterPlotItem
+    native: pg.PlotDataItem | pg.ScatterPlotItem
 
     @property
     def xdata(self) -> np.ndarray:
         return self.native.getData()[0]
 
     @xdata.setter
     def xdata(self, value: Sequence[float]):
@@ -102,34 +102,14 @@
             i = [i]
         sl = list(set(range(self.ndata)) - set(i))
         xdata = self.xdata[sl]
         ydata = self.ydata[sl]
         self.native.setData(xdata, ydata)
         return None
 
-    @property
-    def edge_color(self) -> np.ndarray:
-        """Edge color of the data."""
-        return to_rgba(self.native.opts["pen"])
-
-    @edge_color.setter
-    def edge_color(self, value: str | Sequence):
-        value = convert_color_code(value)
-        self.native.setPen(value, width=self.lw, style=self.ls)
-
-    @property
-    def face_color(self) -> np.ndarray:
-        """Face color of the data."""
-        return to_rgba(self.native.opts["brush"])
-
-    @face_color.setter
-    def face_color(self, value: str | Sequence):
-        value = convert_color_code(value)
-        self.native.setBrush(value)
-
     color = property()
 
     @color.setter
     def color(self, value: str | Sequence):
         """Set face color and edge color at the same time."""
         self.face_color = value
         self.edge_color = value
@@ -181,14 +161,34 @@
         symbol = _SYMBOL_MAP.get(symbol, symbol)
         self.native = pg.ScatterPlotItem(
             x=x, y=y, pen=pen, brush=brush, size=size, symbol=symbol
         )
         self.name = name
 
     @property
+    def edge_color(self) -> np.ndarray:
+        """Edge color of the data."""
+        return to_rgba(self.native.opts["pen"])
+
+    @edge_color.setter
+    def edge_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setPen([value] * self.xdata.size, width=self.lw, style=self.ls)
+
+    @property
+    def face_color(self) -> np.ndarray:
+        """Face color of the data."""
+        return to_rgba(self.native.opts["brush"])
+
+    @face_color.setter
+    def face_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setBrush([value] * self.xdata.size)
+
+    @property
     def symbol(self):
         """Get the symbol of the scatter plot."""
         return self.native.opts["symbol"]
 
     @symbol.setter
     def symbol(self, value):
         value = _SYMBOL_MAP.get(value, value)
@@ -303,14 +303,34 @@
         )
         self.name = name
 
     def set_hist(self, data, bins=10, range=None, density=False):
         y, x = np.histogram(data, bins=bins, range=range, density=density)
         self.native.setData(x=x, y=y)
 
+    @property
+    def edge_color(self) -> np.ndarray:
+        """Edge color of the data."""
+        return to_rgba(self.native.opts["pen"])
+
+    @edge_color.setter
+    def edge_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setPen(value, width=self.lw, style=self.ls)
+
+    @property
+    def face_color(self) -> np.ndarray:
+        """Face color of the data."""
+        return to_rgba(self.native.opts["brush"])
+
+    @face_color.setter
+    def face_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setBrush(value)
+
 
 class BarPlot(PlotDataLayer):
     native: pg.BarGraphItem
 
     def __init__(
         self,
         x,
@@ -440,14 +460,34 @@
         return self.native._name
 
     @name.setter
     def name(self, value: str):
         self.native.setName(value)
 
     @property
+    def edge_color(self) -> np.ndarray:
+        """Edge color of the data."""
+        return to_rgba(self.native.opts["pen"])
+
+    @edge_color.setter
+    def edge_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setPen(value, width=self.lw, style=self.ls)
+
+    @property
+    def face_color(self) -> np.ndarray:
+        """Face color of the data."""
+        return to_rgba(self.native.opts["brush"])
+
+    @face_color.setter
+    def face_color(self, value: str | Sequence):
+        value = convert_color_code(value)
+        self.native.setBrush(value)
+
+    @property
     def lw(self):
         """Line width."""
         return self.native.pen.width()
 
     @lw.setter
     def lw(self, value: float):
         self.native.pen.setWidth(value)
```

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/mouse_event.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/mouse_event.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/plot_api.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/widgets.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py` & `magic_class-0.7.1/magicclass/ext/pyqtgraph/tests/test_qtgraph.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/qtconsole/__init__.py` & `magic_class-0.7.1/magicclass/ext/qtconsole/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/qtconsole/_qt.py` & `magic_class-0.7.1/magicclass/ext/qtconsole/_qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/qtconsole/widgets.py` & `magic_class-0.7.1/magicclass/ext/qtconsole/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/_base.py` & `magic_class-0.7.1/magicclass/ext/vispy/_base.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/camera.py` & `magic_class-0.7.1/magicclass/ext/vispy/camera.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/layer2d.py` & `magic_class-0.7.1/magicclass/ext/vispy/layer2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/layer3d.py` & `magic_class-0.7.1/magicclass/ext/vispy/layer3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/layerlist.py` & `magic_class-0.7.1/magicclass/ext/vispy/layerlist.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/plot_api.py` & `magic_class-0.7.1/magicclass/ext/vispy/plot_api.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/widgets2d.py` & `magic_class-0.7.1/magicclass/ext/vispy/widgets2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/widgets3d.py` & `magic_class-0.7.1/magicclass/ext/vispy/widgets3d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vispy/tests/test_vispy2d.py` & `magic_class-0.7.1/magicclass/ext/vispy/tests/test_vispy2d.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vtk/components.py` & `magic_class-0.7.1/magicclass/ext/vtk/components.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vtk/const.py` & `magic_class-0.7.1/magicclass/ext/vtk/const.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vtk/volume.py` & `magic_class-0.7.1/magicclass/ext/vtk/volume.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/ext/vtk/widgets.py` & `magic_class-0.7.1/magicclass/ext/vtk/widgets.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/fields/_define.py` & `magic_class-0.7.1/magicclass/fields/_define.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/fields/_fields.py` & `magic_class-0.7.1/magicclass/fields/_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,31 +168,31 @@
             self.value = kwargs.pop("value")
         self.options.update(kwargs)
         return self
 
     @overload
     def with_choices(
         self, choices: Sequence[tuple[str, _U]]
-    ) -> MagicField[CategoricalWidget, _U]:
+    ) -> MagicField[CategoricalWidget[_U]]:
         ...
 
     @overload
-    def with_choices(self, choices: Sequence[_U]) -> MagicField[CategoricalWidget, _U]:
+    def with_choices(self, choices: Sequence[_U]) -> MagicField[CategoricalWidget[_U]]:
         ...
 
     @overload
     def with_choices(
         self, choices: Callable[..., Sequence[tuple[str, _U]]]
-    ) -> MagicField[CategoricalWidget, _U]:
+    ) -> MagicField[CategoricalWidget[_U]]:
         ...
 
     @overload
     def with_choices(
         self, choices: Callable[..., Sequence[_U]]
-    ) -> MagicField[CategoricalWidget, _U]:
+    ) -> MagicField[CategoricalWidget[_U]]:
         ...
 
     def with_choices(self, choices):
         """Method to add choices to the field."""
         self.options["choices"] = choices
         return self
 
@@ -609,35 +609,29 @@
     def _postgethook(self, obj, value: _V) -> _V:
         return value
 
     def _presethook(self, obj, value: _V) -> _V:
         return value
 
     @overload
-    def with_choices(
-        self, choices: Sequence[tuple[str, _U]]
-    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+    def with_choices(self, choices: Sequence[tuple[str, _U]]) -> MagicValueField[_U]:
         ...
 
     @overload
-    def with_choices(
-        self, choices: Sequence[_U]
-    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+    def with_choices(self, choices: Sequence[_U]) -> MagicValueField[_U]:
         ...
 
     @overload
     def with_choices(
         self, choices: Callable[..., Sequence[tuple[str, _U]]]
-    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+    ) -> MagicValueField[_U]:
         ...
 
     @overload
-    def with_choices(
-        self, choices: Callable[..., Sequence[_U]]
-    ) -> MagicValueField[CategoricalWidget[_U], _U]:
+    def with_choices(self, choices: Callable[..., Sequence[_U]]) -> MagicValueField[_U]:
         ...
 
     def with_choices(self, choices):
         """Method to add choices to the field."""
         return super().with_choices(choices)
```

### Comparing `magic_class-0.7.0rc1/magicclass/fields/_group.py` & `magic_class-0.7.1/magicclass/fields/_group.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/fields/_property.py` & `magic_class-0.7.1/magicclass/fields/_property.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/functools/_dispatch.py` & `magic_class-0.7.1/magicclass/functools/_dispatch.py`

 * *Files 26% similar despite different names*

```diff
@@ -156,91 +156,28 @@
     def __signature__(self, sig):
         self.func.__signature__ = sig
 
     def __call__(self, *args: Any, **kwds: Any) -> Any:
         raise TypeError("singledispatchmethod must be called on an instance")
 
 
-class UnionWidget(TabbedContainer):
-    def __init__(
-        self,
-        annotations: list[type],
-        names: list[str] | None = None,
-        layout: str = "vertical",
-        labels: bool = False,
-        nullable: bool = False,
-        options: list[dict] | None = None,
-        value=Undefined,
-        **kwargs,
-    ):
-        if names is None:
-            names: list[str] = []
-            for ann in annotations:
-                if isinstance(ann, type):
-                    names.append(ann.__name__)
-                elif isinstance(ann, _AnnotatedAlias):
-                    _type, _options = split_annotated_type(ann)
-                    _name = _options.get("name", _type.__name__)
-                    names.append(_name)
-
-        if options is None:
-            options = [{}] * len(annotations)
-
-        widgets: list[Widget] = []
-        for ann, name, opt in zip(annotations, names, options):
-            _kwargs = dict(name=name, label="")
-            _kwargs.update(opt)
-            if isinstance(ann, _AnnotatedAlias):
-                ann, _options = split_annotated_type(ann)
-                _kwargs.update(_options)
-            wdt = create_widget(annotation=ann, options=_kwargs)
-            widgets.append(wdt)
-
-        if nullable:
-            widgets.append(Label(value="None", bind=None))
-
-        if "value" in kwargs:
-            value = kwargs.pop("value")
-
-        super().__init__(
-            layout=layout, widgets=widgets, labels=labels, scrollable=False, **kwargs
-        )
-
-        self._annotations = annotations
-        if value is not Undefined:
-            self.value = value
-
-    @property
-    def value(self):
-        idx = self.current_index
-        return self[idx].value  # type: ignore
-
-    @value.setter
-    def value(self, value):
-        _type = type(value)
-        for idx, ann in enumerate(self._annotations):
-            if _type is ann:
-                self[idx].value = value  # type: ignore
-                self.current_index = idx
-                break
-        else:
-            raise TypeError(f"Cannot set value of type {_type!r}.")
-
-
 def _merge_parameters(params: Sequence[inspect.Parameter]) -> MagicParameter:
+    from magicclass.widgets import UnionWidget
+
     annotations = []
     name = None
     for param in params:
         if param.annotation is MagicParameter.empty:
             # If the first dispatch is not annotated (i.e. the default behavior),
             # do not add an empty widget.
             continue
         if name is None:
             name = param.name
             default = param.default
         annotations.append(param.annotation)
+
     return MagicParameter(
         name=name,
         kind=MagicParameter.POSITIONAL_OR_KEYWORD,
         default=default,
         gui_options={"widget_type": UnionWidget, "annotations": annotations},
     )
```

### Comparing `magic_class-0.7.0rc1/magicclass/functools/_partial.py` & `magic_class-0.7.1/magicclass/functools/_partial.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/functools/_wraps.py` & `magic_class-0.7.1/magicclass/functools/_wraps.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/logging/core.py` & `magic_class-0.7.1/magicclass/logging/core.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/stylesheets/__init__.py` & `magic_class-0.7.1/magicclass/stylesheets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/types/__init__.py` & `magic_class-0.7.1/magicclass/types/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from ._choices import OneOf, SomeOf, Choices
 from ._const import (
     WidgetType,
     WidgetTypeStr,
     PopUpModeStr,
     ErrorModeStr,
     Color,
+    Colormap,
     MGUI_SIMPLE_TYPES,
 )
 from ._expr import ExprStr
 from ._optional import Optional
 from ._path import Path
 from ._union import Union
 
@@ -21,13 +22,14 @@
     "SomeOf",
     "Choices",
     "WidgetType",
     "WidgetTypeStr",
     "PopUpModeStr",
     "ErrorModeStr",
     "Color",
+    "Colormap",
     "MGUI_SIMPLE_TYPES",
     "ExprStr",
     "Optional",
     "Path",
     "Union",
 ]
```

### Comparing `magic_class-0.7.0rc1/magicclass/types/_bound.py` & `magic_class-0.7.1/magicclass/types/_bound.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/types/_choices.py` & `magic_class-0.7.1/magicclass/types/_choices.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/types/_const.py` & `magic_class-0.7.1/magicclass/types/_const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from enum import Enum
-from typing import Literal, Union, Iterable
+from typing import Literal, Union, Iterable, Dict
 import datetime
 import pathlib
 
 
 class WidgetType(Enum):
     none = "none"
     scrollable = "scrollable"
@@ -54,14 +54,15 @@
     "parentlast",
 ]
 
 
 ErrorModeStr = Literal["msgbox", "stderr", "stdout"]
 
 Color = Union[Iterable[float], str]
+Colormap = Dict[float, Color]
 
 MGUI_SIMPLE_TYPES = (
     Union[
         int,
         float,
         bool,
         str,
```

### Comparing `magic_class-0.7.0rc1/magicclass/types/_expr.py` & `magic_class-0.7.1/magicclass/types/_expr.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/types/_optional.py` & `magic_class-0.7.1/magicclass/types/_optional.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 import typing
 from typing import (
     TYPE_CHECKING,
     Any,
+    Generic,
     overload,
     TypeVar,
+    get_args,
+    get_origin,
 )
 from typing_extensions import Annotated, _AnnotatedAlias
 from magicclass.utils import is_type_like
 from magicclass.signature import split_annotated_type
 
 _T = TypeVar("_T")
 
@@ -35,16 +38,36 @@
         opt = dict(widget_type=OptionalWidget)
         if isinstance(value, _AnnotatedAlias):
             type0, opt0 = split_annotated_type(value)
             type_ = typing.Optional[type0]
             opt.update(annotation=type_, options=opt0)
             return Annotated[type_, opt]
         else:
-            opt.update(annotation=typing.Optional[value])
-            return Annotated[typing.Optional[value], opt]
+            value_unwrapped = _unwrap_annotated(value)
+            try:
+                new_annot = typing.Optional[value]
+            except TypeError:  # unhashable
+                new_annot = _FakeOptional[value]
+            opt.update(annotation=new_annot)
+            return Annotated[value_unwrapped, opt]
+
+
+def _unwrap_annotated(typ):
+    origin = get_origin(typ)
+    args = get_args(typ)
+    if origin is Annotated:
+        return args[0]
+    if origin is not None and args:
+        unwrapped = tuple(_unwrap_annotated(arg) for arg in args)
+        return origin[unwrapped]
+    return typ
+
+
+class _FakeOptional(Generic[_T]):
+    """This type is recognized as typing.Optional by OptionalWidget."""
 
 
 if TYPE_CHECKING:
     from typing import Optional
 else:
 
     class Optional(metaclass=_OptionalAlias):
```

### Comparing `magic_class-0.7.0rc1/magicclass/types/_path.py` & `magic_class-0.7.1/magicclass/types/_path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 from __future__ import annotations
 from abc import ABCMeta
 
 import pathlib
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    List,
-    Sequence,
-)
+from typing import TYPE_CHECKING, Any, Sequence
 from typing_extensions import Annotated
 
 
 if TYPE_CHECKING:
     from typing_extensions import Self
 
 
@@ -28,15 +23,15 @@
 
     def __subclasscheck__(cls, subclass: type) -> bool:
         return issubclass(subclass, pathlib.Path)
 
 
 class _AnnotatedMultiPathAlias(ABCMeta):
     def __getitem__(cls, filter: str) -> Self:
-        return Annotated[List[Path], {"mode": "rm", "filter": filter}]
+        return Annotated[list[Path], {"mode": "rm", "filter": filter}]
 
 
 class _Path(pathlib.Path, metaclass=_AnnotatedPathAlias):
     _file_edit_mode = "r"
 
 
 class _SavePath(_Path):
```

### Comparing `magic_class-0.7.0rc1/magicclass/types/_union.py` & `magic_class-0.7.1/magicclass/types/_union.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     @overload
     def __getitem__(
         cls, value: tuple[_T, _T1, _T2, _T3]
     ) -> typing.Union[_T, _T1, _T2, _T3]:
         ...
 
     def __getitem__(cls, value):
-        from magicclass.functools._dispatch import UnionWidget
+        from magicclass.widgets import UnionWidget
 
         annotations = []
         opt = dict(widget_type=UnionWidget, nullable=False, annotations=annotations)
         if isinstance(value, tuple):
             for val in value:
                 if val is not None:
                     annotations.append(val)
```

### Comparing `magic_class-0.7.0rc1/magicclass/utils/__init__.py` & `magic_class-0.7.1/magicclass/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/utils/_click.py` & `magic_class-0.7.1/magicclass/utils/_click.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/utils/_functions.py` & `magic_class-0.7.1/magicclass/utils/_functions.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/utils/_recent.py` & `magic_class-0.7.1/magicclass/utils/_recent.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,18 +41,18 @@
         Maximum number of history.
 
     Returns
     -------
     MenuGuiBase
         magicmenu object.
     """
-    from ..core import magicmenu
-    from .._gui import MagicTemplate
-    from ..wrappers import mark_on_called
-    from ..functools._partial import partial
+    from magicclass.core import magicmenu
+    from magicclass._gui import MagicTemplate
+    from magicclass.wrappers import mark_on_called
+    from magicclass.functools._partial import partial
 
     # dispatch text type
     if text is None:
         _make_text = _default_fmt
     elif isinstance(text, str):
         _make_text = text.format
     elif callable(text):
```

### Comparing `magic_class-0.7.0rc1/magicclass/utils/qt.py` & `magic_class-0.7.1/magicclass/utils/qt.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/utils/qthreading.py` & `magic_class-0.7.1/magicclass/utils/qthreading.py`

 * *Files 2% similar despite different names*

```diff
@@ -630,27 +630,28 @@
             def _run(*args, **kwargs):
                 with gui.macro.blocked():
                     out = self._func.__get__(gui)(*args, **kwargs)
                 return out
 
         worker = create_worker(
             _run,
-            _ignore_errors=self._ignore_errors,
+            _ignore_errors=True,  # NOTE: reraising is processed in _create_method
             _start_thread=False,
             *args,
             **kwargs,
         )
 
         return worker
 
     def _create_method(self, gui: BaseGui) -> Callable[_P, None]:
         from magicclass.fields import MagicField
 
         @wraps(self)
         def _create_worker(*args, **kwargs):
+            _is_non_blocking = self.button(gui).running
             # create a worker object
             worker = self._create_qt_worker(gui, *args, **kwargs)
             is_generator = isinstance(worker, GeneratorWorker)
             pbar = None
             if self._progress:
                 # prepare progress bar
                 _pbar = self._progress["pbar"]
@@ -685,29 +686,32 @@
 
                 if hasattr(pbar, "set_worker"):
                     # if _SupportProgress object support set_worker
                     pbar.set_worker(worker)
                 if hasattr(pbar, "set_title"):
                     pbar.set_title(self._func.__name__.replace("_", " "))
 
-            if self.button(gui).running:
+            if is_generator:
+
+                @worker.aborted.connect
+                def _on_abort():
+                    gui._error_mode.wrap_handler(Aborted.raise_, parent=gui)()
+                    gui.macro.active = True
+                    Aborted.raise_()
+
+            if _is_non_blocking:
 
                 @worker.errored.connect
                 def _on_error(err: Exception):
                     # NOTE: Exceptions are raised in other thread so context manager
                     # cannot catch them. Macro has to be reactived here.
                     gui._error_mode.get_handler()(err, parent=gui)
                     gui.macro.active = True
-
-                if is_generator:
-
-                    @worker.aborted.connect
-                    def _on_abort():
-                        gui._error_mode.wrap_handler(Aborted.raise_, parent=gui)()
-                        gui.macro.active = True
+                    if not self._ignore_errors:
+                        raise err  # reraise
 
                 worker.start()
             else:
                 # If function is called from script, some events must get processed by
                 # the application while keep script stopping at each line of code.
                 self._run_blocked(gui, worker, pbar)
 
@@ -719,28 +723,56 @@
     def _run_blocked(
         self,
         gui: BaseGui,
         worker: FunctionWorker | GeneratorWorker,
         pbar: ProgressBar | None,
     ):
         app = use_app()
+
+        if isinstance(pbar, DefaultProgressBar):
+            pbar.pause_button.enabled = False
         worker.started.connect(app.process_events)
         worker.finished.connect(app.process_events)
+
+        _empty = object()
+        result = err = _empty
+
+        @worker.returned.connect
+        def _(val):
+            nonlocal result
+            result = val
+
+        @worker.errored.connect
+        def _(exc):
+            nonlocal err
+            err = exc
+
+        if isinstance(worker, GeneratorWorker):
+
+            @worker.aborted.connect
+            def _():
+                nonlocal err
+                err = Aborted("Aborted.")
+
         if isinstance(worker, GeneratorWorker):
             worker.yielded.connect(app.process_events)
         try:
             worker.run()
 
-        except KeyboardInterrupt:
+        except KeyboardInterrupt as e:
             if isinstance(pbar, DefaultProgressBar):
                 pbar._abort_worker()
             else:
                 worker.quit()
             worker.finished.emit()
             gui._error_mode.wrap_handler(Aborted.raise_, parent=gui)()
+            raise e
+
+        if result is _empty and err is not _empty:
+            raise err
 
     def _get_method_signature(self) -> inspect.Signature:
         sig = self.__signature__
         params = list(sig.parameters.values())[1:]
         return sig.replace(parameters=params)
 
     def _bind_callbacks(
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/__init__.py` & `magic_class-0.7.1/magicclass/widgets/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,60 +15,60 @@
     SplitterContainer,
     StackedContainer,
     TabbedContainer,
     ToolBoxContainer,
 )
 from .pywidgets import ListWidget, DictWidget
 from .color import ColorEdit, ColorSlider
+from .colormap import ColormapEdit
 from .misc import (
     OptionalWidget,
     ConsoleTextEdit,
     CheckButton,
-    RangeSlider,
-    FloatRangeSlider,
     HistoryLineEdit,
     HistoryFileEdit,
     SpreadSheet,
 )
 from .plot import Figure, SeabornFigure
 from .separator import Separator
 from .utils import FreeWidget
 from .logger import Logger
 from .codeedit import CodeEdit
 from .toggle_switch import ToggleSwitch
 from .eval import EvalLineEdit
+from ._union import UnionWidget
 
 __all__ = [
     "ButtonContainer",
     "CodeEdit",
     "ColorEdit",
+    "ColormapEdit",
     "ColorSlider",
     "ConsoleTextEdit",
     "CheckButton",
     "CollapsibleContainer",
     "DictWidget",
     "DraggableContainer",
     "EvalLineEdit",
     "FrameContainer",
     "Figure",
-    "FloatRangeSlider",
     "FreeWidget",
     "GroupBoxContainer",
     "HCollapsibleContainer",
     "HistoryFileEdit",
     "HistoryLineEdit",
     "ListContainer",
     "ListWidget",
     "Logger",
     "OptionalWidget",
-    "RangeSlider",
     "SeabornFigure",
     "Separator",
     "ScrollableContainer",
     "SubWindowsContainer",
     "SplitterContainer",
     "SpreadSheet",
     "StackedContainer",
     "TabbedContainer",
     "ToggleSwitch",
     "ToolBoxContainer",
+    "UnionWidget",
 ]
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/_html.py` & `magic_class-0.7.1/magicclass/widgets/_html.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/_mpl_canvas.py` & `magic_class-0.7.1/magicclass/widgets/_mpl_canvas.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/codeedit.py` & `magic_class-0.7.1/magicclass/widgets/codeedit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+from contextlib import contextmanager
 import sys
 from typing import Any, Iterator, NamedTuple, TYPE_CHECKING
 import weakref
 from qtpy import QtWidgets as QtW, QtGui, QtCore
 from qtpy.QtCore import Qt, Signal as pyqtSignal
 
 from psygnal import Signal
@@ -426,33 +427,48 @@
         """Highlight syntax."""
         from superqt.utils import CodeSyntaxHighlight
 
         highlight = CodeSyntaxHighlight(self.document(), lang, theme=theme)
         self._highlight = highlight
         return None
 
+    @contextmanager
+    def _fix_horizontal_position(self):
+        hbar = self.horizontalScrollBar()
+        pos = hbar.value()
+        try:
+            yield
+        finally:
+            hbar.setValue(pos)
+
+    def appendPlainText(self, txt: str):
+        with self._fix_horizontal_position():
+            super().appendPlainText(txt)
+
     def eraseLast(self):
         """Erase the last line."""
-        cursor = self.textCursor()
-        cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
-        cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
-        cursor.removeSelectedText()
-        cursor.deletePreviousChar()
-        self.setTextCursor(cursor)
+        with self._fix_horizontal_position():
+            cursor = self.textCursor()
+            cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
+            cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
+            cursor.removeSelectedText()
+            cursor.deletePreviousChar()
+            self.setTextCursor(cursor)
 
     def eraseFirst(self):
         """Erase the first line."""
-        cursor = self.textCursor()
-        cursor.movePosition(QtGui.QTextCursor.MoveOperation.Start)
-        cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
-        cursor.removeSelectedText()
-        cursor.movePosition(QtGui.QTextCursor.MoveOperation.Down)
-        cursor.deletePreviousChar()
-        cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
-        self.setTextCursor(cursor)
+        with self._fix_horizontal_position():
+            cursor = self.textCursor()
+            cursor.movePosition(QtGui.QTextCursor.MoveOperation.Start)
+            cursor.select(QtGui.QTextCursor.SelectionType.LineUnderCursor)
+            cursor.removeSelectedText()
+            cursor.movePosition(QtGui.QTextCursor.MoveOperation.Down)
+            cursor.deletePreviousChar()
+            cursor.movePosition(QtGui.QTextCursor.MoveOperation.End)
+            self.setTextCursor(cursor)
 
     def selectedText(self) -> str:
         """Return selected string."""
         cursor = self.textCursor()
         return cursor.selectedText().replace("\u2029", "\n")
 
     def selectedLines(self) -> list[str]:
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/color.py` & `magic_class-0.7.1/magicclass/widgets/color.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,132 +1,161 @@
 from __future__ import annotations
-from typing import Iterable
-from qtpy.QtWidgets import (
-    QLineEdit,
-    QColorDialog,
-    QFrame,
-    QWidget,
-    QVBoxLayout,
-    QHBoxLayout,
-    QLabel,
-    QDoubleSpinBox,
-    QSlider,
-)
-from qtpy.QtGui import QColor
+from functools import lru_cache
+from typing import Any, Callable, Iterable
+from qtpy import QtGui, QtCore, QtWidgets as QtW
 from qtpy.QtCore import Qt, Signal as QtSignal
 
 from magicgui.widgets.bases import ValueWidget
 from magicgui.backends._qtpy.widgets import QBaseValueWidget
 from magicgui.application import use_app
 from .utils import merge_super_sigs
 
 
-def rgba_to_qcolor(rgba: Iterable[float]) -> QColor:
-    return QColor(*[int(round(255 * c)) for c in rgba])
-
-
-def qcolor_to_rgba(qcolor: QColor) -> tuple[float, float, float, float]:
-    return tuple(c / 255 for c in qcolor.getRgb())
-
-
 def rgba_to_html(rgba: Iterable[float]) -> str:
     code = "#" + "".join(hex(int(c * 255))[2:].upper().zfill(2) for c in rgba)
     if code.endswith("FF"):
         code = code[:-2]
     return code
 
 
 # modified from napari/_qt/widgets/qt_color_swatch.py
-class QColorSwatch(QFrame):
+class QColorSwatch(QtW.QFrame):
     colorChanged = QtSignal()
 
     def __init__(self, parent=None):
         super().__init__(parent)
         self.setCursor(Qt.CursorShape.PointingHandCursor)
         self._color: tuple[float, float, float, float] = (0.0, 0.0, 0.0, 0.0)
         self.colorChanged.connect(self._update_swatch_style)
         self.setMinimumWidth(40)
+        self._pressed_pos = None
+        self.setContextMenuPolicy(Qt.ContextMenuPolicy.CustomContextMenu)
+        self._tooltip = lambda: rgba_to_html(self.getQColor().getRgbF())
 
     def heightForWidth(self, w: int) -> int:
         return int(w * 0.667)
 
     def _update_swatch_style(self, _=None) -> None:
         rgba = f'rgba({",".join(str(int(x*255)) for x in self._color)})'
         self.setStyleSheet("QColorSwatch {background-color: " + rgba + ";}")
 
-    def mouseReleaseEvent(self, event):
+    def mousePressEvent(self, a0: QtGui.QMouseEvent) -> None:
+        self._pressed_pos = self.mapToGlobal(a0.pos())
+        return super().mousePressEvent(a0)
+
+    def mouseMoveEvent(self, a0: QtGui.QMouseEvent) -> None:
+        # moved?
+        if self._pressed_pos is not None:
+            pos = self.mapToGlobal(a0.pos())
+            dx = self._pressed_pos.x() - pos.x()
+            dy = self._pressed_pos.y() - pos.y()
+            if dx**2 + dy**2 > 4:
+                self._pressed_pos = None
+        return super().mouseMoveEvent(a0)
+
+    def mouseReleaseEvent(self, event: QtGui.QMouseEvent) -> None:
         """Show QColorPopup picker when the user clicks on the swatch."""
+        # inside the widget?
+        if self._pressed_pos is None or not self.rect().contains(event.pos()):
+            return None
         if event.button() == Qt.MouseButton.LeftButton:
             initial = self.getQColor()
-            dlg = QColorDialog(initial, self)
-            dlg.setOptions(QColorDialog.ColorDialogOption.ShowAlphaChannel)
+            dlg = QtW.QColorDialog(initial, self)
+            dlg.setOptions(QtW.QColorDialog.ColorDialogOption.ShowAlphaChannel)
             ok = dlg.exec_()
             if ok:
                 self.setColor(dlg.selectedColor())
+        self._pressed_pos = None
 
-    def getQColor(self) -> QColor:
-        return rgba_to_qcolor(self._color)
+    def getQColor(self) -> QtGui.QColor:
+        return QtGui.QColor.fromRgbF(*self._color)
 
-    def setColor(self, color: QColor) -> None:
+    def setColor(self, color: QtGui.QColor) -> None:
         old_color = rgba_to_html(self._color)
-        self._color = qcolor_to_rgba(color)
+        self._color = QtGui.QColor.getRgbF(color)
         if rgba_to_html(self._color) != old_color:
             self.colorChanged.emit()
 
+    def event(self, event: QtCore.QEvent) -> bool:
+        if event.type() == QtCore.QEvent.Type.ToolTip:
+            event = QtGui.QHelpEvent(event)
+            QtW.QToolTip.showText(event.globalPos(), self._tooltip(), self)
+            return True
+        return super().event(event)
+
+
+@lru_cache(maxsize=1)
+def _get_color_converter() -> Callable[[Any], tuple[float, float, float, float]]:
+    """Get a function that converts a color to a tuple of floats."""
+    import pkgutil
+
+    all_pkg = set(pkgutil.iter_importers())
+    if "cmap" in all_pkg:
+        import cmap
 
-class QColorLineEdit(QLineEdit):
-    def __init__(self, parent=None):
-        super().__init__(parent)
+        return lambda x: cmap.Color(x).rgba
+    elif "matplotlib" in all_pkg:
         import matplotlib.colors
 
-        self._color_converter = matplotlib.colors.to_rgba
+        return matplotlib.colors.to_rgba
+    elif "vispy" in all_pkg:
+        from vispy import color as vispycolor
+
+        return lambda x: tuple(vispycolor.Color(x).rgba)
+    else:
+        return lambda x: QtGui.QColor(x).getRgbF()
+
+
+class QColorLineEdit(QtW.QLineEdit):
+    def _color_converter(self, x):
+        return _get_color_converter()(x)
 
     def setText(self, color: str | Iterable[float]):
         """Set the text of the lineEdit using any ColorType.
 
         Colors will be converted to standard SVG spec names if possible,
         or shown as #RGBA hex if not.
 
         Parameters
         ----------
         color : ColorType
             Can be any ColorType recognized by our
             utils.colormaps.standardize_color.transform_color function.
         """
-        if isinstance(color, QColor):
-            color = rgba_to_html(qcolor_to_rgba(color))
+        if isinstance(color, QtGui.QColor):
+            color = rgba_to_html(QtGui.QColor.getRgbF(color))
         elif not isinstance(color, str):
             color = rgba_to_html(color)
 
         super().setText(color)
 
-    def getQColor(self) -> QColor:
-        """Get color as QColor object"""
+    def getQColor(self) -> QtGui.QColor:
+        """Get color as QtGui.QColor object"""
         rgba = self._color_converter(self.text())
-        return rgba_to_qcolor(rgba)
+        return QtGui.QColor.fromRgbF(*rgba)
 
-    def setColor(self, color: QColor | str):
+    def setColor(self, color: QtGui.QColor | str):
         if isinstance(color, str):
             color = self._color_converter(color)
-        elif isinstance(color, QColor):
-            color = qcolor_to_rgba(color)
+        elif isinstance(color, QtGui.QColor):
+            color = QtGui.QColor.getRgbF(color)
         code = "#" + "".join(
             hex(int(round(c * 255)))[2:].upper().zfill(2) for c in color
         )
         if code.endswith("FF"):
             code = code[:-2]
         self.setText(code)
 
 
-class QColorEdit(QWidget):
+class QColorEdit(QtW.QWidget):
     colorChanged = QtSignal(tuple)
 
     def __init__(self, parent=None, value: str = "white"):
         super().__init__(parent)
-        _layout = QHBoxLayout()
+        _layout = QtW.QHBoxLayout()
         self._color_swatch = QColorSwatch(self)
         self._line_edit = QColorLineEdit(self)
         _layout.addWidget(self._color_swatch)
         _layout.addWidget(self._line_edit)
         self.setLayout(_layout)
 
         self._color_swatch.colorChanged.connect(self._on_swatch_changed)
@@ -137,16 +166,16 @@
 
     def color(self):
         """Return the current color."""
         return self._color_swatch._color
 
     def setColor(self, color):
         """Set value as the current color."""
-        if isinstance(color, QColor):
-            color = qcolor_to_rgba(color)
+        if isinstance(color, QtGui.QColor):
+            color = QtGui.QColor.getRgbF(color)
         self._line_edit.setText(color)
         color = self._line_edit.getQColor()
         self._color_swatch.setColor(color)
 
     def _on_line_edit_edited(self, _=None):
         text = self._line_edit.text()
         try:
@@ -160,15 +189,15 @@
     def _on_swatch_changed(self, _=None):
         qcolor = self._color_swatch.getQColor()
         self._line_edit.setColor(qcolor)
         self.colorChanged.emit(self.color())
 
 
 # See https://stackoverflow.com/questions/42820380/use-float-for-qslider
-class QDoubleSlider(QSlider):
+class QDoubleSlider(QtW.QSlider):
     changed = QtSignal(float)
 
     def __init__(self, parent=None, decimals: int = 3):
         super().__init__(parent=parent)
         self.scale = 10**decimals
         self.setOrientation(Qt.Orientation.Horizontal)
         self.valueChanged.connect(self.doubleValueChanged)
@@ -192,23 +221,23 @@
     def singleStep(self):
         return float(super().singleStep()) / self.scale
 
     def setSingleStep(self, value):
         return super().setSingleStep(value * self.scale)
 
 
-class QColorSlider(QWidget):
+class QColorSlider(QtW.QWidget):
     colorChanged = QtSignal(tuple)
 
     def __init__(self, parent=None, value="white"):
         super().__init__(parent=parent)
         import matplotlib.colors
 
         self._color_converter = matplotlib.colors.to_rgba
-        _layout = QVBoxLayout()
+        _layout = QtW.QVBoxLayout()
         self.setLayout(_layout)
         _layout.setContentsMargins(0, 0, 0, 0)
         self._qsliders = [
             self.addSlider("R"),
             self.addSlider("G"),
             self.addSlider("B"),
             self.addSlider("A"),
@@ -219,41 +248,41 @@
         @self._color_edit._line_edit.editingFinished.connect
         def _read_color_str(e=None):
             self.setColor(self._color_edit._line_edit.getQColor())
 
         self._color_edit._color_swatch.setEnabled(False)
 
         @self.colorChanged.connect
-        def _set_color_swatch(color: QColor):
-            qcolor = rgba_to_qcolor(color)
+        def _set_color_swatch(color: QtGui.QColor):
+            qcolor = QtGui.QColor.fromRgbF(*color)
             self._color_edit._color_swatch.setColor(qcolor)
 
         _layout.addWidget(self._color_edit)
 
     def addSlider(self, label: str):
-        qlabel = QLabel(label)
+        qlabel = QtW.QLabel(label)
         qlabel.setFixedWidth(15)
         qslider = QDoubleSlider()
         qslider.setMaximum(1.0)
         qslider.setSingleStep(0.001)
-        qspinbox = QDoubleSpinBox()
+        qspinbox = QtW.QDoubleSpinBox()
         qspinbox.setMaximum(1.0)
         qspinbox.setSingleStep(0.001)
         qspinbox.setAlignment(Qt.AlignmentFlag.AlignRight)
 
-        qspinbox.setButtonSymbols(QDoubleSpinBox.ButtonSymbols.NoButtons)
+        qspinbox.setButtonSymbols(QtW.QDoubleSpinBox.ButtonSymbols.NoButtons)
         qspinbox.setStyleSheet("background:transparent; border: 0;")
 
         qslider.changed.connect(qspinbox.setValue)
         qslider.changed.connect(lambda e: self.setColor(self.color()))
         qspinbox.editingFinished.connect(qslider.setValue)
         qspinbox.editingFinished.connect(lambda e: self.setColor(qspinbox.text()))
 
-        _container = QWidget(self)
-        layout = QHBoxLayout()
+        _container = QtW.QWidget(self)
+        layout = QtW.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
         _container.setLayout(layout)
         layout.addWidget(qlabel)
         layout.addWidget(qslider)
         layout.addWidget(qspinbox)
 
         self.layout().addWidget(_container)
@@ -261,16 +290,16 @@
 
     def color(self):
         """Return the current color."""
         return tuple(sl.value() for sl in self._qsliders)
 
     def setColor(self, color):
         """Set value as the current color."""
-        if isinstance(color, QColor):
-            color = qcolor_to_rgba(color)
+        if isinstance(color, QtGui.QColor):
+            color = QtGui.QColor.getRgbF(color)
         elif isinstance(color, str):
             color = self._color_converter(color)
         self._color_edit.setColor(color)
         for sl, c in zip(self._qsliders, color):
             sl.setValue(c)
         self.colorChanged.emit(self.color())
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/containers.py` & `magic_class-0.7.1/magicclass/widgets/containers.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/eval.py` & `magic_class-0.7.1/magicclass/widgets/eval.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/logger.py` & `magic_class-0.7.1/magicclass/widgets/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 from typing import TYPE_CHECKING, Any, Union, overload, NamedTuple
 
 from magicclass.utils import rst_to_html
 
 if TYPE_CHECKING:
     import numpy as np
     from matplotlib.figure import Figure as mpl_Figure
+    from matplotlib.backend_bases import FigureManagerBase, RendererBase
+
 
 # See https://stackoverflow.com/questions/28655198/best-way-to-display-logs-in-pyqt
 
 
 # Variable "FigureCanvas" should globally updated to plot figure inside the logger
 # However, importing FigureCanvasAgg should be done lazily. Here's how to hack
 # this procedure.
@@ -59,56 +61,72 @@
     link: str
 
 
 Printable = Union[str, QtGui.QImage, linkedStr]
 # HREF_PATTERN = re.compile(r"<a href=.+>.+</a>")
 
 
-class QFinderWidget(QtW.QWidget):
-    def __init__(self):
-        super().__init__()
+class QFinderWidget(QtW.QDialog):
+    def __init__(self, parent: QtW.QWidget | None = None):
+        super().__init__(parent, Qt.WindowType.SubWindow)
         _layout = QtW.QHBoxLayout(self)
         _layout.setContentsMargins(2, 2, 2, 2)
         self.setLayout(_layout)
         _line = QtW.QLineEdit()
         _btn_prev = QtW.QPushButton("▲")
         _btn_next = QtW.QPushButton("▼")
-        _btn_prev.setFixedSize(20, 20)
-        _btn_next.setFixedSize(20, 20)
+        _btn_prev.setFixedSize(18, 18)
+        _btn_next.setFixedSize(18, 18)
         _layout.addWidget(_line)
         _layout.addWidget(_btn_prev)
         _layout.addWidget(_btn_next)
         _btn_prev.clicked.connect(self._find_prev)
         _btn_next.clicked.connect(self._find_next)
-        _line.editingFinished.connect(self._find_next)
+        _line.textChanged.connect(self._find_next)
         self._line_edit = _line
 
+    # fmt: off
     if TYPE_CHECKING:
+        def parentWidget(self) -> QtLogger: ...
+    # fmt: on
 
-        def parentWidget(self) -> QtLogger:
-            ...  # fmt: skip
+    def lineEdit(self) -> QtW.QLineEdit:
+        return self._line_edit
 
     def _find_prev(self):
+        text = self._line_edit.text()
+        if text == "":
+            return
         qlogger = self.parentWidget()
         flag = QtGui.QTextDocument.FindFlag.FindBackward
-        found = qlogger.find(self._line_edit.text(), flag)
+        found = qlogger.find(text, flag)
         if not found:
             qlogger.moveCursor(QtGui.QTextCursor.MoveOperation.End)
-            exists = qlogger.find(self._line_edit.text(), flag)
-            if not exists:
-                QtW.QMessageBox.information(self, "Find", "No text matches.")
+            qlogger.find(text, flag)
 
     def _find_next(self):
+        text = self._line_edit.text()
+        if text == "":
+            return
         qlogger = self.parentWidget()
-        found = qlogger.find(self._line_edit.text())
+        found = qlogger.find(text)
         if not found:
             qlogger.moveCursor(QtGui.QTextCursor.MoveOperation.Start)
-            exists = qlogger.find(self._line_edit.text())
-            if not exists:
-                QtW.QMessageBox.information(self, "Find", "No text matches.")
+            qlogger.find(text)
+
+    def keyPressEvent(self, a0: QtGui.QKeyEvent) -> None:
+        if a0.key() == Qt.Key.Key_Escape:
+            self.hide()
+            self.parentWidget().setFocus()
+        elif a0.key() in (Qt.Key.Key_Enter, Qt.Key.Key_Return):
+            if a0.modifiers() & Qt.KeyboardModifier.ShiftModifier:
+                self._find_prev()
+            else:
+                self._find_next()
+        return super().keyPressEvent(a0)
 
 
 class QtLogger(QtW.QTextEdit):
     process = Signal(tuple)
 
     def __init__(self, parent=None, max_history: int = 500):
         super().__init__(parent=parent)
@@ -205,43 +223,59 @@
         menu = QtW.QMenu(self)
         menu.addAction("Find ...", self._find_string)
         menu.addAction("Export as HTML", self._export_as_html)
         menu.addSeparator()
         if name := format.stringProperty(QtGui.QTextFormat.Property.ImageName):
             menu.addAction("Copy Image", lambda: self._copy_image(name))
             menu.addAction("Save Image As...", lambda: self._save_image(name))
-        if name := format.stringProperty(QtGui.QTextFormat.Property.AnchorName):
-            menu.addAction("Copy Link", lambda: self._copy_link(name))
         return menu
 
     def _copy_image(self, name):
         image = self._get_image(name)
+        if image is None:
+            raise ValueError("Image not found")
         return QtW.QApplication.clipboard().setImage(image)
 
     def _save_image(self, name, format="PNG"):
         """Shows a save dialog for the ImageResource with 'name'."""
+        image = self._get_image(name)
+        if image is None:
+            raise ValueError("Image not found")
         dialog = QtW.QFileDialog(self, "Save Image")
         dialog.setAcceptMode(QtW.QFileDialog.AcceptMode.AcceptSave)
         dialog.setDefaultSuffix(format.lower())
         if self._last_save_path is None:
             self._last_save_path = Path.cwd()
         dialog.setDirectory(str(self._last_save_path))
         dialog.setNameFilter(f"{format} file (*.{format.lower()})")
         if dialog.exec_():
             filename = dialog.selectedFiles()[0]
-            image = self._get_image(name)
             image.save(filename, format)
             self._last_save_path = Path(filename).parent
         return None
 
     def _find_string(self):
         if self._finder_widget is None:
-            self._finder_widget = QFinderWidget()
-        self._finder_widget.setParent(self, self.windowFlags())
+            self._finder_widget = QFinderWidget(self)
         self._finder_widget.show()
+        self._finder_widget.lineEdit().setFocus()
+        self._align_finder()
+
+    def resizeEvent(self, event):
+        if self._finder_widget is not None:
+            self._align_finder()
+        super().resizeEvent(event)
+
+    def _align_finder(self):
+        if fd := self._finder_widget:
+            vbar = self.verticalScrollBar()
+            if vbar.isVisible():
+                fd.move(self.width() - fd.width() - vbar.width() - 3, 5)
+            else:
+                fd.move(self.width() - fd.width() - 3, 5)
 
     def _export_as_html(self):
         from ._html import HtmlExporter
 
         HtmlExporter(self).export()
 
     def _get_image(self, name):
@@ -263,23 +297,32 @@
 
     def mouseMoveEvent(self, e: QtGui.QMouseEvent) -> None:
         super().mouseMoveEvent(e)
         _anchor = self.anchorAt(e.pos())
         self.viewport().setCursor(
             Qt.CursorShape.PointingHandCursor if _anchor else Qt.CursorShape.IBeamCursor
         )
-        return None
+        return super().mouseMoveEvent(e)
 
     def mouseReleaseEvent(self, e: QtGui.QMouseEvent):
-        _anchor = self.anchorAt(e.pos())
-        if self._anchor == _anchor:
-            QtGui.QDesktopServices.openUrl(QtCore.QUrl(self._anchor))
-        self._anchor = None
+        if e.button() == Qt.MouseButton.LeftButton:
+            _anchor = self.anchorAt(e.pos())
+            if self._anchor == _anchor:
+                QtGui.QDesktopServices.openUrl(QtCore.QUrl(self._anchor))
+            self._anchor = None
         return super().mouseReleaseEvent(e)
 
+    def keyPressEvent(self, e: QtGui.QKeyEvent):
+        mod = e.modifiers()
+        if mod == Qt.KeyboardModifier.ControlModifier:
+            if e.key() == Qt.Key.Key_F:
+                self._find_string()
+                return None
+        return super().keyPressEvent(e)
+
 
 class Logger(Widget, logging.Handler):
     """
     A widget for logging.
 
     Examples
     --------
@@ -449,22 +492,21 @@
         return None
 
     def print_link(self, text: str, href: str):
         """Print a link in the logger widget."""
         self.native.appendHref(text, href)
         return None
 
-    def print_figure(self, fig: mpl_Figure) -> None:
+    def print_figure(self, fig: mpl_Figure | FigureManagerBase) -> None:
         """Print matplotlib Figure object like inline plot."""
         import numpy as np
 
         fig.canvas.draw()
         data = np.asarray(fig.canvas.renderer.buffer_rgba(), dtype=np.uint8)
         self.print_image(data)
-
         return None
 
     def write(self, msg) -> None:
         """Handle the print event."""
         self.print(msg, end="")
         return None
 
@@ -529,14 +571,18 @@
 
         if style is None:
             try:
                 style = self._get_proper_plt_style()
             except RuntimeError:
                 style = "default"
 
+        if "figure.dpi" not in rc_context:
+            rc_context["figure.dpi"] = 800
+        if "figure.figsize" not in rc_context:
+            rc_context["figure.figsize"] = (4, 3)
         backend = mpl.get_backend()
         show._called = False
         try:
             mpl.use("module://magicclass.widgets.logger")
             with plt.style.context(style), plt.rc_context(rc_context):
                 yield self
         finally:
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/misc.py` & `magic_class-0.7.1/magicclass/widgets/misc.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,47 @@
 from __future__ import annotations
 from pathlib import Path
 import sys
 from typing import (
-    TYPE_CHECKING,
-    Generic,
     Iterable,
     MutableSequence,
     Any,
     TypeVar,
 )
 from typing_extensions import _AnnotatedAlias, get_args
-from psygnal import Signal
 from qtpy import QtWidgets as QtW, QtGui
 from qtpy.QtCore import Qt
 from magicgui.widgets import (
     PushButton,
     TextEdit,
     Table,
     Container,
     CheckBox,
     FileEdit,
     create_widget,
+    LineEdit,
 )
 from magicgui.application import use_app
-from magicgui.widgets import LineEdit
-from magicgui.types import FileDialogMode
-from magicgui.widgets.bases import ValueWidget
-from magicgui.types import Undefined
+from magicgui.types import FileDialogMode, Undefined
+from magicgui.widgets.bases import ValueWidget, RangedWidget
 from magicgui.backends._qtpy.widgets import (
-    QBaseWidget,
     QBaseStringWidget,
     LineEdit as BaseLineEdit,
 )
 from .utils import FreeWidget, merge_super_sigs
 from magicclass.signature import split_annotated_type
 
-if TYPE_CHECKING:
-    from qtpy.QtWidgets import QTextEdit
-    from superqt import QLabeledRangeSlider
-
+_W = TypeVar("_W", bound=ValueWidget)
 
 if sys.platform == "win32":
     _FONT = "Consolas"
-else:
+elif sys.platform == "darwin":
     _FONT = "Menlo"
+else:
+    _FONT = "Monospace"
 
 
 @merge_super_sigs
 class OptionalWidget(Container):
     """
     A container that can represent optional argument.
 
@@ -61,40 +55,39 @@
         Initial value.
     options : dict, optional
         Widget options of the inner value widget.
     """
 
     def __init__(
         self,
-        inner_widget: type[ValueWidget] | None = None,
+        inner_widget: _W | None = None,
         text: str | None = None,
         layout: str = "vertical",
         nullable: bool = True,
         value=Undefined,
         options: dict | None = None,
         **kwargs,
     ):
         if text is None:
             text = "Use default value"
-        if options is None:
-            options = {}
         self._checkbox = CheckBox(text=text, value=True)
 
         if inner_widget is None:
             annot = kwargs.get("annotation", None)
             if annot is None:
                 annot_arg = type(value)
             else:
                 args = get_args(annot)
                 if len(args) > 0:
                     annot_arg = args[0]
                 else:
                     annot_arg = type(value)
 
             if isinstance(annot_arg, _AnnotatedAlias):
+                options = options or {}
                 annot_arg, metadata = split_annotated_type(annot_arg)
                 options.update(metadata)
 
             self._inner_value_widget = create_widget(
                 annotation=annot_arg,
                 options=options,
             )
@@ -136,23 +129,57 @@
     def text(self) -> str:
         return self._checkbox.text
 
     @text.setter
     def text(self, v: str) -> None:
         self._checkbox.text = v
 
+    @property
+    def inner_widget(self) -> _W:
+        return self._inner_value_widget
+
+    @property
+    def min(self):
+        if isinstance(self.inner_widget, RangedWidget):
+            return self.inner_widget.min
+        raise AttributeError(f"Inner widget {self.inner_widget} has no attribute 'min'")
+
+    @min.setter
+    def min(self, v):
+        if isinstance(self.inner_widget, RangedWidget):
+            self.inner_widget.min = v
+        else:
+            raise AttributeError(
+                f"Inner widget {self.inner_widget} has no attribute 'min'"
+            )
+
+    @property
+    def max(self):
+        if isinstance(self.inner_widget, RangedWidget):
+            return self.inner_widget.max
+        raise AttributeError(f"Inner widget {self.inner_widget} has no attribute 'max'")
+
+    @max.setter
+    def max(self, v):
+        if isinstance(self.inner_widget, RangedWidget):
+            self.inner_widget.max = v
+        else:
+            raise AttributeError(
+                f"Inner widget {self.inner_widget} has no attribute 'max'"
+            )
+
 
 class ConsoleTextEdit(TextEdit):
     """A text edit with console-like setting."""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         from qtpy.QtGui import QFont, QTextOption
 
-        self.native: QTextEdit
+        self.native: QtW.QTextEdit
         font = QFont(_FONT)
         font.setStyleHint(QFont.StyleHint.Monospace)
         font.setFixedPitch(True)
         self.native.setFont(font)
         self.native.setWordWrapMode(QTextOption.WrapMode.NoWrap)
 
         # set tab width
@@ -260,145 +287,14 @@
             self,
             value=value,
             widget_type=QFloatEdit,
             **kwargs,
         )
 
 
-_V = TypeVar("_V")
-
-
-class QRangeSlider(QBaseWidget):
-    _qwidget: QLabeledRangeSlider
-
-    def _mgui_get_value(self):
-        pass
-
-    def _mgui_bind_change_callback(self, callback):
-        pass
-
-    def _mgui_set_value(self, rng):
-        pass
-
-
-class AbstractRangeSlider(ValueWidget, Generic[_V]):
-    """
-    A slider widget that represent a range like (2, 5).
-
-    This class is a temporary one and may be substituted by magicgui widget soon.
-    See https://github.com/napari/magicgui/pull/337.
-    """
-
-    changed = Signal(tuple)
-
-    def __init__(
-        self,
-        value=Undefined,
-        min=0,
-        max=1000,
-        orientation: str = "horizontal",
-        nullable: bool = True,
-        **kwargs,
-    ):
-        sl = self._construct_qt()
-        sl.setMinimum(min)
-        sl.setMaximum(max)
-        sl.valueChanged.connect(self.changed)
-        if orientation == "horizontal":
-            sl.setOrientation(Qt.Orientation.Horizontal)
-        elif orientation == "vertical":
-            sl.setOrientation(Qt.Orientation.Vertical)
-        else:
-            raise ValueError(
-                "Only horizontal and vertical orientation are currently supported"
-            )
-        self._slider = sl
-        super().__init__(
-            value=value,
-            widget_type=QRangeSlider,
-            backend_kwargs={"qwidg": QtW.QWidget},
-            **kwargs,
-        )
-        self.native.setLayout(QtW.QVBoxLayout())
-        self.native.setContentsMargins(0, 0, 0, 0)
-        self.native.layout().addWidget(sl)
-
-    @classmethod
-    def _construct_qt(cls, *args, **kwargs) -> QLabeledRangeSlider:
-        raise NotImplementedError()
-
-    @property
-    def value(self) -> tuple[_V, _V]:
-        return self._slider.value()
-
-    @value.setter
-    def value(self, rng: tuple[_V, _V]) -> None:
-        x0, x1 = rng
-        if x0 > x1:
-            raise ValueError(f"lower value exceeds higher value ({x0} > {x1}).")
-        self._slider.setValue((x0, x1))
-
-    @property
-    def range(self) -> tuple[_V, _V]:
-        return self._slider.minimum(), self._slider.maximum()
-
-    @range.setter
-    def range(self, rng: tuple[_V, _V]) -> None:
-        x0, x1 = rng
-        if x0 > x1:
-            raise ValueError(f"Minimum value exceeds maximum value ({x0} > {x1}).")
-        self._slider.setMinimum(x0)
-        self._slider.setMaximum(x1)
-
-    @property
-    def min(self) -> _V:
-        return self._slider.minimum()
-
-    @min.setter
-    def min(self, value: _V) -> None:
-        self._slider.setMinimum(value)
-
-    @property
-    def max(self) -> _V:
-        return self._slider.maximum()
-
-    @max.setter
-    def max(self, value: _V) -> None:
-        self._slider.setMaximum(value)
-
-
-class RangeSlider(AbstractRangeSlider[int]):
-    @classmethod
-    def _construct_qt(cls, *args, **kwargs):
-        from superqt import QLabeledRangeSlider
-
-        sl = QLabeledRangeSlider()
-        sl.setHandleLabelPosition(QLabeledRangeSlider.LabelPosition.LabelsAbove)
-        sl.setEdgeLabelMode(QLabeledRangeSlider.EdgeLabelMode.NoLabel)
-        return sl
-
-
-class FloatRangeSlider(AbstractRangeSlider[float]):
-    @classmethod
-    def _construct_qt(cls, *args, **kwargs):
-        from superqt import QLabeledDoubleRangeSlider
-
-        sl = QLabeledDoubleRangeSlider()
-        sl.setHandleLabelPosition(QLabeledDoubleRangeSlider.LabelPosition.LabelsAbove)
-        sl.setEdgeLabelMode(QLabeledDoubleRangeSlider.EdgeLabelMode.NoLabel)
-        return sl
-
-
-# magicgui>=0.6.0 has its own range sliders.
-try:
-    from magicgui.widgets import RangeSlider, FloatRangeSlider
-except ImportError:
-    pass
-
-
 class _QtSpreadSheet(QtW.QTabWidget):
     def __init__(self):
         super().__init__()
         self.setMovable(True)
         self._n_table = 0
         self.tabBar().tabBarDoubleClicked.connect(self.editTabBarLabel)
         self.tabBar().setContextMenuPolicy(Qt.CustomContextMenu)
@@ -533,19 +429,35 @@
         )
 
     def keyPressEvent(self, event: QtGui.QKeyEvent):
         if event.key() in (Qt.Key.Key_Down, Qt.Key.Key_Up):
             self.showPopup()
         super().keyPressEvent(event)
 
+    def wheelEvent(self, e: QtGui.QWheelEvent) -> None:
+        """Don't change the value when scrolling the mouse wheel."""
+        return None
+
     def _append_history(self, text: str):
         i = self.findText(text)
         if i >= 0:
             self.removeItem(i)
-        return self.addItem(text)
+        self.addItem(text)
+        if self.count() == 1:
+            self.setCurrentIndex(0)
+
+    def _pop_history(self, i: int):
+        nhist = self.count()
+        if i < 0:
+            i += nhist
+        if 0 <= i < nhist:
+            return self.removeItem(i)
+        raise IndexError(
+            f"Index {i} out of range. There are {nhist} items in the history."
+        )
 
 
 class QHistoryLineEdit(QBaseStringWidget):
     _qwidget: _QEditableComboBox
 
     def __init__(self, **kwargs):
         super().__init__(
@@ -564,18 +476,26 @@
         ValueWidget.__init__(
             self,
             value=value,
             widget_type=QHistoryLineEdit,
             **kwargs,
         )
 
-    def append_history(self, text: str):
+    def append_history(self, text: str) -> None:
         """Append new history to the line edit"""
         return self.native._append_history(text)
 
+    def pop_history(self, i: int):
+        """Pop history at index `i`"""
+        return self.native._pop_history(i)
+
+    def get_history(self) -> list[str]:
+        """Return the history as a list"""
+        return [self.native.itemText(i) for i in range(self.native.count())]
+
 
 class HistoryFileEdit(FileEdit):
     def __init__(
         self,
         mode: FileDialogMode = FileDialogMode.EXISTING_FILE,
         filter=None,
         nullable=False,
@@ -595,17 +515,33 @@
         Container.__init__(self, **kwargs)
         self.margins = (0, 0, 0, 0)
         self._show_file_dialog = use_app().get_obj("show_file_dialog")
         self.choose_btn.changed.disconnect()
         self.line_edit.changed.disconnect()
         self.choose_btn.changed.connect(self._on_choose_clicked)
         self.line_edit.changed.connect(lambda: self.changed.emit(self.value))
+        self._append_history_of_current()
 
-    def _on_choose_clicked(self):
-        super()._on_choose_clicked()
+    def _append_history_of_current(self):
         val = self.value
         if isinstance(val, (str, Path)):
             val = str(val)
             if val != ".":
                 self.line_edit.append_history(val)
         elif isinstance(val, tuple):
             self.line_edit.append_history("; ".join(map(str, val)))
+
+    def _on_choose_clicked(self):
+        super()._on_choose_clicked()
+        self._append_history_of_current()
+
+    def append_history(self, path: str | Path):
+        """Append new history to the line edit""" ""
+        return self.line_edit.append_history(path)
+
+    def pop_history(self, i: int):
+        """Pop history at index `i`"""
+        return self.line_edit.pop_history(i)
+
+    def get_history(self) -> list[Path]:
+        """Return the history as a list"""
+        return [Path(p) for p in self.line_edit.get_history()]
```

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/plot.py` & `magic_class-0.7.1/magicclass/widgets/plot.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/separator.py` & `magic_class-0.7.1/magicclass/widgets/separator.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/toggle_switch.py` & `magic_class-0.7.1/magicclass/widgets/toggle_switch.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/utils.py` & `magic_class-0.7.1/magicclass/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/__init__.py` & `magic_class-0.7.1/magicclass/widgets/pywidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/dict.py` & `magic_class-0.7.1/magicclass/widgets/pywidgets/dict.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/list.py` & `magic_class-0.7.1/magicclass/widgets/pywidgets/list.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/object.py` & `magic_class-0.7.1/magicclass/widgets/pywidgets/object.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/widgets/pywidgets/tree.py` & `magic_class-0.7.1/magicclass/widgets/pywidgets/tree.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/wrappers/__init__.py` & `magic_class-0.7.1/magicclass/wrappers/__init__.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/wrappers/_abstractapi.py` & `magic_class-0.7.1/magicclass/wrappers/_abstractapi.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/wrappers/_confirm.py` & `magic_class-0.7.1/magicclass/wrappers/_confirm.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/magicclass/wrappers/_misc.py` & `magic_class-0.7.1/magicclass/wrappers/_misc.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,21 +181,35 @@
 
 def bind_key(*key) -> Callable[[F], F]:
     """
     Define a keybinding to a button or an action.
     This function accepts several styles of shortcut expression.
 
     >>> @bind_key("Ctrl-A")         # napari style
-    >>> @bind_key("Ctrl", "A")      # separately
-    >>> @bind_key(Key.Ctrl + Key.A) # use Key class
-    >>> @bind_key(Key.Ctrl, Key.A)  # use Key class separately
+    >>> @bind_key("Ctrl+A")         # Qt style
+
+    >>> @bind_key("Ctrl+K, Ctrl+V") # Key combo
 
     """
-    if isinstance(key[0], tuple):
+    if len(key) == 1 and isinstance(key[0], str):
         key = key[0]
+        # check Ctrl-A style
+        lower = key.lower()
+        for k in ["ctrl", "cmd", "shift", "alt"]:
+            if f"{k}-" in lower:
+                lower = lower.replace(f"{k}-", f"{k}+")
+        key = lower
+    else:
+        warnings.warn(
+            "`bind_key` now accepts only one string argument. "
+            "Please use such as `bind_key('Ctrl+A')`.",
+            DeprecationWarning,
+        )
+        if isinstance(key[0], tuple):
+            key = key[0]
 
     def wrapper(method: F) -> F:
         upgrade_signature(method, additional_options={"keybinding": key})
         return method
 
     return wrapper
 
@@ -241,15 +255,15 @@
                 while self.__class__.__name__ != prev_ns:
                     self = self.__magicclass_parent__
                 return setup(self, mgui)
 
         else:
             _setup = setup
         upgrade_signature(target, additional_options={"setup": _setup})
-        upgrade_signature(setup, additional_options={"nogui": True})
+        upgrade_signature(setup, additional_options={"gui": False})
         return setup
 
     return wrapper
 
 
 _Fn = TypeVar("_Fn", bound=Callable[[FunctionGui], Any])
```

### Comparing `magic_class-0.7.0rc1/magicclass/wrappers/_preview.py` & `magic_class-0.7.1/magicclass/wrappers/_preview.py`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/.gitignore` & `magic_class-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/LICENSE` & `magic_class-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/README.md` & `magic_class-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `magic_class-0.7.0rc1/pyproject.toml` & `magic_class-0.7.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,23 @@
 [project]
 name = "magic-class"
 classifiers = [
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 description = "Generate multifunctional GUIs from classes"
 readme = "README.md"
 license = { file = "LICENSE" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 authors = [
     { name = "Hanjin Liu", email = "liuhanjin-sc@g.ecc.u-tokyo.ac.jp" },
 ]
 dependencies = [
     "macro-kit>=0.4.0",
     "magicgui>=0.7.0",
     "qtpy>=1.10.0",
```

### Comparing `magic_class-0.7.0rc1/PKG-INFO` & `magic_class-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magic-class
-Version: 0.7.0rc1
+Version: 0.7.1
 Summary: Generate multifunctional GUIs from classes
 Project-URL: Download, https://github.com/hanjinliu/magic-class
 Author-email: Hanjin Liu <liuhanjin-sc@g.ecc.u-tokyo.ac.jp>
 License: BSD 3-Clause License
         
         Copyright (c) 2021, hanjinliu
         All rights reserved.
@@ -34,19 +34,18 @@
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Requires-Dist: macro-kit>=0.4.0
 Requires-Dist: magicgui>=0.7.0
 Requires-Dist: qtpy>=1.10.0
 Requires-Dist: superqt>=0.4.0
 Provides-Extra: pyqt5
 Requires-Dist: pyqt5>=5.12.0; extra == 'pyqt5'
 Provides-Extra: pyqt6
```

