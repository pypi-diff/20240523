# Comparing `tmp/pygubu_designer-0.39.2.tar.gz` & `tmp/pygubu_designer-0.39.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygubu_designer-0.39.2.tar", last modified: Sun May  5 20:00:11 2024, max compression
+gzip compressed data, was "pygubu_designer-0.39.3.tar", last modified: Thu May 23 02:59:17 2024, max compression
```

## Comparing `pygubu_designer-0.39.2.tar` & `pygubu_designer-0.39.3.tar`

### file list

```diff
@@ -1,768 +1,780 @@
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.038929 pygubu_designer-0.39.2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       67 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/AUTHORS
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5128 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/LEEME.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    35064 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/LICENSE.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/LISEZMOI.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      248 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/MANIFEST.in
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7714 2024-05-05 20:00:11.038929 pygubu_designer-0.39.2/PKG-INFO
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5020 2024-04-24 23:50:39.000000 pygubu_designer-0.39.2/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.526929 pygubu_designer-0.39.2/development/
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6434 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/create-imgs.py
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6977 2024-05-05 01:35:02.000000 pygubu_designer-0.39.2/development/dev-notes.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2186 2024-04-08 04:51:29.000000 pygubu_designer-0.39.2/development/devtool.py
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     3885 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/devtool.sh
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.526929 pygubu_designer-0.39.2/development/gettext/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1037 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/development/gettext/pygubu.its
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/development/gettext/pygubu.loc
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.530929 pygubu_designer-0.39.2/development/new-designer-icons/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2780 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/main.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.554929 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7010 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/button.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3744 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4072 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/canvas.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2101 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/combobox.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1252 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/default.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      665 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3834 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/entry.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6047 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/frame.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5074 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/label.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1666 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/labelframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6735 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/labelframe.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8598 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/menubutton.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      962 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook-tab.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3043 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook-tab.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1060 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3693 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      797 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      782 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3238 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1077 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/progressbar.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/rect848.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1786 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/spinbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/spinbutton.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/textview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6381 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/textview.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      867 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3229 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/toplevel.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1068 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview-col.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview-col.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      935 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4893 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2489 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/viewport.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7036 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/viewport.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4315 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/template.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/testnewicons.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/new-designer-icons/testnewiconsapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.570929 pygubu_designer-0.39.2/development/pygubuLogo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5501 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/Python-logo-notext.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu .ico
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   101863 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.icns
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.ico
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   175900 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.xcf
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)   124131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/pyGubu_newLogo.svg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       92 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/rootOfSVGs.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10232 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubuLogo/tcl-tk.svg
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/pygubudesigner_.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       11 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/development/requirements.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.578929 pygubu_designer-0.39.2/examples/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.578929 pygubu_designer-0.39.2/examples/7guis/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.578929 pygubu_designer-0.39.2/examples/7guis/01_counter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/01_counter/counter.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/01_counter/counterapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.578929 pygubu_designer-0.39.2/examples/7guis/02_temperature_converter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2687 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/02_temperature_converter/tempconv.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/02_temperature_converter/tempconvapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.582929 pygubu_designer-0.39.2/examples/7guis/03_flight_Booker/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/03_flight_Booker/flight_booker.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3212 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/03_flight_Booker/flightbookerapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.582929 pygubu_designer-0.39.2/examples/7guis/04_timer/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4089 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/04_timer/timer.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/04_timer/timerapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/7guis/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      546 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/binding.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      960 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/button_cb.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2053 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/button_cb.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.506929 pygubu_designer-0.39.2/examples/canvas/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.582929 pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      106 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5196 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      842 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/canvas_example.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.582929 pygubu_designer-0.39.2/examples/command_properties/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1221 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/command_properties/command_properties.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2641 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/command_properties/command_properties.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/command_properties/command_properties2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/commands.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    18575 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/commands.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.582929 pygubu_designer-0.39.2/examples/control_variables/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      584 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/control_variables/controlvariables.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3634 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/control_variables/controlvariables.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.586929 pygubu_designer-0.39.2/examples/custom_widget/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      436 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/custom_widget/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2029 2024-05-05 19:53:01.000000 pygubu_designer-0.39.2/examples/custom_widget/timer_main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      515 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/custom_widget/timerapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      687 2024-04-25 20:43:14.000000 pygubu_designer-0.39.2/examples/custom_widget/timerappui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      287 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/custom_widget/timerappwidgets.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3064 2024-04-25 20:53:04.000000 pygubu_designer-0.39.2/examples/custom_widget/timewidget.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2363 2024-04-25 20:50:52.000000 pygubu_designer-0.39.2/examples/custom_widget/timewidget_old.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.586929 pygubu_designer-0.39.2/examples/customtkinter/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/customtkinter/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.586929 pygubu_designer-0.39.2/examples/customtkinter/complex/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    22578 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/customtkinter/complex/complex_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/customtkinter/complex/complexdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.586929 pygubu_designer-0.39.2/examples/customtkinter/simple/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6284 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/customtkinter/simple/simple_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1269 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/customtkinter/simple/simpledemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.586929 pygubu_designer-0.39.2/examples/dialogs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       51 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.590929 pygubu_designer-0.39.2/examples/dialogs/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo1/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo1/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5699 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo1/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.590929 pygubu_designer-0.39.2/examples/dialogs/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       95 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo2/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo2/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4523 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo2/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.594929 pygubu_designer-0.39.2/examples/dialogs/demo3/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       98 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo3/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo3/demo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9704 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo3/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.594929 pygubu_designer-0.39.2/examples/dialogs/demo4/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      314 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo4/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.594929 pygubu_designer-0.39.2/examples/dialogs/demo4/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3373 2023-09-30 23:40:25.000000 pygubu_designer-0.39.2/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6987 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdemoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdialog.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1471 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/example_grid_rc.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1631 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/example_grid_rc_2.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.594929 pygubu_designer-0.39.2/examples/forms/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.598929 pygubu_designer-0.39.2/examples/forms/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1939 2024-04-13 02:37:32.000000 pygubu_designer-0.39.2/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2087 2024-02-04 03:08:22.000000 pygubu_designer-0.39.2/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1156 2024-02-14 15:19:49.000000 pygubu_designer-0.39.2/examples/forms/__pycache__/project_styles.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12310 2024-04-13 02:36:09.000000 pygubu_designer-0.39.2/examples/forms/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1635 2024-04-13 02:37:16.000000 pygubu_designer-0.39.2/examples/forms/formsdemo1app.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      796 2024-04-14 01:37:57.000000 pygubu_designer-0.39.2/examples/forms/formsdemo1appui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      635 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/examples/forms/project_styles.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      723 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/framepad.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.602929 pygubu_designer-0.39.2/examples/helloworld/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       82 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/helloworld/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      740 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/helloworld/helloworld.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/helloworld/helloworld.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/helloworld/holamundo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1176 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/helloworld/holamundo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.602929 pygubu_designer-0.39.2/examples/i18n_gettext_demo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2303 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.602929 pygubu_designer-0.39.2/examples/i18n_gettext_demo/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1237 2024-02-13 03:45:58.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11576 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/demo-i18n.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1251 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/i18n.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.602929 pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1433 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/demoapp.pot
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.506929 pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/es/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.602929 pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.606929 pygubu_designer-0.39.2/examples/image_property/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/image_property/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      710 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/image_property/image_property.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1682 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/image_property/image_property.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/image_property/red.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/image_property/yellow.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.606929 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      337 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.610929 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6612 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2529 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_cxFreeze/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.610929 pygubu_designer-0.39.2/examples/integration_with_nuitka/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      366 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.618929 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6510 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_nuitka/myapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.618929 pygubu_designer-0.39.2/examples/integration_with_py2exe/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      258 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.622929 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/myapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2731 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_py2exe/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.626929 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.630929 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/ps_circle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/ps_cross.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/ps_square.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2513 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.spec
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.630929 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      582 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.634929 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1141 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      526 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.638929 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1750 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      547 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.638929 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2190 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/main.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/myapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1975 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.638929 pygubu_designer-0.39.2/examples/integration_with_zipapp/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.510929 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.638929 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/__init__.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.642929 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3445 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.642929 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/extradata/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      556 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/info.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/red.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1013 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/main.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.642929 pygubu_designer-0.39.2/examples/jpg_image_on_canvas/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      825 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/jpg_image_on_canvas/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1244 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/jpg_image_on_canvas/demoapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       14 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/jpg_image_on_canvas/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    38211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/jpg_image_on_canvas/seaside400.jpg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3187 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/menubutton.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/menuexample.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/notebook/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/notebook/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/notebook/demo1app.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1835 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/panedwindow.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/panes_and_notebooks.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/pathchooserdemo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       32 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/pathchooserdemo/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/pathchooserdemo/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/pathchooserdemo/demo1/pathchooserdemo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3220 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/pathchooserdemo/demo1/pathchooserdemo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/pathchooserdemo/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/pathchooserdemo/demo2/pathchooserdemo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/pathchooserdemo/demo2/pathchooserdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1840 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/scrollbarhelper.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/scrolledframe/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/scrolledframe/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      646 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/scrolledframe/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12412 2024-02-14 15:17:08.000000 pygubu_designer-0.39.2/examples/scrolledframe/scrolledframe_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10765 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/scrolledframe-layouts.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9388 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/scrolledframe.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.646929 pygubu_designer-0.39.2/examples/scrolledtext/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4030 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/scrolledtext/scrolledtext_demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      977 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/scrolledtext/scrolledtextdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.650929 pygubu_designer-0.39.2/examples/static_image/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      539 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/static_image/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1676 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/static_image/demoapp.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23336 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/static_image/logo_253.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/static_image/requirements.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.510929 pygubu_designer-0.39.2/examples/text/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.650929 pygubu_designer-0.39.2/examples/text/logwindowdemo/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3075 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/text/logwindowdemo/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1714 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/text/logwindowdemo/demo1app.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.650929 pygubu_designer-0.39.2/examples/tk_window/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      144 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/tk_window/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/tk_window/green.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1354 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/tk_window/tkdemo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      600 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/tk_window/tkdemoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.654929 pygubu_designer-0.39.2/examples/toplevel_centered/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      154 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_centered/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1216 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_centered/centered_demo1.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_centered/centered_demo2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1020 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_centered/demo.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.654929 pygubu_designer-0.39.2/examples/toplevel_menu/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_menu/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_menu/menu.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2470 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/toplevel_menu/menu.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.654929 pygubu_designer-0.39.2/examples/treeview/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.654929 pygubu_designer-0.39.2/examples/treeview/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       43 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo1/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1496 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo1/treeview.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3473 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo1/treeview.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo2/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23736 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo2/columns_stretching.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2712 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview/demo2/columnsstretchingdemo.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview_editable/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       28 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_editable/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview_editable/demo1/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5044 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo1/demoapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo1/demoapp.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview_editable/demo2/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5944 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo2/demo2.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3432 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo2/demo2app.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview_editable/demo3/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      119 2024-05-04 02:36:40.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo3/README.md
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.658929 pygubu_designer-0.39.2/examples/treeview_editable/demo3/__pycache__/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2469 2024-05-04 02:17:34.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo3/__pycache__/demo3appui.cpython-311.pyc
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8944 2024-05-04 02:14:14.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5707 2024-05-04 02:36:40.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3app.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2024-05-04 02:36:40.000000 pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3appui.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.662929 pygubu_designer-0.39.2/examples/treeview_filterable/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       30 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_filterable/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5404 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_filterable/demo.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2886 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/treeview_filterable/demoapp.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.662929 pygubu_designer-0.39.2/examples/user_input/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/user_input/README.md
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/user_input/requirements.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    28967 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/user_input/userinput.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3730 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/user_input/userinputapp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/variables.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4346 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/vscrolledframe.ui
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.666929 pygubu_designer-0.39.2/examples/windowdeleteevent/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      887 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/windowdeleteevent/demo1.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/windowdeleteevent/demo1.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      847 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/windowdeleteevent/demo2.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/examples/windowdeleteevent/demo2.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    88292 2024-04-10 03:51:03.000000 pygubu_designer-0.39.2/pygubu-designer.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2436 2024-05-05 19:46:24.000000 pygubu_designer-0.39.2/pyproject.toml
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       38 2024-05-05 20:00:11.038929 pygubu_designer-0.39.2/setup.cfg
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/setup.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.034929 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7714 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/PKG-INFO
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    37228 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/SOURCES.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        1 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/dependency_links.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       65 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/entry_points.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      445 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/requires.txt
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       15 2024-05-05 20:00:10.000000 pygubu_designer-0.39.2/src/pygubu_designer.egg-info/top_level.txt
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.670929 pygubu_designer-0.39.2/src/pygubudesigner/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      200 2024-05-05 19:46:07.000000 pygubu_designer-0.39.2/src/pygubudesigner/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/__main__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1049 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/actions.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6373 2024-03-12 19:01:57.000000 pygubu_designer-0.39.2/src/pygubudesigner/bindingseditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.670929 pygubu_designer-0.39.2/src/pygubudesigner/codegen/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       76 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/codegen/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    19333 2024-04-08 01:37:06.000000 pygubu_designer-0.39.2/src/pygubudesigner/codegen/codebuilder.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12401 2024-05-05 01:26:06.000000 pygubu_designer-0.39.2/src/pygubudesigner/codegen/scriptgenerator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11044 2024-03-12 19:01:57.000000 pygubu_designer-0.39.2/src/pygubudesigner/containerlayouteditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.518929 pygubu_designer-0.39.2/src/pygubudesigner/data/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.674929 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2992 2024-03-13 03:14:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/app.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      907 2024-05-05 00:30:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/appuser.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      371 2024-05-05 00:29:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/base.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1620 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/customstyles.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2116 2024-04-08 02:11:56.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/script.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      474 2024-04-12 03:50:58.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/scriptuser.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      771 2024-04-08 02:22:55.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widget.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      542 2024-03-06 04:13:52.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widgetbo.py.mako
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      655 2024-04-12 03:59:49.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widgetuser.py.mako
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.694929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       70 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       71 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/bin-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       85 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/close.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/download3-16.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/download3-32.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      230 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/mglass.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/property_invalid.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/pygubu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/pygubu200.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.754929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      352 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      128 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      224 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      231 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       75 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1120 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      100 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      109 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.838929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      132 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      599 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      195 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      114 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.838929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      592 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      567 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      357 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.846929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      194 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/arrow-left2.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      184 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/arrow-right2.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      162 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/bin-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      353 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/circle-left.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      333 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/circle-right.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      170 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/download3-16.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      214 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/download3-32.png
--rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      316 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/mglass.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      603 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/property_invalid.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/pygubu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    15896 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/pygubu200.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.930929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      527 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      433 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      325 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      435 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      545 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      293 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.006929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      689 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      202 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      323 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.010929 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      705 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      619 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      611 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      673 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.010929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/de/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.014929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/de/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3172 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      425 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.014929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13309 2024-04-22 01:09:43.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    58879 2024-04-22 00:44:13.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/pygubu-designer.pot
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    20171 2024-04-22 00:44:13.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/pygubu.pot
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/tr/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.014929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4815 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      393 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.014929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    53166 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10936 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:10.514929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.018929 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    52658 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10937 2024-04-22 01:08:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.026929 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13872 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/about_dialog.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10318 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/container_layout_editor_base.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    16121 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/designer_settings.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4093 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/messagebox.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    45719 2024-04-12 04:11:16.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/project_settings.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    49541 2024-04-20 01:39:30.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/pygubu-ui.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2024-04-09 23:44:02.000000 pygubu_designer-0.39.2/src/pygubudesigner/data/ui/treecomponent_palette.ui
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4326 2024-04-15 03:30:30.000000 pygubu_designer-0.39.2/src/pygubudesigner/designerstyles.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2525 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/dialogs.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/i18n.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8476 2024-03-19 19:06:18.000000 pygubu_designer-0.39.2/src/pygubudesigner/layouteditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2688 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/logpanel.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    34307 2024-04-20 01:39:30.000000 pygubu_designer-0.39.2/src/pygubudesigner/main.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4418 2024-04-06 02:39:05.000000 pygubu_designer-0.39.2/src/pygubudesigner/preferences.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.026929 pygubu_designer-0.39.2/src/pygubudesigner/preview/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)       63 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/preview/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2664 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/preview/builder.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13624 2024-04-02 02:28:06.000000 pygubu_designer-0.39.2/src/pygubudesigner/preview/helper.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    17119 2024-04-01 04:38:44.000000 pygubu_designer-0.39.2/src/pygubudesigner/preview/preview.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.026929 pygubu_designer-0.39.2/src/pygubudesigner/properties/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      373 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/__init__.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.026929 pygubu_designer-0.39.2/src/pygubudesigner/properties/editors/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/editors/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1027 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/editors/forms.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1866 2024-02-17 03:46:34.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/manager.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    50538 2024-04-11 03:47:20.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/predefined.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    31209 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/properties/propertieshelp.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5528 2024-04-14 01:38:41.000000 pygubu_designer-0.39.2/src/pygubudesigner/propertieseditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1915 2024-04-07 01:08:23.000000 pygubu_designer-0.39.2/src/pygubudesigner/rfilemanager.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.030929 pygubu_designer-0.39.2/src/pygubudesigner/services/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1854 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/aboutdialog.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      982 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/aboutdialogui.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.030929 pygubu_designer-0.39.2/src/pygubudesigner/services/builders/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/builders/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3356 2024-03-31 01:41:21.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/designersettings.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      931 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/designersettingsui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2733 2024-04-14 22:42:58.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/fieldvalidator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1945 2024-03-07 01:08:46.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/messagebox.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      843 2024-03-07 01:11:22.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/messageboxui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4292 2024-05-05 07:26:13.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/project.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12314 2024-05-05 05:09:57.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/projectsettings.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1821 2024-04-12 04:13:44.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/projectsettingsui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6301 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/stylehandler.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4220 2024-03-31 23:43:45.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/theming.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.030929 pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5799 2024-04-08 02:37:37.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/treecomponentpalette.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      450 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/treecomponentpalettebo.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3465 2024-04-08 03:06:36.000000 pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/treecomponentpaletteui.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    59403 2024-05-04 03:38:11.000000 pygubu_designer-0.39.2/src/pygubudesigner/uitreeeditor.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.030929 pygubu_designer-0.39.2/src/pygubudesigner/util/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2823 2024-04-01 01:31:03.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4297 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/gridcalculator.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1964 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/keyboard.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/observable.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1289 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/screens.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/util/selecttool.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8344 2024-04-14 01:38:14.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgetdescr.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.034929 pygubu_designer-0.39.2/src/pygubudesigner/widgets/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/__init__.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3063 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/bindingeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3502 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/colorentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/commandentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3943 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/componentpalette.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/containerlayouteditorbase.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1640 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/cursorentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2681 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/dimensionentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2282 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/dynamicpropeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8250 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/fontentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10193 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/gridselector.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2491 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/imageentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3046 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/namedideditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2102 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/pixelcoordinateentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11940 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/propertyeditor.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3059 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/relativeentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/stickyentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3255 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/tkvarentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5936 2024-02-25 22:14:08.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/toolbarframe.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2650 2024-04-02 02:52:39.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/ttkstyleentry.py
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2536 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/src/pygubudesigner/widgets/whentry.py
-drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-05 20:00:11.034929 pygubu_designer-0.39.2/tests/
--rw-r--r--   0 aautalan  (1001) aautalan  (1001)      562 2023-09-09 20:40:32.000000 pygubu_designer-0.39.2/tests/test_plugin_init.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.075342 pygubu_designer-0.39.3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       67 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/AUTHORS
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5123 2024-05-23 02:11:21.000000 pygubu_designer-0.39.3/LEEME.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    35064 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/LICENSE.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/LISEZMOI.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      248 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/MANIFEST.in
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7659 2024-05-23 02:59:17.075342 pygubu_designer-0.39.3/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5014 2024-05-23 02:10:53.000000 pygubu_designer-0.39.3/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.219350 pygubu_designer-0.39.3/development/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6434 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/create-imgs.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     6977 2024-05-05 01:35:02.000000 pygubu_designer-0.39.3/development/dev-notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2186 2024-04-08 04:51:29.000000 pygubu_designer-0.39.3/development/devtool.py
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)     3885 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/devtool.sh
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.223350 pygubu_designer-0.39.3/development/gettext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1037 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/development/gettext/pygubu.its
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/development/gettext/pygubu.loc
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.223350 pygubu_designer-0.39.3/development/new-designer-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2780 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.267349 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7010 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/button.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3744 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4072 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/canvas.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2101 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/combobox.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1252 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/default.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      665 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3834 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/entry.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6047 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/frame.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5074 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/label.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1666 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/labelframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6735 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/labelframe.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8598 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/menubutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      962 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook-tab.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3043 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook-tab.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1060 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3693 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      797 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      782 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3238 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1077 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/progressbar.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/rect848.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1786 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/spinbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/spinbutton.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/textview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6381 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/textview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      867 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3229 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/toplevel.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1068 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview-col.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5481 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview-col.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      935 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4893 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2489 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/viewport.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7036 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/viewport.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4315 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/template.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7552 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/testnewicons.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/new-designer-icons/testnewiconsapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.287349 pygubu_designer-0.39.3/development/pygubuLogo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5501 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/Python-logo-notext.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu .ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   101863 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.icns
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   174121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.ico
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   175900 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.xcf
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)   124131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/pyGubu_newLogo.svg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       92 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/rootOfSVGs.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10232 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubuLogo/tcl-tk.svg
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/pygubudesigner_.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       11 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/development/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.299349 pygubu_designer-0.39.3/examples/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.303349 pygubu_designer-0.39.3/examples/7guis/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.303349 pygubu_designer-0.39.3/examples/7guis/01_counter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/01_counter/counter.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/01_counter/counterapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.303349 pygubu_designer-0.39.3/examples/7guis/02_temperature_converter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2687 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/02_temperature_converter/tempconv.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/02_temperature_converter/tempconvapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.303349 pygubu_designer-0.39.3/examples/7guis/03_flight_Booker/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2648 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/03_flight_Booker/flight_booker.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3212 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/03_flight_Booker/flightbookerapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.307349 pygubu_designer-0.39.3/examples/7guis/04_timer/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4089 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/04_timer/timer.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/04_timer/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/7guis/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      546 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/binding.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      960 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/button_cb.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2053 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/button_cb.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.199350 pygubu_designer-0.39.3/examples/canvas/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.307349 pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      106 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5196 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      842 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/canvas_example.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.311349 pygubu_designer-0.39.3/examples/command_properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1221 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/command_properties/command_properties.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2641 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/command_properties/command_properties.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1256 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/command_properties/command_properties2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/commands.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    18575 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/commands.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.311349 pygubu_designer-0.39.3/examples/control_variables/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      584 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/control_variables/controlvariables.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3634 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/control_variables/controlvariables.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.327349 pygubu_designer-0.39.3/examples/custom_widget/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      436 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/custom_widget/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2029 2024-05-23 02:54:14.000000 pygubu_designer-0.39.3/examples/custom_widget/timer_main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      515 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/custom_widget/timerapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      687 2024-04-25 20:43:14.000000 pygubu_designer-0.39.3/examples/custom_widget/timerappui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      287 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/custom_widget/timerappwidgets.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3064 2024-04-25 20:53:04.000000 pygubu_designer-0.39.3/examples/custom_widget/timewidget.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2363 2024-04-25 20:50:52.000000 pygubu_designer-0.39.3/examples/custom_widget/timewidget_old.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.327349 pygubu_designer-0.39.3/examples/customtkinter/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/customtkinter/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.327349 pygubu_designer-0.39.3/examples/customtkinter/complex/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    22578 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/customtkinter/complex/complex_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/customtkinter/complex/complexdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.331349 pygubu_designer-0.39.3/examples/customtkinter/simple/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6284 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/customtkinter/simple/simple_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1269 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/customtkinter/simple/simpledemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.331349 pygubu_designer-0.39.3/examples/dialogs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       51 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.339349 pygubu_designer-0.39.3/examples/dialogs/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo1/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5699 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo1/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.343349 pygubu_designer-0.39.3/examples/dialogs/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       95 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo2/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4523 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo2/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.347349 pygubu_designer-0.39.3/examples/dialogs/demo3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       98 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo3/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo3/demo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9704 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo3/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.351348 pygubu_designer-0.39.3/examples/dialogs/demo4/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      314 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo4/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.351348 pygubu_designer-0.39.3/examples/dialogs/demo4/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3373 2023-09-30 23:40:25.000000 pygubu_designer-0.39.3/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6987 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdemoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1319 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdialog.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.363348 pygubu_designer-0.39.3/examples/dialogs/demo5/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      346 2024-05-22 22:03:26.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.375348 pygubu_designer-0.39.3/examples/dialogs/demo5/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1558 2024-05-22 22:06:39.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/__pycache__/dialog1.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1941 2024-05-22 22:06:39.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/__pycache__/dialog1ui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2196 2024-05-22 21:43:07.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/__pycache__/mainappui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      554 2024-05-22 22:05:48.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/dialog1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3705 2024-05-22 21:36:05.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/dialog1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      778 2024-05-22 21:47:13.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/dialog1ui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      749 2024-05-22 21:34:34.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/mainapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4193 2024-05-22 21:31:28.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/mainapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      904 2024-05-22 21:42:47.000000 pygubu_designer-0.39.3/examples/dialogs/demo5/mainappui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1471 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/example_grid_rc.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1631 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/example_grid_rc_2.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.391348 pygubu_designer-0.39.3/examples/forms/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.415348 pygubu_designer-0.39.3/examples/forms/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1939 2024-04-13 02:37:32.000000 pygubu_designer-0.39.3/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2087 2024-02-04 03:08:22.000000 pygubu_designer-0.39.3/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1156 2024-02-14 15:19:49.000000 pygubu_designer-0.39.3/examples/forms/__pycache__/project_styles.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12310 2024-04-13 02:36:09.000000 pygubu_designer-0.39.3/examples/forms/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1635 2024-04-13 02:37:16.000000 pygubu_designer-0.39.3/examples/forms/formsdemo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      796 2024-04-14 01:37:57.000000 pygubu_designer-0.39.3/examples/forms/formsdemo1appui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      635 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/examples/forms/project_styles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      723 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/framepad.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.423348 pygubu_designer-0.39.3/examples/helloworld/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       82 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/helloworld/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      740 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/helloworld/helloworld.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1178 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/helloworld/helloworld.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/helloworld/holamundo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1176 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/helloworld/holamundo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.431348 pygubu_designer-0.39.3/examples/i18n_gettext_demo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2303 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.431348 pygubu_designer-0.39.3/examples/i18n_gettext_demo/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1237 2024-02-13 03:45:58.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11576 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/demo-i18n.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1251 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/i18n.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.435348 pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1433 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/demoapp.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.199350 pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.435348 pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.439348 pygubu_designer-0.39.3/examples/image_property/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/image_property/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      710 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/image_property/image_property.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1682 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/image_property/image_property.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/image_property/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/image_property/yellow.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.447348 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      337 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.455348 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6612 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2529 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_cxFreeze/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.463348 pygubu_designer-0.39.3/examples/integration_with_nuitka/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      366 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.463348 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6510 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_nuitka/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.467347 pygubu_designer-0.39.3/examples/integration_with_py2exe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      258 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.475347 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/myapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2731 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_py2exe/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.479347 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.483347 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       72 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/MenuIcon4.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       90 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/ps_circle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/ps_cross.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       86 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/ps_square.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/imgs/ps_triangle.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6602 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2513 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.spec
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.483347 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      582 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.483347 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1141 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      526 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.487347 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1750 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      547 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.487347 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2190 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/main.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      755 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/myapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       34 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1975 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.491347 pygubu_designer-0.39.3/examples/integration_with_zipapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      365 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.203350 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.495347 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.503347 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3445 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.503347 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/extradata/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/extradata/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/extradata/notes.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      556 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/info.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3270 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/red.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/yellow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1013 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/main.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.507347 pygubu_designer-0.39.3/examples/jpg_image_on_canvas/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      825 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/jpg_image_on_canvas/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1244 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/jpg_image_on_canvas/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       14 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/jpg_image_on_canvas/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    38211 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/jpg_image_on_canvas/seaside400.jpg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3187 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/menubutton.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1347 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/menuexample.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.511347 pygubu_designer-0.39.3/examples/notebook/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/notebook/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/notebook/demo1app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1835 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/panedwindow.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/panes_and_notebooks.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.511347 pygubu_designer-0.39.3/examples/pathchooserdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       32 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/pathchooserdemo/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.515347 pygubu_designer-0.39.3/examples/pathchooserdemo/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/pathchooserdemo/demo1/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3220 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/pathchooserdemo/demo1/pathchooserdemo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.515347 pygubu_designer-0.39.3/examples/pathchooserdemo/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2644 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/pathchooserdemo/demo2/pathchooserdemo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/pathchooserdemo/demo2/pathchooserdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1840 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/scrollbarhelper.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.519347 pygubu_designer-0.39.3/examples/scrolledframe/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      104 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/scrolledframe/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      646 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/scrolledframe/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12412 2024-02-14 15:17:08.000000 pygubu_designer-0.39.3/examples/scrolledframe/scrolledframe_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10765 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/scrolledframe-layouts.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     9388 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/scrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.519347 pygubu_designer-0.39.3/examples/scrolledtext/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4030 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/scrolledtext/scrolledtext_demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      977 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/scrolledtext/scrolledtextdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.523347 pygubu_designer-0.39.3/examples/static_image/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      539 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/static_image/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1676 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/static_image/demoapp.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23336 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/static_image/logo_253.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/static_image/requirements.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.203350 pygubu_designer-0.39.3/examples/text/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.523347 pygubu_designer-0.39.3/examples/text/logwindowdemo/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3075 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/text/logwindowdemo/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1714 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/text/logwindowdemo/demo1app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.527347 pygubu_designer-0.39.3/examples/tk_window/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      144 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/tk_window/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4015 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/tk_window/green.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1354 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/tk_window/tkdemo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      600 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/tk_window/tkdemoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.527347 pygubu_designer-0.39.3/examples/toplevel_centered/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      154 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_centered/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1216 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_centered/centered_demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1317 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_centered/centered_demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1020 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_centered/demo.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.531347 pygubu_designer-0.39.3/examples/toplevel_menu/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_menu/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_menu/menu.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2470 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/toplevel_menu/menu.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.531347 pygubu_designer-0.39.3/examples/treeview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.531347 pygubu_designer-0.39.3/examples/treeview/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       43 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo1/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1496 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo1/treeview.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3473 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo1/treeview.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.535347 pygubu_designer-0.39.3/examples/treeview/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       64 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo2/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    23736 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo2/columns_stretching.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2712 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview/demo2/columnsstretchingdemo.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.535347 pygubu_designer-0.39.3/examples/treeview_editable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       28 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_editable/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.535347 pygubu_designer-0.39.3/examples/treeview_editable/demo1/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5044 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo1/demoapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo1/demoapp.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.539347 pygubu_designer-0.39.3/examples/treeview_editable/demo2/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5944 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo2/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3432 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo2/demo2app.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.547347 pygubu_designer-0.39.3/examples/treeview_editable/demo3/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      119 2024-05-04 02:36:40.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo3/README.md
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.551347 pygubu_designer-0.39.3/examples/treeview_editable/demo3/__pycache__/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2469 2024-05-04 02:17:34.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo3/__pycache__/demo3appui.cpython-311.pyc
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8944 2024-05-04 02:14:14.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5707 2024-05-04 02:36:40.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3app.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1002 2024-05-04 02:36:40.000000 pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3appui.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.559347 pygubu_designer-0.39.3/examples/treeview_filterable/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       30 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_filterable/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5404 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_filterable/demo.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2886 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/treeview_filterable/demoapp.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.563346 pygubu_designer-0.39.3/examples/user_input/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/user_input/README.md
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       16 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/user_input/requirements.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    28967 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/user_input/userinput.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3730 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/user_input/userinputapp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      883 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/variables.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4346 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/vscrolledframe.ui
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.567346 pygubu_designer-0.39.3/examples/windowdeleteevent/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      887 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/windowdeleteevent/demo1.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/windowdeleteevent/demo1.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      847 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/windowdeleteevent/demo2.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1271 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/examples/windowdeleteevent/demo2.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    88292 2024-04-10 03:51:03.000000 pygubu_designer-0.39.3/pygubu-designer.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2378 2024-05-23 02:52:59.000000 pygubu_designer-0.39.3/pyproject.toml
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       38 2024-05-23 02:59:17.075342 pygubu_designer-0.39.3/setup.cfg
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/setup.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.075342 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     7659 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/PKG-INFO
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    37650 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/SOURCES.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        1 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/dependency_links.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       65 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/entry_points.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      445 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/requires.txt
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       15 2024-05-23 02:59:16.000000 pygubu_designer-0.39.3/src/pygubu_designer.egg-info/top_level.txt
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.583346 pygubu_designer-0.39.3/src/pygubudesigner/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      200 2024-05-23 02:39:48.000000 pygubu_designer-0.39.3/src/pygubudesigner/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/__main__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1049 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/actions.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6373 2024-03-12 19:01:57.000000 pygubu_designer-0.39.3/src/pygubudesigner/bindingseditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.587346 pygubu_designer-0.39.3/src/pygubudesigner/codegen/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       76 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/codegen/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    19333 2024-04-08 01:37:06.000000 pygubu_designer-0.39.3/src/pygubudesigner/codegen/codebuilder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12583 2024-05-23 00:13:16.000000 pygubu_designer-0.39.3/src/pygubudesigner/codegen/scriptgenerator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11044 2024-03-12 19:01:57.000000 pygubu_designer-0.39.3/src/pygubudesigner/containerlayouteditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.591346 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2992 2024-03-13 03:14:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/app.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      907 2024-05-05 00:30:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/appuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      371 2024-05-05 00:29:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/base.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1620 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/customstyles.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2116 2024-04-08 02:11:56.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/script.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      474 2024-04-12 03:50:58.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/scriptuser.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      771 2024-04-08 02:22:55.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widget.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      542 2024-03-06 04:13:52.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widgetbo.py.mako
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      655 2024-04-12 03:59:49.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widgetuser.py.mako
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/images/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.599346 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       70 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/arrow-left2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       71 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/arrow-right2.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       81 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/bin-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       85 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/cancel-circle-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       61 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/close.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       73 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/download3-16.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/download3-32.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      230 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/mglass.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      377 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/property_invalid.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      875 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/pygubu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4897 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/pygubu200.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.775345 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      352 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      128 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      224 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      231 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       75 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1120 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      126 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      100 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      109 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1095 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.863344 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      132 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.Labelwidget.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.calendarframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.dialog.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.editabletreeview.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.pathchooserinput.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.scrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      197 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/pygubu.builder.widgets.toplevelmenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Calendar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      599 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.LabelFrame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Listbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Command.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      195 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      139 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Menuitem.Submenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Message.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.PanedWindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      114 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Text.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Toplevel.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.default.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Button.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Checkbutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Combobox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       96 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Entry.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Frame.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      105 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Label.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.LabeledScale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      129 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Labelframe.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Menubutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      142 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.Tab.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      131 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Notebook.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      140 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.OptionMenu.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.Pane.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      108 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Panedwindow.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Progressbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      124 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Radiobutton.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      111 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scale.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      121 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Scrollbar.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       89 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Separator.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      153 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Sizegrip.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      133 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Spinbox.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      156 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.Column.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      130 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/ttk.Treeview.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.867344 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      592 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      567 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      357 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-strikethrough.gif
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      572 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.871344 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      194 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/arrow-left2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      184 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/arrow-right2.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      162 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/bin-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      353 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/cancel-circle-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/circle-left.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      333 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/circle-right.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      170 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/download3-16.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      214 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/download3-32.png
+-rwxr-xr-x   0 aautalan  (1001) aautalan  (1001)      316 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/mglass.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      603 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/property_invalid.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4777 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/pygubu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    15896 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/pygubu200.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.963343 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      480 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      509 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      488 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      527 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      334 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      433 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      325 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      518 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      426 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      389 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      291 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      638 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      524 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      613 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      379 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      356 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      706 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      435 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      440 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      349 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      545 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      508 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      429 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      431 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      293 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      627 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      418 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.003342 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.calendarframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.dialog.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.editabletreeview.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.pathchooserinput.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.scrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkinterscrolledtext.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      186 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrollbarhelper.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      339 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.tkscrolledframe.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/pygubu.builder.widgets.toplevelmenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      161 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Calendar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      689 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Listbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      202 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Command.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      323 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      127 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Menuitem.Submenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.PanedWindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      148 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Text.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      169 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Toplevel.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      116 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.default.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      181 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Button.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      179 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Checkbutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      263 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Combobox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      125 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Entry.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      143 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Frame.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      205 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Label.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.LabeledScale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Menubutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Notebook.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      185 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.OptionMenu.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.Pane.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      118 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Panedwindow.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      138 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Progressbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      257 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Radiobutton.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      172 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scale.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      155 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Scrollbar.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      107 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Separator.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      206 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Spinbox.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      158 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/ttk.Treeview.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.003342 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      705 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      619 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      611 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      673 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.007342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/de/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.007342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/de/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3172 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      425 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.007342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13309 2024-04-22 01:09:43.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      854 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    58879 2024-04-22 00:44:13.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/pygubu-designer.pot
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    20171 2024-04-22 00:44:13.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/pygubu.pot
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/tr/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.011342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4815 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      393 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.011342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    53166 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10936 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:16.207350 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.015342 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    52658 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10937 2024-04-22 01:08:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.019342 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13872 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/about_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6320 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10318 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/container_layout_editor_base.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    16121 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/designer_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4093 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/messagebox.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    45719 2024-04-12 04:11:16.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/project_settings.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    49541 2024-04-20 01:39:30.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/pygubu-ui.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6509 2024-04-09 23:44:02.000000 pygubu_designer-0.39.3/src/pygubudesigner/data/ui/treecomponent_palette.ui
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4326 2024-04-15 03:30:30.000000 pygubu_designer-0.39.3/src/pygubudesigner/designerstyles.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2525 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/dialogs.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2122 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/i18n.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8476 2024-03-19 19:06:18.000000 pygubu_designer-0.39.3/src/pygubudesigner/layouteditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2688 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/logpanel.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    34307 2024-04-20 01:39:30.000000 pygubu_designer-0.39.3/src/pygubudesigner/main.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4418 2024-04-06 02:39:05.000000 pygubu_designer-0.39.3/src/pygubudesigner/preferences.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.023342 pygubu_designer-0.39.3/src/pygubudesigner/preview/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)       63 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/preview/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2664 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/preview/builder.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    13624 2024-04-02 02:28:06.000000 pygubu_designer-0.39.3/src/pygubudesigner/preview/helper.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    17119 2024-04-01 04:38:44.000000 pygubu_designer-0.39.3/src/pygubudesigner/preview/preview.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.027342 pygubu_designer-0.39.3/src/pygubudesigner/properties/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      373 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/__init__.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.027342 pygubu_designer-0.39.3/src/pygubudesigner/properties/editors/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/editors/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1027 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/editors/forms.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1866 2024-02-17 03:46:34.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/manager.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    50538 2024-04-11 03:47:20.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/predefined.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    31209 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/properties/propertieshelp.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5528 2024-04-14 01:38:41.000000 pygubu_designer-0.39.3/src/pygubudesigner/propertieseditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1915 2024-04-07 01:08:23.000000 pygubu_designer-0.39.3/src/pygubudesigner/rfilemanager.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.035342 pygubu_designer-0.39.3/src/pygubudesigner/services/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1854 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/aboutdialog.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      982 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/aboutdialogui.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.035342 pygubu_designer-0.39.3/src/pygubudesigner/services/builders/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/builders/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3356 2024-03-31 01:41:21.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/designersettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      931 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/designersettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2733 2024-04-14 22:42:58.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/fieldvalidator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1945 2024-03-07 01:08:46.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/messagebox.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      843 2024-03-07 01:11:22.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/messageboxui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4292 2024-05-05 07:26:13.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/project.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    12314 2024-05-05 05:09:57.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/projectsettings.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1821 2024-04-12 04:13:44.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/projectsettingsui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     6301 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/stylehandler.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4220 2024-03-31 23:43:45.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/theming.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.039342 pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)        0 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5799 2024-04-08 02:37:37.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/treecomponentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      450 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/treecomponentpalettebo.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3465 2024-04-08 03:06:36.000000 pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/treecomponentpaletteui.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    59403 2024-05-04 03:38:11.000000 pygubu_designer-0.39.3/src/pygubudesigner/uitreeeditor.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.043342 pygubu_designer-0.39.3/src/pygubudesigner/util/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2823 2024-04-01 01:31:03.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     4297 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/gridcalculator.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1964 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/keyboard.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1175 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/observable.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1289 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/screens.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2798 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/util/selecttool.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8344 2024-04-14 01:38:14.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgetdescr.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.071342 pygubu_designer-0.39.3/src/pygubudesigner/widgets/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1048 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/__init__.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3063 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/bindingeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3502 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/colorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5327 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/commandentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3943 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/componentpalette.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5088 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/containerlayouteditorbase.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     1640 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/cursorentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2681 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/dimensionentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2282 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/dynamicpropeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5164 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/entryvalidatecommandeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     8250 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/fontentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    10193 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/gridselector.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2491 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/imageentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3046 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/namedideditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2102 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/pixelcoordinateentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)    11940 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/propertyeditor.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3059 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/relativeentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5174 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/stickyentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     3255 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/tkvarentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     5936 2024-02-25 22:14:08.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/toolbarframe.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2650 2024-04-02 02:52:39.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/ttkstyleentry.py
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)     2536 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/src/pygubudesigner/widgets/whentry.py
+drwxr-xr-x   0 aautalan  (1001) aautalan  (1001)        0 2024-05-23 02:59:17.071342 pygubu_designer-0.39.3/tests/
+-rw-r--r--   0 aautalan  (1001) aautalan  (1001)      562 2023-09-09 20:40:32.000000 pygubu_designer-0.39.3/tests/test_plugin_init.py
```

### Comparing `pygubu_designer-0.39.2/LEEME.md` & `pygubu_designer-0.39.3/LEEME.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 a medida que lo necesiten.
 
 Pygubu esta inspirado por [Glade](https://es.wikipedia.org/wiki/Glade) (el diseñador de interfaces de gtk).
 
 Instalación
 ============
 
-La última versión de pygubu requiere Python >= 3.6
+La última versión de pygubu requiere Python >= 3.8
 
 Puedes instalar pygubu-designer usando:
 
 ### pip:
 
 ```
 pip install pygubu-designer
@@ -26,15 +26,15 @@
 
 <img src="pygubu-designer.png" alt="pygubu-desinger.png">
 
 
 Modo de uso
 ===========
 
-Ejecuta el diseñador ejecutando en una consola los siguientes comandos, 
+Ejecuta el diseñador ejecutando en una consola los siguientes comandos,
 dependiendo del sistema operativo que uses.
 
 ### Sistemas tipo Unix:
 
 ```
 pygubu-designer
 ```
@@ -86,15 +86,15 @@
         </child>
       </object>
     </child>
   </object>
 </interface>
 ```
 
-Luego, crea tu _aplicación_ como se muestra a continuación 
+Luego, crea tu _aplicación_ como se muestra a continuación
 ([holamundo.py](examples/helloworld/holamundo.py)):
 
 ```python
 # helloworld.py
 import pathlib
 import pygubu
 
@@ -138,20 +138,20 @@
 
 Ten en cuenta además que en lugar de `'mainwindow'` en la línea:
 
 ```python
 self.mainwindow = builder.get_object('mainwindow')
 ```
 
-Debes tener el nombre del _widget principal_ (el padre de todos los widgets), 
+Debes tener el nombre del _widget principal_ (el padre de todos los widgets),
 en caso contrario obtendras un error similar al siguiente::
 
     Exception: Widget not defined.
 
-Mira [este](https://github.com/alejandroautalan/pygubu/issues/40) issue 
+Mira [este](https://github.com/alejandroautalan/pygubu/issues/40) issue
 para mayor información.
 
 
 Documentación
 =============
 
 Visita la [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) para
@@ -161,15 +161,15 @@
 
 - [TkDocs](http://www.tkdocs.com)
 - [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)
 - [Tkinter 8.5 reference: a GUI for Python](https://tkdocs.com/shipman)
 - [An Introduction to Tkinter](http://effbot.org/tkinterbook) [(archive)](http://web.archive.org/web/20200504141939/http://www.effbot.org/tkinterbook)
 - [Tcl/Tk 8.5 Manual](http://www.tcl.tk/man/tcl8.5/)
 
-Tambien puedes buscar en el directorio de [ejemplos](examples) o mirar este 
+Tambien puedes buscar en el directorio de [ejemplos](examples) o mirar este
 ejemplo de 'Hola mundo' en
 [vídeo](http://youtu.be/wuzV9P8geDg)
 
 
 Historia
 ========
```

### Comparing `pygubu_designer-0.39.2/LICENSE.md` & `pygubu_designer-0.39.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/LISEZMOI.md` & `pygubu_designer-0.39.3/LISEZMOI.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/PKG-INFO` & `pygubu_designer-0.39.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.39.2
+Version: 0.39.3
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 Requires-Dist: appdirs>=1.4.3
 Requires-Dist: Mako>=1.1.4
 Requires-Dist: screeninfo>=0.8
 Requires-Dist: autopep8>=1.7
-Requires-Dist: pygubu>=0.35.1
+Requires-Dist: pygubu>=0.35.2
 Provides-Extra: ttkwidgets
 Requires-Dist: ttkwidgets; extra == "ttkwidgets"
 Provides-Extra: tksheet
 Requires-Dist: tksheet; extra == "tksheet"
 Provides-Extra: tkinterweb
 Requires-Dist: tkinterweb; extra == "tkinterweb"
 Provides-Extra: tkintertable
@@ -73,15 +72,15 @@
 The user interfaces designed are saved as [XML](https://en.wikipedia.org/wiki/XML) files, and, by using the _pygubu builder_, these can be loaded by applications dynamically as needed.
 
 Pygubu is inspired by [Glade](https://gitlab.gnome.org/GNOME/glade).
 
 Installation
 ============
 
-The latest version of pygubu requires Python >= 3.6
+The latest version of pygubu requires Python >= 3.8
 
 You can install pygubu-designer using:
 
 ### pip
 
 ```
 pip install pygubu-designer
@@ -115,18 +114,18 @@
 ```
 
 Where `C:\Python3` is the path to **your** Python installation directory.
 
 Now, you can start creating your tkinter application using the widgets that you
 find in the top panel called `Widget Palette`.
 
-After you finished creating your _UI definition_, save it to a `.ui` file by 
+After you finished creating your _UI definition_, save it to a `.ui` file by
 going to the top menu `File > Save`.
 
-The following is a UI definition example called 
+The following is a UI definition example called
 [helloworld.ui](examples/helloworld/helloworld.ui) created using pygubu:
 
 
 ```xml
 <?xml version='1.0' encoding='utf-8'?>
 <interface version="1.2">
   <object class="tk.Toplevel" id="mainwindow">
@@ -156,15 +155,15 @@
         </child>
       </object>
     </child>
   </object>
 </interface>
 ```
 
-Then, you should create your _application script_ as shown below 
+Then, you should create your _application script_ as shown below
 ([helloworld.py](examples/helloworld/helloworld.py)):
 
 ```python
 # helloworld.py
 import pathlib
 import tkinter as tk
 import tkinter.ttk as ttk
@@ -210,27 +209,27 @@
 
 Note also that instead of `'mainwindow'` in the following line:
 
 ```python
 self.mainwindow = builder.get_object('mainwindow', master)
 ```
 
-You should have the name of your _main widget_ (the parent of all widgets), 
+You should have the name of your _main widget_ (the parent of all widgets),
 otherwise you will get an error similar to the following:
 
     Exception: Widget not defined.
 
-See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for 
+See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for
 more information.
 
 
 Documentation
 =============
 
-Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for 
+Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for
 more documentation.
 
 
 The following are some good tkinter (and tk) references:
 
 - [TkDocs](http://www.tkdocs.com)
 - [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)
```

### Comparing `pygubu_designer-0.39.2/README.md` & `pygubu_designer-0.39.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 The user interfaces designed are saved as [XML](https://en.wikipedia.org/wiki/XML) files, and, by using the _pygubu builder_, these can be loaded by applications dynamically as needed.
 
 Pygubu is inspired by [Glade](https://gitlab.gnome.org/GNOME/glade).
 
 Installation
 ============
 
-The latest version of pygubu requires Python >= 3.6
+The latest version of pygubu requires Python >= 3.8
 
 You can install pygubu-designer using:
 
 ### pip
 
 ```
 pip install pygubu-designer
@@ -51,18 +51,18 @@
 ```
 
 Where `C:\Python3` is the path to **your** Python installation directory.
 
 Now, you can start creating your tkinter application using the widgets that you
 find in the top panel called `Widget Palette`.
 
-After you finished creating your _UI definition_, save it to a `.ui` file by 
+After you finished creating your _UI definition_, save it to a `.ui` file by
 going to the top menu `File > Save`.
 
-The following is a UI definition example called 
+The following is a UI definition example called
 [helloworld.ui](examples/helloworld/helloworld.ui) created using pygubu:
 
 
 ```xml
 <?xml version='1.0' encoding='utf-8'?>
 <interface version="1.2">
   <object class="tk.Toplevel" id="mainwindow">
@@ -92,15 +92,15 @@
         </child>
       </object>
     </child>
   </object>
 </interface>
 ```
 
-Then, you should create your _application script_ as shown below 
+Then, you should create your _application script_ as shown below
 ([helloworld.py](examples/helloworld/helloworld.py)):
 
 ```python
 # helloworld.py
 import pathlib
 import tkinter as tk
 import tkinter.ttk as ttk
@@ -146,27 +146,27 @@
 
 Note also that instead of `'mainwindow'` in the following line:
 
 ```python
 self.mainwindow = builder.get_object('mainwindow', master)
 ```
 
-You should have the name of your _main widget_ (the parent of all widgets), 
+You should have the name of your _main widget_ (the parent of all widgets),
 otherwise you will get an error similar to the following:
 
     Exception: Widget not defined.
 
-See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for 
+See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for
 more information.
 
 
 Documentation
 =============
 
-Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for 
+Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for
 more documentation.
 
 
 The following are some good tkinter (and tk) references:
 
 - [TkDocs](http://www.tkdocs.com)
 - [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)
```

### Comparing `pygubu_designer-0.39.2/development/create-imgs.py` & `pygubu_designer-0.39.3/development/create-imgs.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/dev-notes.txt` & `pygubu_designer-0.39.3/development/dev-notes.txt`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/devtool.py` & `pygubu_designer-0.39.3/development/devtool.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/devtool.sh` & `pygubu_designer-0.39.3/development/devtool.sh`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/gettext/pygubu.its` & `pygubu_designer-0.39.3/development/gettext/pygubu.its`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/main.py` & `pygubu_designer-0.39.3/development/new-designer-icons/main.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/button.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/button.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/button.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/canvas.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/canvas.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/canvas.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/combobox.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/combobox.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/combobox.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/default.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/default.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/default.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/default.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/entry.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/entry.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/entry.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/entry.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/frame.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/frame.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/frame.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/frame.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/label.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/label.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/label.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/labelframe.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/labelframe.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/labelframe.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/labelframe.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/menubutton.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/menubutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/menubutton.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/menubutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook-tab.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook-tab.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook-tab.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook-tab.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/notebook.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/notebook.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow-pane.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow-pane.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/pannedwindow.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/pannedwindow.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/progressbar.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/progressbar.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/progressbar.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/spinbutton.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/spinbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/spinbutton.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/spinbutton.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/textview.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/textview.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/textview.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/textview.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/toplevel.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/toplevel.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/toplevel.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/toplevel.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview-col.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview-col.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview-col.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview-col.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/treeview.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/treeview.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/viewport.png` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/viewport.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/pygubu-icons/viewport.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/pygubu-icons/viewport.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/template.svg` & `pygubu_designer-0.39.3/development/new-designer-icons/template.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/testnewicons.ui` & `pygubu_designer-0.39.3/development/new-designer-icons/testnewicons.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/new-designer-icons/testnewiconsapp.py` & `pygubu_designer-0.39.3/development/new-designer-icons/testnewiconsapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/Python-logo-notext.svg` & `pygubu_designer-0.39.3/development/pygubuLogo/Python-logo-notext.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu .ico` & `pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu .ico`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.icns` & `pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.icns`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.ico` & `pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.ico`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/logo_pygubu.xcf` & `pygubu_designer-0.39.3/development/pygubuLogo/logo_pygubu.xcf`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/pyGubu_newLogo.svg` & `pygubu_designer-0.39.3/development/pygubuLogo/pyGubu_newLogo.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubuLogo/tcl-tk.svg` & `pygubu_designer-0.39.3/development/pygubuLogo/tcl-tk.svg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/development/pygubudesigner_.py` & `pygubu_designer-0.39.3/development/pygubudesigner_.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/01_counter/counter.ui` & `pygubu_designer-0.39.3/examples/7guis/01_counter/counter.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/01_counter/counterapp.py` & `pygubu_designer-0.39.3/examples/7guis/01_counter/counterapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/02_temperature_converter/tempconv.ui` & `pygubu_designer-0.39.3/examples/7guis/02_temperature_converter/tempconv.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/02_temperature_converter/tempconvapp.py` & `pygubu_designer-0.39.3/examples/7guis/02_temperature_converter/tempconvapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/03_flight_Booker/flight_booker.ui` & `pygubu_designer-0.39.3/examples/7guis/03_flight_Booker/flight_booker.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/03_flight_Booker/flightbookerapp.py` & `pygubu_designer-0.39.3/examples/7guis/03_flight_Booker/flightbookerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/04_timer/timer.ui` & `pygubu_designer-0.39.3/examples/7guis/04_timer/timer.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/7guis/04_timer/timerapp.py` & `pygubu_designer-0.39.3/examples/7guis/04_timer/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/binding.ui` & `pygubu_designer-0.39.3/examples/binding.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/button_cb.py` & `pygubu_designer-0.39.3/examples/button_cb.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/button_cb.ui` & `pygubu_designer-0.39.3/examples/button_cb.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/myapp.py` & `pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/canvas/canvas-scrollregion/myapp.ui` & `pygubu_designer-0.39.3/examples/canvas/canvas-scrollregion/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/canvas_example.ui` & `pygubu_designer-0.39.3/examples/canvas_example.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/command_properties/command_properties.py` & `pygubu_designer-0.39.3/examples/command_properties/command_properties.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/command_properties/command_properties.ui` & `pygubu_designer-0.39.3/examples/command_properties/command_properties.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/command_properties/command_properties2.py` & `pygubu_designer-0.39.3/examples/command_properties/command_properties2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/commands.py` & `pygubu_designer-0.39.3/examples/commands.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/commands.ui` & `pygubu_designer-0.39.3/examples/commands.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/control_variables/controlvariables.py` & `pygubu_designer-0.39.3/examples/control_variables/controlvariables.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/control_variables/controlvariables.ui` & `pygubu_designer-0.39.3/examples/control_variables/controlvariables.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/custom_widget/timer_main.ui` & `pygubu_designer-0.39.3/examples/custom_widget/timer_main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/custom_widget/timerapp.py` & `pygubu_designer-0.39.3/examples/custom_widget/timerapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/custom_widget/timerappui.py` & `pygubu_designer-0.39.3/examples/custom_widget/timerappui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/custom_widget/timewidget.ui` & `pygubu_designer-0.39.3/examples/custom_widget/timewidget.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/custom_widget/timewidget_old.py` & `pygubu_designer-0.39.3/examples/custom_widget/timewidget_old.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/customtkinter/complex/complex_demo.ui` & `pygubu_designer-0.39.3/examples/customtkinter/complex/complex_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/customtkinter/complex/complexdemoapp.py` & `pygubu_designer-0.39.3/examples/customtkinter/complex/complexdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/customtkinter/simple/simple_demo.ui` & `pygubu_designer-0.39.3/examples/customtkinter/simple/simple_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/customtkinter/simple/simpledemoapp.py` & `pygubu_designer-0.39.3/examples/customtkinter/simple/simpledemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo1/demo.py` & `pygubu_designer-0.39.3/examples/dialogs/demo1/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo1/demo.ui` & `pygubu_designer-0.39.3/examples/dialogs/demo1/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo2/demo.py` & `pygubu_designer-0.39.3/examples/dialogs/demo2/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo2/demo.ui` & `pygubu_designer-0.39.3/examples/dialogs/demo2/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo3/demo.py` & `pygubu_designer-0.39.3/examples/dialogs/demo3/demo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo3/demo.ui` & `pygubu_designer-0.39.3/examples/dialogs/demo3/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdemo.ui` & `pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdemoapp.py` & `pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/dialogs/demo4/settingsdialog.py` & `pygubu_designer-0.39.3/examples/dialogs/demo4/settingsdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/example_grid_rc.ui` & `pygubu_designer-0.39.3/examples/example_grid_rc.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/example_grid_rc_2.ui` & `pygubu_designer-0.39.3/examples/example_grid_rc_2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/forms/__pycache__/formsdemo1base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/__pycache__/project_styles.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/forms/__pycache__/project_styles.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/demo1.ui` & `pygubu_designer-0.39.3/examples/forms/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/formsdemo1app.py` & `pygubu_designer-0.39.3/examples/forms/formsdemo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/formsdemo1appui.py` & `pygubu_designer-0.39.3/examples/forms/formsdemo1appui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/forms/project_styles.py` & `pygubu_designer-0.39.3/examples/forms/project_styles.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/framepad.ui` & `pygubu_designer-0.39.3/examples/framepad.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/helloworld/helloworld.py` & `pygubu_designer-0.39.3/examples/helloworld/helloworld.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/helloworld/helloworld.ui` & `pygubu_designer-0.39.3/examples/helloworld/helloworld.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/helloworld/holamundo.py` & `pygubu_designer-0.39.3/examples/helloworld/holamundo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/helloworld/holamundo.ui` & `pygubu_designer-0.39.3/examples/helloworld/holamundo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/README.md` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/README.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/__pycache__/i18n.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/demo-i18n.ui` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/demo-i18n.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/demoapp.py` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/i18n.py` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/demoapp.pot` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/demoapp.pot`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo` & `pygubu_designer-0.39.3/examples/i18n_gettext_demo/locale/es/LC_MESSAGES/demoapp.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/image_property/green.gif` & `pygubu_designer-0.39.3/examples/image_property/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/image_property/image_property.py` & `pygubu_designer-0.39.3/examples/image_property/image_property.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/image_property/image_property.ui` & `pygubu_designer-0.39.3/examples/image_property/image_property.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/image_property/red.gif` & `pygubu_designer-0.39.3/examples/image_property/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/image_property/yellow.gif` & `pygubu_designer-0.39.3/examples/image_property/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_cxFreeze/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_cxFreeze/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_cxFreeze/myapp.ui` & `pygubu_designer-0.39.3/examples/integration_with_cxFreeze/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_cxFreeze/setup.py` & `pygubu_designer-0.39.3/examples/integration_with_cxFreeze/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_nuitka/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_nuitka/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_nuitka/myapp.ui` & `pygubu_designer-0.39.3/examples/integration_with_nuitka/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_py2exe/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_py2exe/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_py2exe/myapp.ui` & `pygubu_designer-0.39.3/examples/integration_with_py2exe/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_py2exe/setup.py` & `pygubu_designer-0.39.3/examples/integration_with_py2exe/setup.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.spec` & `pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.spec`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_pyinstaller/myapp.ui` & `pygubu_designer-0.39.3/examples/integration_with_pyinstaller/myapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/README.md` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/README.md`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/main.ui` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp1/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp1/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/main.ui` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp2/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/main.ui` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/main.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/myapp.py` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/myapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py` & `pygubu_designer-0.39.3/examples/integration_with_tkcalendar/myapp3/tkcalendarwidgets.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/green.gif` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/info.txt` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/info.txt`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/red.gif` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/red.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/data/yellow.gif` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/data/yellow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/integration_with_zipapp/src/demoapp/main.py` & `pygubu_designer-0.39.3/examples/integration_with_zipapp/src/demoapp/main.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/jpg_image_on_canvas/demoapp.py` & `pygubu_designer-0.39.3/examples/jpg_image_on_canvas/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/jpg_image_on_canvas/demoapp.ui` & `pygubu_designer-0.39.3/examples/jpg_image_on_canvas/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/jpg_image_on_canvas/seaside400.jpg` & `pygubu_designer-0.39.3/examples/jpg_image_on_canvas/seaside400.jpg`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/menubutton.ui` & `pygubu_designer-0.39.3/examples/menubutton.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/menuexample.ui` & `pygubu_designer-0.39.3/examples/menuexample.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/notebook/demo1.ui` & `pygubu_designer-0.39.3/examples/notebook/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/notebook/demo1app.py` & `pygubu_designer-0.39.3/examples/notebook/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/panedwindow.ui` & `pygubu_designer-0.39.3/examples/panedwindow.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/panes_and_notebooks.ui` & `pygubu_designer-0.39.3/examples/panes_and_notebooks.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/pathchooserdemo/demo1/pathchooserdemo.py` & `pygubu_designer-0.39.3/examples/pathchooserdemo/demo1/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/pathchooserdemo/demo1/pathchooserdemo.ui` & `pygubu_designer-0.39.3/examples/pathchooserdemo/demo1/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/pathchooserdemo/demo2/pathchooserdemo.py` & `pygubu_designer-0.39.3/examples/pathchooserdemo/demo2/pathchooserdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/pathchooserdemo/demo2/pathchooserdemo.ui` & `pygubu_designer-0.39.3/examples/pathchooserdemo/demo2/pathchooserdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrollbarhelper.ui` & `pygubu_designer-0.39.3/examples/scrollbarhelper.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledframe/demoapp.py` & `pygubu_designer-0.39.3/examples/scrolledframe/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledframe/scrolledframe_demo.ui` & `pygubu_designer-0.39.3/examples/scrolledframe/scrolledframe_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledframe-layouts.ui` & `pygubu_designer-0.39.3/examples/scrolledframe-layouts.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledframe.ui` & `pygubu_designer-0.39.3/examples/scrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledtext/scrolledtext_demo.ui` & `pygubu_designer-0.39.3/examples/scrolledtext/scrolledtext_demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/scrolledtext/scrolledtextdemoapp.py` & `pygubu_designer-0.39.3/examples/scrolledtext/scrolledtextdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/static_image/demoapp.py` & `pygubu_designer-0.39.3/examples/static_image/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/static_image/demoapp.ui` & `pygubu_designer-0.39.3/examples/static_image/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/static_image/logo_253.png` & `pygubu_designer-0.39.3/examples/static_image/logo_253.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/text/logwindowdemo/demo1.ui` & `pygubu_designer-0.39.3/examples/text/logwindowdemo/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/text/logwindowdemo/demo1app.py` & `pygubu_designer-0.39.3/examples/text/logwindowdemo/demo1app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/tk_window/green.gif` & `pygubu_designer-0.39.3/examples/tk_window/green.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/tk_window/tkdemo.ui` & `pygubu_designer-0.39.3/examples/tk_window/tkdemo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/tk_window/tkdemoapp.py` & `pygubu_designer-0.39.3/examples/tk_window/tkdemoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/toplevel_centered/centered_demo1.py` & `pygubu_designer-0.39.3/examples/toplevel_centered/centered_demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/toplevel_centered/centered_demo2.py` & `pygubu_designer-0.39.3/examples/toplevel_centered/centered_demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/toplevel_centered/demo.ui` & `pygubu_designer-0.39.3/examples/toplevel_centered/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/toplevel_menu/menu.py` & `pygubu_designer-0.39.3/examples/toplevel_menu/menu.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/toplevel_menu/menu.ui` & `pygubu_designer-0.39.3/examples/toplevel_menu/menu.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview/demo1/treeview.py` & `pygubu_designer-0.39.3/examples/treeview/demo1/treeview.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview/demo1/treeview.ui` & `pygubu_designer-0.39.3/examples/treeview/demo1/treeview.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview/demo2/columns_stretching.ui` & `pygubu_designer-0.39.3/examples/treeview/demo2/columns_stretching.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview/demo2/columnsstretchingdemo.py` & `pygubu_designer-0.39.3/examples/treeview/demo2/columnsstretchingdemo.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo1/demoapp.py` & `pygubu_designer-0.39.3/examples/treeview_editable/demo1/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo1/demoapp.ui` & `pygubu_designer-0.39.3/examples/treeview_editable/demo1/demoapp.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo2/demo2.ui` & `pygubu_designer-0.39.3/examples/treeview_editable/demo2/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo2/demo2app.py` & `pygubu_designer-0.39.3/examples/treeview_editable/demo2/demo2app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo3/__pycache__/demo3appui.cpython-311.pyc` & `pygubu_designer-0.39.3/examples/treeview_editable/demo3/__pycache__/demo3appui.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3.ui` & `pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3app.py` & `pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3app.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_editable/demo3/demo3appui.py` & `pygubu_designer-0.39.3/examples/treeview_editable/demo3/demo3appui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_filterable/demo.ui` & `pygubu_designer-0.39.3/examples/treeview_filterable/demo.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/treeview_filterable/demoapp.py` & `pygubu_designer-0.39.3/examples/treeview_filterable/demoapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/user_input/userinput.ui` & `pygubu_designer-0.39.3/examples/user_input/userinput.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/user_input/userinputapp.py` & `pygubu_designer-0.39.3/examples/user_input/userinputapp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/variables.ui` & `pygubu_designer-0.39.3/examples/variables.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/vscrolledframe.ui` & `pygubu_designer-0.39.3/examples/vscrolledframe.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/windowdeleteevent/demo1.py` & `pygubu_designer-0.39.3/examples/windowdeleteevent/demo1.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/windowdeleteevent/demo1.ui` & `pygubu_designer-0.39.3/examples/windowdeleteevent/demo1.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/windowdeleteevent/demo2.py` & `pygubu_designer-0.39.3/examples/windowdeleteevent/demo2.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/examples/windowdeleteevent/demo2.ui` & `pygubu_designer-0.39.3/examples/windowdeleteevent/demo2.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/pygubu-designer.png` & `pygubu_designer-0.39.3/pygubu-designer.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/pyproject.toml` & `pygubu_designer-0.39.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,43 +2,42 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygubu-designer"
 description = "A simple GUI designer for the python tkinter module"
 readme = "README.md"
-requires-python = ">=3.6"
+requires-python = ">=3.8"
 license = { text = "GPL-3" }
 keywords = ["gui", "tkinter", "designer"]
 authors = [
   { name = "Alejandro Autalan", email = "alejandroautalan@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
   "Operating System :: OS Independent",
   "Intended Audience :: Developers",
   "Topic :: Software Development :: Libraries :: Python Modules",
   "Topic :: Utilities",
   "Topic :: Software Development :: User Interfaces",
 ]
 dependencies = [
     "appdirs >=1.4.3",
     "Mako >=1.1.4",
     "screeninfo >=0.8",
     "autopep8 >=1.7",
-    "pygubu >=0.35.1"
+    "pygubu >=0.35.2"
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/alejandroautalan/pygubu-designer#readme"
 Issues = "https://github.com/alejandroautalan/pygubu-designer/issues"
 Source = "https://github.com/alejandroautalan/pygubu-designer"
@@ -72,15 +71,15 @@
 where = ["src"]
 
 [tool.setuptools.exclude-package-data]
 "*" = ["*.pot", "*.po"]
 
 [tool.black]
 line-length = 80
-target-version = ["py36", "py37", "py38", "py39", "py310"]
+target-version = ["py38", "py39", "py310"]
 include = '\\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.mypy_cache
   | \.tox
```

### Comparing `pygubu_designer-0.39.2/src/pygubu_designer.egg-info/PKG-INFO` & `pygubu_designer-0.39.3/src/pygubu_designer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 Metadata-Version: 2.1
 Name: pygubu-designer
-Version: 0.39.2
+Version: 0.39.3
 Summary: A simple GUI designer for the python tkinter module
 Author-email: Alejandro Autalan <alejandroautalan@gmail.com>
 License: GPL-3
 Project-URL: Documentation, https://github.com/alejandroautalan/pygubu-designer#readme
 Project-URL: Issues, https://github.com/alejandroautalan/pygubu-designer/issues
 Project-URL: Source, https://github.com/alejandroautalan/pygubu-designer
 Keywords: gui,tkinter,designer
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: User Interfaces
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 License-File: AUTHORS
 Requires-Dist: appdirs>=1.4.3
 Requires-Dist: Mako>=1.1.4
 Requires-Dist: screeninfo>=0.8
 Requires-Dist: autopep8>=1.7
-Requires-Dist: pygubu>=0.35.1
+Requires-Dist: pygubu>=0.35.2
 Provides-Extra: ttkwidgets
 Requires-Dist: ttkwidgets; extra == "ttkwidgets"
 Provides-Extra: tksheet
 Requires-Dist: tksheet; extra == "tksheet"
 Provides-Extra: tkinterweb
 Requires-Dist: tkinterweb; extra == "tkinterweb"
 Provides-Extra: tkintertable
@@ -73,15 +72,15 @@
 The user interfaces designed are saved as [XML](https://en.wikipedia.org/wiki/XML) files, and, by using the _pygubu builder_, these can be loaded by applications dynamically as needed.
 
 Pygubu is inspired by [Glade](https://gitlab.gnome.org/GNOME/glade).
 
 Installation
 ============
 
-The latest version of pygubu requires Python >= 3.6
+The latest version of pygubu requires Python >= 3.8
 
 You can install pygubu-designer using:
 
 ### pip
 
 ```
 pip install pygubu-designer
@@ -115,18 +114,18 @@
 ```
 
 Where `C:\Python3` is the path to **your** Python installation directory.
 
 Now, you can start creating your tkinter application using the widgets that you
 find in the top panel called `Widget Palette`.
 
-After you finished creating your _UI definition_, save it to a `.ui` file by 
+After you finished creating your _UI definition_, save it to a `.ui` file by
 going to the top menu `File > Save`.
 
-The following is a UI definition example called 
+The following is a UI definition example called
 [helloworld.ui](examples/helloworld/helloworld.ui) created using pygubu:
 
 
 ```xml
 <?xml version='1.0' encoding='utf-8'?>
 <interface version="1.2">
   <object class="tk.Toplevel" id="mainwindow">
@@ -156,15 +155,15 @@
         </child>
       </object>
     </child>
   </object>
 </interface>
 ```
 
-Then, you should create your _application script_ as shown below 
+Then, you should create your _application script_ as shown below
 ([helloworld.py](examples/helloworld/helloworld.py)):
 
 ```python
 # helloworld.py
 import pathlib
 import tkinter as tk
 import tkinter.ttk as ttk
@@ -210,27 +209,27 @@
 
 Note also that instead of `'mainwindow'` in the following line:
 
 ```python
 self.mainwindow = builder.get_object('mainwindow', master)
 ```
 
-You should have the name of your _main widget_ (the parent of all widgets), 
+You should have the name of your _main widget_ (the parent of all widgets),
 otherwise you will get an error similar to the following:
 
     Exception: Widget not defined.
 
-See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for 
+See [this](https://github.com/alejandroautalan/pygubu/issues/40) issue for
 more information.
 
 
 Documentation
 =============
 
-Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for 
+Visit the [wiki](https://github.com/alejandroautalan/pygubu-designer/wiki) for
 more documentation.
 
 
 The following are some good tkinter (and tk) references:
 
 - [TkDocs](http://www.tkdocs.com)
 - [Graphical User Interfaces with Tk](https://docs.python.org/3/library/tk.html)
```

### Comparing `pygubu_designer-0.39.2/src/pygubu_designer.egg-info/SOURCES.txt` & `pygubu_designer-0.39.3/src/pygubu_designer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -127,14 +127,24 @@
 examples/dialogs/demo3/demo.py
 examples/dialogs/demo3/demo.ui
 examples/dialogs/demo4/README.md
 examples/dialogs/demo4/settingsdemo.ui
 examples/dialogs/demo4/settingsdemoapp.py
 examples/dialogs/demo4/settingsdialog.py
 examples/dialogs/demo4/__pycache__/settingsdialog.cpython-311.pyc
+examples/dialogs/demo5/README.md
+examples/dialogs/demo5/dialog1.py
+examples/dialogs/demo5/dialog1.ui
+examples/dialogs/demo5/dialog1ui.py
+examples/dialogs/demo5/mainapp.py
+examples/dialogs/demo5/mainapp.ui
+examples/dialogs/demo5/mainappui.py
+examples/dialogs/demo5/__pycache__/dialog1.cpython-311.pyc
+examples/dialogs/demo5/__pycache__/dialog1ui.cpython-311.pyc
+examples/dialogs/demo5/__pycache__/mainappui.cpython-311.pyc
 examples/forms/demo1.ui
 examples/forms/formsdemo1app.py
 examples/forms/formsdemo1appui.py
 examples/forms/project_styles.py
 examples/forms/__pycache__/formsdemo1appui.cpython-311.pyc
 examples/forms/__pycache__/formsdemo1base.cpython-311.pyc
 examples/forms/__pycache__/project_styles.cpython-311.pyc
```

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/actions.py` & `pygubu_designer-0.39.3/src/pygubudesigner/actions.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/bindingseditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/bindingseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/codegen/codebuilder.py` & `pygubu_designer-0.39.3/src/pygubudesigner/codegen/codebuilder.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/codegen/scriptgenerator.py` & `pygubu_designer-0.39.3/src/pygubudesigner/codegen/scriptgenerator.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # PURPOSE.  See the GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License along
 # with this program.  If not, see <http://www.gnu.org/licenses/>.
 import keyword
 import logging
 import pathlib
+import codecs
 import tkinter as tk
 from tkinter import filedialog, messagebox
 
 import autopep8
 from mako.lookup import TemplateLookup
 
 from .codebuilder import UI2Code
@@ -72,15 +73,15 @@
         bcontext["class_name"] = context["class_name"] + "UI"
         tpl = makolookup.get_template("app.py.mako")
         final_code = tpl.render(**bcontext)
         final_code = self._format_code(final_code)
 
         output_dir = context["output_dir"]
         outfn = output_dir / (context["module_name"] + "ui.py")
-        with open(outfn, "wt") as outfile:
+        with codecs.open(outfn, "w", encoding="utf-8") as outfile:
             outfile.write(final_code)
             logger.info("Generated code file: %s", outfn)
 
         context["import_lines"] += (
             "\nfrom "
             + context["module_name"]
             + "ui import "
@@ -88,15 +89,15 @@
         )
         tpl = makolookup.get_template("appuser.py.mako")
         final_code = tpl.render(**context)
         final_code = self._format_code(final_code)
         outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
         # DO NOT overwrite user module.
         if not outfn.exists():
-            with open(outfn, "wt") as outfile:
+            with codecs.open(outfn, "w", encoding="utf-8") as outfile:
                 outfile.write(final_code)
                 logger.info("Generated code file: %s", outfn)
 
     def _script_code(self, generator, context):
         uidef = self.tree.tree_to_uidef()
         target = context["target"]
 
@@ -130,24 +131,24 @@
         bcontext["class_name"] = context["class_name"] + "UI"
         tpl = makolookup.get_template("script.py.mako")
         final_code = tpl.render(**bcontext)
         final_code = self._format_code(final_code)
 
         output_dir = context["output_dir"]
         outfn = output_dir / (context["module_name"] + "ui.py")
-        with open(outfn, "wt") as outfile:
+        with codecs.open(outfn, "w", encoding="utf-8") as outfile:
             outfile.write(final_code)
 
         tpl = makolookup.get_template("scriptuser.py.mako")
         final_code = tpl.render(**context)
         final_code = self._format_code(final_code)
         outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
         # DO NOT overwrite user module.
         if not outfn.exists():
-            with open(outfn, "wt") as outfile:
+            with codecs.open(outfn, "w", encoding="utf-8") as outfile:
                 outfile.write(final_code)
                 logger.info("Generated code file: %s", outfn)
 
     def _widget_code(self, generator, context):
         uidef = self.tree.tree_to_uidef()
         target = context["target"]
 
@@ -164,36 +165,36 @@
         bcontext["class_name"] = context["class_name"] + "UI"
         tpl = makolookup.get_template("widget.py.mako")
         final_code = tpl.render(**bcontext)
         final_code = self._format_code(final_code)
 
         output_dir = context["output_dir"]
         outfn = output_dir / (context["module_name"] + "ui.py")
-        with open(outfn, "wt") as outfile:
+        with codecs.open(outfn, "w", encoding="utf-8") as outfile:
             outfile.write(final_code)
             logger.info("Generated code file: %s", outfn)
 
         tpl = makolookup.get_template("widgetbo.py.mako")
         final_code = tpl.render(**context)
         final_code = self._format_code(final_code)
         output_dir2 = context["output_dir2"]
         outfn: pathlib.Path = output_dir2 / (context["module_name"] + "bo.py")
         # DO NOT overwrite user module.
         if not outfn.exists():
-            with open(outfn, "wt") as outfile:
+            with codecs.open(outfn, "w", encoding="utf-8") as outfile:
                 outfile.write(final_code)
                 logger.info("Generated code file: %s", outfn)
 
         tpl = makolookup.get_template("widgetuser.py.mako")
         final_code = tpl.render(**context)
         final_code = self._format_code(final_code)
         outfn: pathlib.Path = output_dir / (context["module_name"] + ".py")
         # DO NOT overwrite user module.
         if not outfn.exists():
-            with open(outfn, "wt") as outfile:
+            with codecs.open(outfn, "w", encoding="utf-8") as outfile:
                 outfile.write(final_code)
                 logger.info("Generated code file: %s", outfn)
 
     def generate_code(self):
         project = self.app.current_project
         config = project.get_full_settings()
         generator = UI2Code()
```

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/containerlayouteditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/containerlayouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/app.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/app.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/appuser.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/appuser.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/customstyles.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/customstyles.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/script.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/script.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widget.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widget.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widgetbo.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widgetbo.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/code_templates/widgetuser.py.mako` & `pygubu_designer-0.39.3/src/pygubudesigner/data/code_templates/widgetuser.py.mako`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/pygubu.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/pygubu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/pygubu200.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/pygubu200.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.dialog.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.editabletreeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.scrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrollbarhelper.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/pygubu.builder.widgets.tkscrolledframe.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Calendar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Listbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Command.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Menuitem.Submenu.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.PanedWindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Text.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.Toplevel.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/tk.default.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Button.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Checkbutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Combobox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Entry.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Frame.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Label.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.LabeledScale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Menubutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Notebook.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.Pane.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Panedwindow.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Progressbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Radiobutton.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scale.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Separator.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Spinbox.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/16x16/ttk.Treeview.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/22x22/tk.Canvas.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-bold.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-italic.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-gif/widgets/fontentry/format-text-underline.gif`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/property_invalid.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/property_invalid.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/pygubu.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/pygubu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/pygubu200.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/pygubu200.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/pygubu.builder.widgets.toplevelmenu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Menuitem.Submenu.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/tk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Button.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Checkbutton.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Combobox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Label.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Progressbar.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/16x16/ttk.Spinbox.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/22x22/tk.Canvas.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-bold.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-italic.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-strikethrough.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png` & `pygubu_designer-0.39.3/src/pygubudesigner/data/images/images-png/widgets/fontentry/format-text-underline.png`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/de/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/es/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/pygubu-designer.pot` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/pygubu-designer.pot`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/pygubu.pot` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/pygubu.pot`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/tr/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_CN/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu-designer.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo` & `pygubu_designer-0.39.3/src/pygubudesigner/data/locale/zh_Hans/LC_MESSAGES/pygubu.mo`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/about_dialog.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/about_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/ask_save_changes_dialog.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/container_layout_editor_base.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/container_layout_editor_base.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/designer_settings.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/designer_settings.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/messagebox.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/messagebox.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/project_settings.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/project_settings.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/pygubu-ui.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/pygubu-ui.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/data/ui/treecomponent_palette.ui` & `pygubu_designer-0.39.3/src/pygubudesigner/data/ui/treecomponent_palette.ui`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/designerstyles.py` & `pygubu_designer-0.39.3/src/pygubudesigner/designerstyles.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/dialogs.py` & `pygubu_designer-0.39.3/src/pygubudesigner/dialogs.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/i18n.py` & `pygubu_designer-0.39.3/src/pygubudesigner/i18n.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/layouteditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/layouteditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/logpanel.py` & `pygubu_designer-0.39.3/src/pygubudesigner/logpanel.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/main.py` & `pygubu_designer-0.39.3/src/pygubudesigner/main.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/preferences.py` & `pygubu_designer-0.39.3/src/pygubudesigner/preferences.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/preview/builder.py` & `pygubu_designer-0.39.3/src/pygubudesigner/preview/builder.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/preview/helper.py` & `pygubu_designer-0.39.3/src/pygubudesigner/preview/helper.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/preview/preview.py` & `pygubu_designer-0.39.3/src/pygubudesigner/preview/preview.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/properties/editors/forms.py` & `pygubu_designer-0.39.3/src/pygubudesigner/properties/editors/forms.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/properties/manager.py` & `pygubu_designer-0.39.3/src/pygubudesigner/properties/manager.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/properties/predefined.py` & `pygubu_designer-0.39.3/src/pygubudesigner/properties/predefined.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/properties/propertieshelp.py` & `pygubu_designer-0.39.3/src/pygubudesigner/properties/propertieshelp.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/propertieseditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/propertieseditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/rfilemanager.py` & `pygubu_designer-0.39.3/src/pygubudesigner/rfilemanager.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/aboutdialog.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/aboutdialog.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/aboutdialogui.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/aboutdialogui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/designersettings.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/designersettings.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/designersettingsui.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/designersettingsui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/fieldvalidator.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/fieldvalidator.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/messagebox.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/messagebox.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/messageboxui.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/messageboxui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/project.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/project.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/projectsettings.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/projectsettings.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/projectsettingsui.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/projectsettingsui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/stylehandler.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/stylehandler.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/theming.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/theming.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/treecomponentpalette.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/treecomponentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/services/widgets/treecomponentpaletteui.py` & `pygubu_designer-0.39.3/src/pygubudesigner/services/widgets/treecomponentpaletteui.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/uitreeeditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/uitreeeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/__init__.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/gridcalculator.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/gridcalculator.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/keyboard.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/keyboard.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/observable.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/observable.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/screens.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/screens.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/util/selecttool.py` & `pygubu_designer-0.39.3/src/pygubudesigner/util/selecttool.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgetdescr.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgetdescr.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/__init__.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/bindingeditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/bindingeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/colorentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/colorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/commandentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/commandentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/componentpalette.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/componentpalette.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/containerlayouteditorbase.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/containerlayouteditorbase.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/cursorentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/cursorentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/dimensionentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/dimensionentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/dynamicpropeditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/dynamicpropeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/entryvalidatecommandeditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/entryvalidatecommandeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/fontentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/fontentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/gridselector.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/gridselector.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/imageentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/imageentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/namedideditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/namedideditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/pixelcoordinateentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/pixelcoordinateentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/propertyeditor.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/propertyeditor.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/relativeentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/relativeentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/stickyentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/stickyentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/tkvarentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/tkvarentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/toolbarframe.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/toolbarframe.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/ttkstyleentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/ttkstyleentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/src/pygubudesigner/widgets/whentry.py` & `pygubu_designer-0.39.3/src/pygubudesigner/widgets/whentry.py`

 * *Files identical despite different names*

### Comparing `pygubu_designer-0.39.2/tests/test_plugin_init.py` & `pygubu_designer-0.39.3/tests/test_plugin_init.py`

 * *Files identical despite different names*

