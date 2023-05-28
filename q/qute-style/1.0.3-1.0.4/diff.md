# Comparing `tmp/qute_style-1.0.3.tar.gz` & `tmp/qute_style-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qute_style-1.0.3.tar", max compression
+gzip compressed data, was "qute_style-1.0.4.tar", max compression
```

## Comparing `qute_style-1.0.3.tar` & `qute_style-1.0.4.tar`

### file list

```diff
@@ -1,148 +1,148 @@
--rw-r--r--   0        0        0     1087 2023-04-27 09:33:45.449041 qute_style-1.0.3/LICENSE
--rw-r--r--   0        0        0     5391 2023-04-27 09:33:45.449041 qute_style-1.0.3/README.md
--rw-r--r--   0        0        0     1042 2023-04-27 09:33:45.449041 qute_style-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/__init__.py
--rw-r--r--   0        0        0     6132 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/dev_functions.py
--rw-r--r--   0        0        0     8916 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/dev/mocks.py
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.449041 qute_style-1.0.3/qute_style/gen/__init__.py
--rw-r--r--   0        0        0    29831 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/gen/ui_test_window.py
--rw-r--r--   0        0        0     5330 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/gen/ui_whats_new_window.py
--rw-r--r--   0        0        0     1813 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/helper.py
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/py.typed
--rw-r--r--   0        0        0     8198 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_application.py
--rw-r--r--   0        0        0    29069 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_main_window.py
--rw-r--r--   0        0        0     6436 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qs_message_box.py
--rw-r--r--   0        0        0    26591 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/qute_style.py
--rw-r--r--   0        0        0      104 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/png_icons/transparent_icon.png
--rw-r--r--   0        0        0      466 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/accept.svg
--rw-r--r--   0        0        0     3012 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/accept_circle.svg
--rw-r--r--   0        0        0     2379 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/active_menu.svg
--rw-r--r--   0        0        0     2139 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/add.svg
--rw-r--r--   0        0        0     2160 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/add_circle.svg
--rw-r--r--   0        0        0     1939 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/admin.svg
--rw-r--r--   0        0        0     2721 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/admin_panel.svg
--rw-r--r--   0        0        0     2002 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_back.svg
--rw-r--r--   0        0        0      394 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_down.svg
--rw-r--r--   0        0        0      398 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/arrow_right.svg
--rw-r--r--   0        0        0     2004 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/block.svg
--rw-r--r--   0        0        0     3858 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/bug.svg
--rw-r--r--   0        0        0     2145 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/check_circle.svg
--rw-r--r--   0        0        0      208 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/checked.svg
--rw-r--r--   0        0        0      324 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/chevron_left.svg
--rw-r--r--   0        0        0      441 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/clipboard.svg
--rw-r--r--   0        0        0     2271 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/close.svg
--rw-r--r--   0        0        0     2289 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/close_circle.svg
--rw-r--r--   0        0        0      363 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/cloud_upload.svg
--rw-r--r--   0        0        0     2068 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/copy.svg
--rw-r--r--   0        0        0     2255 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/cps_trends.svg
--rw-r--r--   0        0        0     2019 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete.svg
--rw-r--r--   0        0        0      699 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete_forever.svg
--rw-r--r--   0        0        0     1928 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/delete_import.svg
--rw-r--r--   0        0        0     1881 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/document.svg
--rw-r--r--   0        0        0      785 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/document_scanner.svg
--rw-r--r--   0        0        0     1989 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/error.svg
--rw-r--r--   0        0        0     1575 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/expand_less.svg
--rw-r--r--   0        0        0     2062 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/expand_more.svg
--rw-r--r--   0        0        0     1961 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/file_distributor.svg
--rw-r--r--   0        0        0      482 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/filter.svg
--rw-r--r--   0        0        0     2023 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/folder_open.svg
--rw-r--r--   0        0        0     2880 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen.svg
--rw-r--r--   0        0        0     2877 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen_exit.svg
--rw-r--r--   0        0        0     2236 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/heart_broken.svg
--rw-r--r--   0        0        0     2642 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/help.svg
--rw-r--r--   0        0        0     2206 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/home.svg
--rw-r--r--   0        0        0     4370 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/ian_manager.svg
--rw-r--r--   0        0        0     4191 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/icon_PSE.svg
--rw-r--r--   0        0        0     2597 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/import.svg
--rw-r--r--   0        0        0     1939 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/info.svg
--rw-r--r--   0        0        0      491 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/inventory.svg
--rw-r--r--   0        0        0     2018 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/lidl_budget.svg
--rw-r--r--   0        0        0     2485 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/menu.svg
--rw-r--r--   0        0        0     1747 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/minimize.svg
--rw-r--r--   0        0        0     2498 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/nav_updater.svg
--rw-r--r--   0        0        0     2505 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/new_releases.svg
--rw-r--r--   0        0        0     2932 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/news.svg
--rw-r--r--   0        0        0     3184 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/no_icon.svg
--rw-r--r--   0        0        0     2214 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/package_commander.svg
--rw-r--r--   0        0        0     2475 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/palette.svg
--rw-r--r--   0        0        0     2709 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/pap.svg
--rw-r--r--   0        0        0      175 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/partial_checked.svg
--rw-r--r--   0        0        0     2236 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/protocol_creator.svg
--rw-r--r--   0        0        0      549 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/pzf_widget.svg
--rw-r--r--   0        0        0     3073 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/qt.svg
--rw-r--r--   0        0        0     2684 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/read_more.svg
--rw-r--r--   0        0        0     2468 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/refresh.svg
--rw-r--r--   0        0        0     1910 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/report_merger.svg
--rw-r--r--   0        0        0     2113 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/sap_excel.svg
--rw-r--r--   0        0        0     2244 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/save.svg
--rw-r--r--   0        0        0     2390 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/save_alt.svg
--rw-r--r--   0        0        0     2398 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/search.svg
--rw-r--r--   0        0        0     2103 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/send.svg
--rw-r--r--   0        0        0     3472 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/settings.svg
--rw-r--r--   0        0        0      184 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/status.svg
--rw-r--r--   0        0        0     2448 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/swap.svg
--rw-r--r--   0        0        0     2778 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/sync.svg
--rw-r--r--   0        0        0     2336 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/template_selector.svg
--rw-r--r--   0        0        0     2531 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/testbase_manager.svg
--rw-r--r--   0        0        0     1965 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/todo_circle.svg
--rw-r--r--   0        0        0     2257 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_icons/undo.svg
--rw-r--r--   0        0        0    32469 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/banner_qute_style.svg
--rw-r--r--   0        0        0     7237 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_chemistry.svg
--rw-r--r--   0        0        0     8429 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_labmonitor.svg
--rw-r--r--   0        0        0    39983 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_qute_style.svg
--rw-r--r--   0        0        0     8278 2023-04-27 09:33:45.453041 qute_style-1.0.3/qute_style/resources/svg_images/logo_toolbox.svg
--rw-r--r--   0        0        0   323159 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/resources_rc.py
--rw-r--r--   0        0        0     1657 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/startup_threads.py
--rw-r--r--   0        0        0    23017 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/style.py
--rw-r--r--   0        0        0    20664 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/ui/test_window.ui
--rw-r--r--   0        0        0     3001 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/ui/whats_new_window.ui
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/__init__.py
--rw-r--r--   0        0        0     1165 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/background_frame.py
--rw-r--r--   0        0        0     2967 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/base_widgets.py
--rw-r--r--   0        0        0     5533 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/color_manager.py
--rw-r--r--   0        0        0     1089 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/credit_bar.py
--rw-r--r--   0        0        0     4440 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/custom_icon_engine.py
--rw-r--r--   0        0        0      483 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/div.py
--rw-r--r--   0        0        0     1745 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/drop_label.py
--rw-r--r--   0        0        0     7164 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/grips.py
--rw-r--r--   0        0        0    16374 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/home_page.py
--rw-r--r--   0        0        0     2049 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon.py
--rw-r--r--   0        0        0     7697 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon_button.py
--rw-r--r--   0        0        0     3474 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/icon_tooltip_button.py
--rw-r--r--   0        0        0     6849 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_column.py
--rw-r--r--   0        0        0      808 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_column_close_button.py
--rw-r--r--   0        0        0     8775 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_menu.py
--rw-r--r--   0        0        0     7075 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/left_menu_button.py
--rw-r--r--   0        0        0    11127 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/spinner.py
--rw-r--r--   0        0        0    14486 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/styled_combobox.py
--rw-r--r--   0        0        0     1878 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/text_truncator.py
--rw-r--r--   0        0        0     6869 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/title_bar.py
--rw-r--r--   0        0        0     1733 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/title_button.py
--rw-r--r--   0        0        0     4334 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/toggle.py
--rw-r--r--   0        0        0     1046 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style/widgets/tooltip.py
--rw-r--r--   0        0        0        0 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/__init__.py
--rw-r--r--   0        0        0      136 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/__main__.py
--rw-r--r--   0        0        0    21042 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/example_images/color_manager.PNG
--rw-r--r--   0        0        0    79278 2023-04-27 09:33:45.457041 qute_style-1.0.3/qute_style_examples/example_images/custom_style.PNG
--rw-r--r--   0        0        0    62693 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/darcula.PNG
--rw-r--r--   0        0        0     3902 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/drop_label.PNG
--rw-r--r--   0        0        0    50435 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/highbridge_grey.PNG
--rw-r--r--   0        0        0     4594 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/information_messagebox.PNG
--rw-r--r--   0        0        0    30905 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/princesspink.PNG
--rw-r--r--   0        0        0    30041 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/rubyred.PNG
--rw-r--r--   0        0        0    30867 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/snowwhite.PNG
--rw-r--r--   0        0        0    56113 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/example_images/widgets_display.PNG
--rw-r--r--   0        0        0     2818 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/main.py
--rw-r--r--   0        0        0     1244 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_classes.py
--rw-r--r--   0        0        0     3414 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_main_window.py
--rw-r--r--   0        0        0     9665 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/sample_widgets.py
--rw-r--r--   0        0        0      110 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/1.json
--rw-r--r--   0        0        0      211 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/2.json
--rw-r--r--   0        0        0    45119 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.01/bug.png
--rw-r--r--   0        0        0      167 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/1.json
--rw-r--r--   0        0        0      209 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/2.json
--rw-r--r--   0        0        0    45119 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.10/bug.png
--rw-r--r--   0        0        0      114 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.100/1.json
--rw-r--r--   0        0        0       97 2023-04-27 09:33:45.461041 qute_style-1.0.3/qute_style_examples/test_changelog/1.100/2.json
--rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 qute_style-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1087 2023-05-28 23:21:36.931701 qute_style-1.0.4/LICENSE
+-rw-r--r--   0        0        0     5391 2023-05-28 23:21:36.931701 qute_style-1.0.4/README.md
+-rw-r--r--   0        0        0     1040 2023-05-28 23:21:36.931701 qute_style-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/dev/__init__.py
+-rw-r--r--   0        0        0     6132 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/dev/dev_functions.py
+-rw-r--r--   0        0        0     8916 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/dev/mocks.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/gen/__init__.py
+-rw-r--r--   0        0        0    29831 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/gen/ui_test_window.py
+-rw-r--r--   0        0        0     5330 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/gen/ui_whats_new_window.py
+-rw-r--r--   0        0        0     1813 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/helper.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/py.typed
+-rw-r--r--   0        0        0     8198 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/qs_application.py
+-rw-r--r--   0        0        0    29069 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/qs_main_window.py
+-rw-r--r--   0        0        0     6436 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/qs_message_box.py
+-rw-r--r--   0        0        0    26591 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/qute_style.py
+-rw-r--r--   0        0        0      104 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/png_icons/transparent_icon.png
+-rw-r--r--   0        0        0      466 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/accept.svg
+-rw-r--r--   0        0        0     3012 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/accept_circle.svg
+-rw-r--r--   0        0        0     2379 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/active_menu.svg
+-rw-r--r--   0        0        0     2139 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/add.svg
+-rw-r--r--   0        0        0     2160 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/add_circle.svg
+-rw-r--r--   0        0        0     1939 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/admin.svg
+-rw-r--r--   0        0        0     2721 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/admin_panel.svg
+-rw-r--r--   0        0        0     2002 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/arrow_back.svg
+-rw-r--r--   0        0        0      394 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/arrow_down.svg
+-rw-r--r--   0        0        0      398 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/arrow_right.svg
+-rw-r--r--   0        0        0     2004 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/block.svg
+-rw-r--r--   0        0        0     3858 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/bug.svg
+-rw-r--r--   0        0        0     2145 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/check_circle.svg
+-rw-r--r--   0        0        0      208 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/checked.svg
+-rw-r--r--   0        0        0      324 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/chevron_left.svg
+-rw-r--r--   0        0        0      441 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/clipboard.svg
+-rw-r--r--   0        0        0     2271 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/close.svg
+-rw-r--r--   0        0        0     2289 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/close_circle.svg
+-rw-r--r--   0        0        0      363 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/cloud_upload.svg
+-rw-r--r--   0        0        0     2068 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/copy.svg
+-rw-r--r--   0        0        0     2255 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/cps_trends.svg
+-rw-r--r--   0        0        0     2019 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/delete.svg
+-rw-r--r--   0        0        0      699 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/delete_forever.svg
+-rw-r--r--   0        0        0     1928 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/delete_import.svg
+-rw-r--r--   0        0        0     1881 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/document.svg
+-rw-r--r--   0        0        0      785 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/document_scanner.svg
+-rw-r--r--   0        0        0     1989 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/error.svg
+-rw-r--r--   0        0        0     1575 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/expand_less.svg
+-rw-r--r--   0        0        0     2062 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/expand_more.svg
+-rw-r--r--   0        0        0     1961 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/file_distributor.svg
+-rw-r--r--   0        0        0      482 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/filter.svg
+-rw-r--r--   0        0        0     2023 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/folder_open.svg
+-rw-r--r--   0        0        0     2880 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/fullscreen.svg
+-rw-r--r--   0        0        0     2877 2023-05-28 23:21:36.931701 qute_style-1.0.4/qute_style/resources/svg_icons/fullscreen_exit.svg
+-rw-r--r--   0        0        0     2236 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/heart_broken.svg
+-rw-r--r--   0        0        0     2642 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/help.svg
+-rw-r--r--   0        0        0     2206 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/home.svg
+-rw-r--r--   0        0        0     4370 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/ian_manager.svg
+-rw-r--r--   0        0        0     4191 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/icon_PSE.svg
+-rw-r--r--   0        0        0     2597 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/import.svg
+-rw-r--r--   0        0        0     1939 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/info.svg
+-rw-r--r--   0        0        0      491 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/inventory.svg
+-rw-r--r--   0        0        0     2018 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/lidl_budget.svg
+-rw-r--r--   0        0        0     2485 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/menu.svg
+-rw-r--r--   0        0        0     1747 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/minimize.svg
+-rw-r--r--   0        0        0     2498 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/nav_updater.svg
+-rw-r--r--   0        0        0     2505 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/new_releases.svg
+-rw-r--r--   0        0        0     2932 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/news.svg
+-rw-r--r--   0        0        0     3184 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/no_icon.svg
+-rw-r--r--   0        0        0     2214 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/package_commander.svg
+-rw-r--r--   0        0        0     2475 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/palette.svg
+-rw-r--r--   0        0        0     2709 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/pap.svg
+-rw-r--r--   0        0        0      175 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/partial_checked.svg
+-rw-r--r--   0        0        0     2236 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/protocol_creator.svg
+-rw-r--r--   0        0        0      549 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/pzf_widget.svg
+-rw-r--r--   0        0        0     3073 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/qt.svg
+-rw-r--r--   0        0        0     2684 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/read_more.svg
+-rw-r--r--   0        0        0     2468 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/refresh.svg
+-rw-r--r--   0        0        0     1910 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/report_merger.svg
+-rw-r--r--   0        0        0     2113 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/sap_excel.svg
+-rw-r--r--   0        0        0     2244 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/save.svg
+-rw-r--r--   0        0        0     2390 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/save_alt.svg
+-rw-r--r--   0        0        0     2398 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/search.svg
+-rw-r--r--   0        0        0     2103 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/send.svg
+-rw-r--r--   0        0        0     3472 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/settings.svg
+-rw-r--r--   0        0        0      184 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/status.svg
+-rw-r--r--   0        0        0     2448 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/swap.svg
+-rw-r--r--   0        0        0     2778 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/sync.svg
+-rw-r--r--   0        0        0     2336 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/template_selector.svg
+-rw-r--r--   0        0        0     2531 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/testbase_manager.svg
+-rw-r--r--   0        0        0     1965 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/todo_circle.svg
+-rw-r--r--   0        0        0     2257 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_icons/undo.svg
+-rw-r--r--   0        0        0    32469 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_images/banner_qute_style.svg
+-rw-r--r--   0        0        0     7237 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_images/logo_chemistry.svg
+-rw-r--r--   0        0        0     8429 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_images/logo_labmonitor.svg
+-rw-r--r--   0        0        0    39983 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_images/logo_qute_style.svg
+-rw-r--r--   0        0        0     8278 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources/svg_images/logo_toolbox.svg
+-rw-r--r--   0        0        0   323159 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/resources_rc.py
+-rw-r--r--   0        0        0     1657 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/startup_threads.py
+-rw-r--r--   0        0        0    23017 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/style.py
+-rw-r--r--   0        0        0    20664 2023-05-28 23:21:36.935701 qute_style-1.0.4/qute_style/ui/test_window.ui
+-rw-r--r--   0        0        0     3001 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/ui/whats_new_window.ui
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/__init__.py
+-rw-r--r--   0        0        0     1165 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/background_frame.py
+-rw-r--r--   0        0        0     2993 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/base_widgets.py
+-rw-r--r--   0        0        0     5533 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/color_manager.py
+-rw-r--r--   0        0        0     1089 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/credit_bar.py
+-rw-r--r--   0        0        0     4440 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/custom_icon_engine.py
+-rw-r--r--   0        0        0      483 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/div.py
+-rw-r--r--   0        0        0     1745 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/drop_label.py
+-rw-r--r--   0        0        0     7164 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/grips.py
+-rw-r--r--   0        0        0    16374 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/home_page.py
+-rw-r--r--   0        0        0     2049 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/icon.py
+-rw-r--r--   0        0        0     7697 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/icon_button.py
+-rw-r--r--   0        0        0     3474 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/icon_tooltip_button.py
+-rw-r--r--   0        0        0     6849 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/left_column.py
+-rw-r--r--   0        0        0      808 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/left_column_close_button.py
+-rw-r--r--   0        0        0     8775 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/left_menu.py
+-rw-r--r--   0        0        0     7075 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/left_menu_button.py
+-rw-r--r--   0        0        0    11127 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/spinner.py
+-rw-r--r--   0        0        0    14811 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/styled_combobox.py
+-rw-r--r--   0        0        0     1878 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/text_truncator.py
+-rw-r--r--   0        0        0     6869 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/title_bar.py
+-rw-r--r--   0        0        0     1733 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/title_button.py
+-rw-r--r--   0        0        0     4334 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/toggle.py
+-rw-r--r--   0        0        0     1046 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style/widgets/tooltip.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/__main__.py
+-rw-r--r--   0        0        0    21042 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/color_manager.PNG
+-rw-r--r--   0        0        0    79278 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/custom_style.PNG
+-rw-r--r--   0        0        0    62693 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/darcula.PNG
+-rw-r--r--   0        0        0     3902 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/drop_label.PNG
+-rw-r--r--   0        0        0    50435 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/highbridge_grey.PNG
+-rw-r--r--   0        0        0     4594 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/information_messagebox.PNG
+-rw-r--r--   0        0        0    30905 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/princesspink.PNG
+-rw-r--r--   0        0        0    30041 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/rubyred.PNG
+-rw-r--r--   0        0        0    30867 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/snowwhite.PNG
+-rw-r--r--   0        0        0    56113 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/example_images/widgets_display.PNG
+-rw-r--r--   0        0        0     2818 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/main.py
+-rw-r--r--   0        0        0     1244 2023-05-28 23:21:36.939701 qute_style-1.0.4/qute_style_examples/sample_classes.py
+-rw-r--r--   0        0        0     3414 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/sample_main_window.py
+-rw-r--r--   0        0        0     9665 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/sample_widgets.py
+-rw-r--r--   0        0        0      110 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.01/1.json
+-rw-r--r--   0        0        0      211 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.01/2.json
+-rw-r--r--   0        0        0    45119 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.01/bug.png
+-rw-r--r--   0        0        0      167 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.10/1.json
+-rw-r--r--   0        0        0      209 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.10/2.json
+-rw-r--r--   0        0        0    45119 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.10/bug.png
+-rw-r--r--   0        0        0      114 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.100/1.json
+-rw-r--r--   0        0        0       97 2023-05-28 23:21:36.943701 qute_style-1.0.4/qute_style_examples/test_changelog/1.100/2.json
+-rw-r--r--   0        0        0     6244 1970-01-01 00:00:00.000000 qute_style-1.0.4/PKG-INFO
```

### Comparing `qute_style-1.0.3/LICENSE` & `qute_style-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/README.md` & `qute_style-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/pyproject.toml` & `qute_style-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qute_style"
-version = "1.0.3"
+version = "1.0.4"
 description = "QuteStyle is an expandable application framework for PySide6"
 authors = ["Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke <PS-TF-Entwicklung@tuev-sued.de>"]
 readme = "README.md"
 repository = "https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle"
 license = "MIT"
 packages = [
     {include = "qute_style"},
@@ -14,25 +14,25 @@
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 PySide6 = "6.4.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "7.3.1"
 pytest-qt = "4.2.0"
-requests = "2.29.0"
+requests = "2.31.0"
 black = "23.3.0"
 coverage = "7.2.3"
 isort = "5.12.0"
 mypy = "1.2.0"
 pre-commit = "3.2.2"
 pydocstyle = "6.3.0"
 pylint = "^2.17.3"
 pytest-cov = "^4.0.0"
 pytest-github-actions-annotate-failures = "^0.1.8"
-types-requests = "2.28.11.17"
+types-requests = "2.31.0.0"
 
 
 [tool.poetry.scripts]
 qute-style-example = "qute_style_examples.main:main_method"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `qute_style-1.0.3/qute_style/dev/dev_functions.py` & `qute_style-1.0.4/qute_style/dev/dev_functions.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/dev/mocks.py` & `qute_style-1.0.4/qute_style/dev/mocks.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/gen/ui_test_window.py` & `qute_style-1.0.4/qute_style/gen/ui_test_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/gen/ui_whats_new_window.py` & `qute_style-1.0.4/qute_style/gen/ui_whats_new_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/helper.py` & `qute_style-1.0.4/qute_style/helper.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/qs_application.py` & `qute_style-1.0.4/qute_style/qs_application.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/qs_main_window.py` & `qute_style-1.0.4/qute_style/qs_main_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/qs_message_box.py` & `qute_style-1.0.4/qute_style/qs_message_box.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/qute_style.py` & `qute_style-1.0.4/qute_style/qute_style.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/accept_circle.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/accept_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/active_menu.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/active_menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/add.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/add.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/add_circle.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/add_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/admin.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/admin.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/admin_panel.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/admin_panel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/arrow_back.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/arrow_back.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/block.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/block.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/bug.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/bug.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/check_circle.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/check_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/close.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/close.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/close_circle.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/close_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/copy.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/copy.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/cps_trends.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/cps_trends.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/delete.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/delete.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/delete_forever.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/delete_forever.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/delete_import.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/delete_import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/document.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/document.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/document_scanner.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/document_scanner.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/error.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/error.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/expand_less.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/expand_less.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/expand_more.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/expand_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/file_distributor.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/file_distributor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/folder_open.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/folder_open.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/fullscreen.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/fullscreen_exit.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/fullscreen_exit.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/heart_broken.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/heart_broken.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/help.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/help.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/home.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/home.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/ian_manager.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/ian_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/icon_PSE.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/icon_PSE.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/import.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/import.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/info.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/info.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/lidl_budget.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/lidl_budget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/menu.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/menu.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/minimize.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/minimize.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/nav_updater.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/nav_updater.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/new_releases.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/new_releases.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/news.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/news.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/no_icon.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/no_icon.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/package_commander.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/package_commander.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/palette.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/palette.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/pap.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/pap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/protocol_creator.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/protocol_creator.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/pzf_widget.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/pzf_widget.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/qt.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/qt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/read_more.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/read_more.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/refresh.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/refresh.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/report_merger.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/report_merger.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/sap_excel.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/sap_excel.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/save.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/save.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/save_alt.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/save_alt.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/search.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/search.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/send.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/send.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/settings.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/settings.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/swap.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/swap.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/sync.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/sync.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/template_selector.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/template_selector.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/testbase_manager.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/testbase_manager.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/todo_circle.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/todo_circle.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_icons/undo.svg` & `qute_style-1.0.4/qute_style/resources/svg_icons/undo.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_images/banner_qute_style.svg` & `qute_style-1.0.4/qute_style/resources/svg_images/banner_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_images/logo_chemistry.svg` & `qute_style-1.0.4/qute_style/resources/svg_images/logo_chemistry.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_images/logo_labmonitor.svg` & `qute_style-1.0.4/qute_style/resources/svg_images/logo_labmonitor.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_images/logo_qute_style.svg` & `qute_style-1.0.4/qute_style/resources/svg_images/logo_qute_style.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources/svg_images/logo_toolbox.svg` & `qute_style-1.0.4/qute_style/resources/svg_images/logo_toolbox.svg`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/resources_rc.py` & `qute_style-1.0.4/qute_style/resources_rc.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/startup_threads.py` & `qute_style-1.0.4/qute_style/startup_threads.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/style.py` & `qute_style-1.0.4/qute_style/style.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/ui/test_window.ui` & `qute_style-1.0.4/qute_style/ui/test_window.ui`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/ui/whats_new_window.ui` & `qute_style-1.0.4/qute_style/ui/whats_new_window.ui`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/background_frame.py` & `qute_style-1.0.4/qute_style/widgets/background_frame.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/base_widgets.py` & `qute_style-1.0.4/qute_style/widgets/base_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,8 +91,8 @@
     def add_widget(self, widget: QWidget) -> None:
         """Add the given widget to the settings."""
         self._layout.addWidget(widget, 1, 0)
 
     def clear_widget(self) -> None:
         """Remove a widget from the settings if present."""
         if item := self._layout.itemAtPosition(1, 0):
-            item.widget().setParent(QWidget())
+            item.widget().setParent(None)  # type: ignore[call-overload]
```

### Comparing `qute_style-1.0.3/qute_style/widgets/color_manager.py` & `qute_style-1.0.4/qute_style/widgets/color_manager.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/credit_bar.py` & `qute_style-1.0.4/qute_style/widgets/credit_bar.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/custom_icon_engine.py` & `qute_style-1.0.4/qute_style/widgets/custom_icon_engine.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/drop_label.py` & `qute_style-1.0.4/qute_style/widgets/drop_label.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/grips.py` & `qute_style-1.0.4/qute_style/widgets/grips.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/home_page.py` & `qute_style-1.0.4/qute_style/widgets/home_page.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/icon.py` & `qute_style-1.0.4/qute_style/widgets/icon.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/icon_button.py` & `qute_style-1.0.4/qute_style/widgets/icon_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/icon_tooltip_button.py` & `qute_style-1.0.4/qute_style/widgets/icon_tooltip_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/left_column.py` & `qute_style-1.0.4/qute_style/widgets/left_column.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/left_column_close_button.py` & `qute_style-1.0.4/qute_style/widgets/left_column_close_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/left_menu.py` & `qute_style-1.0.4/qute_style/widgets/left_menu.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/left_menu_button.py` & `qute_style-1.0.4/qute_style/widgets/left_menu_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/spinner.py` & `qute_style-1.0.4/qute_style/widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/styled_combobox.py` & `qute_style-1.0.4/qute_style/widgets/styled_combobox.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,18 @@
         # corners of dropdowns cannot be drawn correctly
         self.view().window().setWindowFlags(
             Qt.WindowType.Popup | Qt.WindowType.FramelessWindowHint
         )
         self.view().window().setAttribute(
             Qt.WidgetAttribute.WA_TranslucentBackground
         )
+        # stop combobox contents from limiting width of whole application
+        self.setSizeAdjustPolicy(
+            QComboBox.SizeAdjustPolicy.AdjustToMinimumContentsLengthWithIcon
+        )
 
     def paintEvent(  # pylint: disable=invalid-name
         self, event: QtGui.QPaintEvent
     ) -> None:
         """Overwrite method to draw custom arrow."""
         # Draw ComboBox like defined in style sheet
         super().paintEvent(event)
@@ -232,32 +236,35 @@
                     index = self.model().index(idx, 0, QModelIndex())
                     self.model().setData(
                         index,
                         Qt.CheckState.Unchecked,
                         Qt.ItemDataRole.CheckStateRole,
                     )
         self.update_text()
-
-        current_state: dict[str | int, Qt.CheckState] = {
-            self.model().item(i).data(): (self.model().item(i).checkState())
-            for i in range(self.model().rowCount())
-        }
-        self.dataChanged.emit(current_state)
+        self.send_current_state()
 
     def update_text(self) -> None:
         """Update the texts."""
         text = self._get_text()
 
         # Compute elided text (with "...")
         metrics = QFontMetrics(self.lineEdit().font())
         elided_text = metrics.elidedText(
             text, Qt.TextElideMode.ElideRight, self.lineEdit().width()
         )
         self.lineEdit().setText(elided_text)
 
+    def send_current_state(self) -> None:
+        """Emit the current state via dataChanged."""
+        current_state: dict[str | int, Qt.CheckState] = {
+            self.model().item(i).data(): (self.model().item(i).checkState())
+            for i in range(self.model().rowCount())
+        }
+        self.dataChanged.emit(current_state)
+
     def _get_text(self) -> str:
         """Return the text that is shown at the top of the combobox."""
         texts = [
             str(cast(QStandardItemModel, self.model()).item(idx).data())
             for idx in range(self.model().rowCount())
             if cast(QStandardItemModel, self.model()).item(idx).checkState()
             == Qt.CheckState.Checked
```

### Comparing `qute_style-1.0.3/qute_style/widgets/text_truncator.py` & `qute_style-1.0.4/qute_style/widgets/text_truncator.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/title_bar.py` & `qute_style-1.0.4/qute_style/widgets/title_bar.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/title_button.py` & `qute_style-1.0.4/qute_style/widgets/title_button.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/toggle.py` & `qute_style-1.0.4/qute_style/widgets/toggle.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style/widgets/tooltip.py` & `qute_style-1.0.4/qute_style/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/color_manager.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/color_manager.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/custom_style.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/custom_style.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/darcula.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/darcula.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/drop_label.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/drop_label.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/highbridge_grey.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/highbridge_grey.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/information_messagebox.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/information_messagebox.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/princesspink.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/princesspink.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/rubyred.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/rubyred.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/snowwhite.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/snowwhite.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/example_images/widgets_display.PNG` & `qute_style-1.0.4/qute_style_examples/example_images/widgets_display.PNG`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/main.py` & `qute_style-1.0.4/qute_style_examples/main.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/sample_classes.py` & `qute_style-1.0.4/qute_style_examples/sample_classes.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/sample_main_window.py` & `qute_style-1.0.4/qute_style_examples/sample_main_window.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/sample_widgets.py` & `qute_style-1.0.4/qute_style_examples/sample_widgets.py`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/test_changelog/1.01/bug.png` & `qute_style-1.0.4/qute_style_examples/test_changelog/1.01/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/qute_style_examples/test_changelog/1.10/bug.png` & `qute_style-1.0.4/qute_style_examples/test_changelog/1.10/bug.png`

 * *Files identical despite different names*

### Comparing `qute_style-1.0.3/PKG-INFO` & `qute_style-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qute-style
-Version: 1.0.3
+Version: 1.0.4
 Summary: QuteStyle is an expandable application framework for PySide6
 Home-page: https://github.com/TUV-SUD-Product-Service-GmbH/QuteStyle
 License: MIT
 Author: Marina Baumgartner, Dairen Gonschior, Tilman Krummeck, Dennis Spitzhorn, Gerhard Trapp, Patrick Zwerschke
 Author-email: PS-TF-Entwicklung@tuev-sued.de
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

