# Comparing `tmp/easyplot_toolbox-0.0.0.tar.gz` & `tmp/easyplot_toolbox-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyplot_toolbox-0.0.0.tar", max compression
+gzip compressed data, was "easyplot_toolbox-1.0.0.tar", max compression
```

## Comparing `easyplot_toolbox-0.0.0.tar` & `easyplot_toolbox-1.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       23 2024-03-21 15:12:08.025025 easyplot_toolbox-0.0.0/easyplot_toolbox/__init__.py
--rw-r--r--   0        0        0    32553 2024-04-24 13:57:53.066999 easyplot_toolbox-0.0.0/easyplot_toolbox/easyplot.py
--rw-r--r--   0        0        0     1115 2023-07-25 14:25:53.487702 easyplot_toolbox-0.0.0/license.md
--rw-r--r--   0        0        0      416 2024-04-24 14:25:46.918750 easyplot_toolbox-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      910 2024-04-24 14:04:31.072060 easyplot_toolbox-0.0.0/readme.md
--rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 easyplot_toolbox-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0       23 2024-03-21 15:12:08.025025 easyplot_toolbox-1.0.0/easyplot_toolbox/__init__.py
+-rw-r--r--   0        0        0    36508 2024-04-24 18:48:18.619387 easyplot_toolbox-1.0.0/easyplot_toolbox/EASYPLOT.py
+-rw-r--r--   0        0        0     1115 2023-07-25 14:25:53.487702 easyplot_toolbox-1.0.0/license.md
+-rw-r--r--   0        0        0      416 2024-04-24 18:48:18.649394 easyplot_toolbox-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      910 2024-04-24 14:04:31.072060 easyplot_toolbox-1.0.0/readme.md
+-rw-r--r--   0        0        0     1565 1970-01-01 00:00:00.000000 easyplot_toolbox-1.0.0/PKG-INFO
```

### Comparing `easyplot_toolbox-0.0.0/easyplot_toolbox/easyplot.py` & `easyplot_toolbox-1.0.0/easyplot_toolbox/EASYPLOT.py`

 * *Files 9% similar despite different names*

```diff
@@ -60,15 +60,35 @@
     """
 
     return {key.lower(): value for key, value in d.items()}
 
 
 def histogram_chart(**kwargs):
     """
-    See documentation in: https://wmpjrufg.github.io/EASYPLOTPY/001-1.html
+    This function shows a Boxplot and Histogram in a single chart.
+
+    Args:
+        plot_setup (Dictionary): Setup chart Dictionary with the following keys:
+            name (String): Path + name figure (key required in plot_setup)
+            width (Float): figure width in SI units (key required in plot_setup)
+            height (Float): figure height in SI units (key required in plot_setup)
+            extension (String): File extension (key required in plot_setup)
+            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            x axis label (String): x axis label (key required in plot_setup)
+            x axis size (Integer): x axis size (key required in plot_setup)
+            y axis label (String): y axis label (key required in plot_setup)
+            y axis size (Integer): y axis size (key required in plot_setup)
+            axises color (String): Axises color (key required in plot_setup)
+            labels size (Integer): Labels size (key required in plot_setup)
+            labels color (String): Labels color (key required in plot_setup)
+            chart color (String): Chart color (key required in plot_setup)
+            bins (Integer): Range representing the width of a single bar (key required in plot_setup)
+            
+    Returns:
+        None
     """
 
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
@@ -76,48 +96,51 @@
     x_axis_label = plot_setup['x axis label']
     x_axis_size = plot_setup['x axis size']
     y_axis_label = plot_setup['y axis label']
     y_axis_size = plot_setup['y axis size']
     axises_color = plot_setup['axises color']
     labels_size = plot_setup['labels size']     
     labels_color = plot_setup['labels color']
-    ChART_color = plot_setup['chart color']
-    BINS = Integer(plot_setup['bins']) 
+    chart_color = plot_setup['chart color']
+    bins = int(plot_setup['bins']) 
     # kDE = plot_setup['kDE']
     dots_per_inch = plot_setup['dots per inch'] 
     extension = plot_setup['extension']
 
     
     # dataset and others information
     data = dataset['dataset']
-    COLUMN = dataset['column']
+    column = dataset['column']
  
     # Plot
     [w, h] = convert_si_to_inches_in_chart_size(w, h)
     sns.set(style = 'ticks')
-    fig, (ax_BOX, ax_hIST) = plt.subplots(2, figsize = (w, h), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
-    sns.boxplot(data = data, x = COLUMN, ax = ax_BOX, color = ChART_color)
-    sns.histplot(data = data, x = COLUMN, ax = ax_hIST, color = ChART_color, bins = BINS)
-    ax_BOX.set(yticks = [])
-    ax_BOX.set(xlabel = '')
-    FONT = {'fontname': 'DejaVu Sans',
+    fig, (ax_box, ax_hist) = plt.subplots(2, figsize = (w, h), sharex = True, gridspec_kw = {'height_ratios': (.15, .85)})
+    sns.boxplot(data = data, x=column, ax = ax_box, color = chart_color)
+    sns.histplot(data = data, x= column, ax = ax_hist, color = chart_color, bins = bins)
+    ax_box.set(yticks = [])
+    ax_box.set(xlabel = '')
+    font = {'fontname': 'DejaVu Sans',
             'color':  labels_color,
             'weight': 'normal',
             'size': labels_size}
-    ax_hIST.set_xlabel(xlabel = x_axis_label, fontDictionary = FONT)
-    ax_hIST.set_ylabel(ylabel = y_axis_label, fontDictionary = FONT)
-    ax_hIST.tick_params(axis = 'x', labelsize = x_axis_size, colors = axises_color)
-    ax_hIST.tick_params(axis = 'y', labelsize = y_axis_size, colors = axises_color)
+    ax_hist.set_ylabel(y_axis_label, fontdict=font)
+    ax_hist.set_xlabel(x_axis_label, fontdict=font)
+    ax_hist.tick_params(axis = 'x', labelsize=x_axis_size, colors=axises_color)
+    ax_hist.tick_params(axis = 'y', labelsize=y_axis_size, colors=axises_color)
     plt.grid()
-    sns.despine(ax = ax_hIST)
-    sns.despine(ax = ax_BOX, left = True)
+    sns.despine(ax=ax_hist)
+    sns.despine(ax=ax_box, left=True)
     plt.tight_layout()
-    
     # Save figure
     save_chart_in_folder(name, extension, dots_per_inch)
+    
+    # Show figure
+    plt.show()
+
 
 
 def line_chart(**kwargs):
     """
     This function shows a multiple lines in single chart.
 
     Args:
@@ -257,15 +280,38 @@
     save_chart_in_folder(name, extension, dots_per_inch)
 
     plt.show()
 
 
 def scatter_chart(**kwargs):    
     """
-    See documentation in: https://wmpjrufg.github.io/EASYPLOTPY/001-3.html
+    This function shows a scatter chart.
+
+    Args:
+        plot_setup (Dictionary): Setup chart Dictionary with the following keys:
+            name (String): Path + name figure (key required in plot_setup)
+            width (Float): Figure width in SI units (key required in plot_setup)
+            height (Float): Figure height in SI units (key required in plot_setup)
+            extension (String): File extension (key required in plot_setup)
+            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            marker size (List): List of marker sizes (key required in plot_setup)
+            color map (String or List): Color map for the scatter plot (key required in plot_setup)
+            y axis label (String): y axis label (key required in plot_setup)
+            x axis label (String): x axis label (key required in plot_setup)
+            labels size (Integer): Labels size (key required in plot_setup)
+            labels color (String): Labels color (key required in plot_setup)
+            x axis size (Integer): x axis size (key required in plot_setup)
+            y axis size (Integer): y axis size (key required in plot_setup)
+            axises color (String): Axises color (key required in plot_setup)
+            on grid? (Boolean): Grid on or off (key required in plot_setup)
+            y log (Boolean): y log scale (key required in plot_setup)
+            x log (Boolean): x log scale (key required in plot_setup)
+            
+    Returns:
+        None
     """
 
     # Setup
     dataset = kwargs.get('dataset')
     plot_setup = kwargs.get('plot_setup')
     name = plot_setup['name']
     w = plot_setup['width']
@@ -281,64 +327,54 @@
     axises_color = plot_setup['axises color']
     grid = plot_setup['on grid?']
     y_log_scale = plot_setup['y log']
     x_log_scale = plot_setup['x log']
     dots_per_inch = plot_setup['dots per inch']
     extension = plot_setup['extension']
 
-
-    # data
-    # data = dataset['dataset']
-    # data_nameS = List(data.columns)
-    # data_nameS = [i.upper() for i in data_nameS]
-    # data.columns = data_nameS
-    # X = data['X']
-    # Y = data['Y']
-    # Z = data['COLORBAR']
-
     # dataset and others information
     dataset = kwargs.get('dataset')
     dataset = keys_to_lower(dataset)
     data = dataset['dataset']
     x_dataset = []
     y_dataset = []
-    number_of_plots = Integer(len(data) / 2)
+    number_of_plots = int(len(data) / 2)
     for I in range(number_of_plots):
         x_column_name = f'x{I}'
         y_column_name = f'y{I}'
         x_dataset.append(data[x_column_name])
         y_dataset.append(data[y_column_name])
 
     # Plot
     w, h = convert_si_to_inches_in_chart_size(w, h)
     fig, ax = plt.subplots(1, 1, figsize=(w, h), sharex=True)
     
-    if isinstance(color_map, String):
+    if isinstance(color_map, str):
         scatter_plots = []
         for k in range(number_of_plots):
             scatter_plots.append(ax.scatter(x_dataset[k], y_dataset[k], marker='o', s=marker_size, cmap=color_map))
-        colorbar = plt.colorbar(scatter_plots[0])  # Use the first scatter plot as mappable
+        colorbar = plt.colorbar(scatter_plots[0]) 
     else:
         for k in range(number_of_plots):
             if len(color_map) == 1:
                 ax.scatter(x_dataset[k], y_dataset[k], marker='o', s=marker_size, c=color_map[0])
             else:
                 ax.scatter(x_dataset[k], y_dataset[k], marker='o', s=marker_size, c=color_map[k])
 
 
     if y_log_scale:
         ax.semilogy()
     if x_log_scale:
         ax.semilogx()
-    FONT = {'fontname': 'DejaVu Sans',
-            'color':  labels_color,
-            'weight': 'normal',
-            'size': labels_size}
-    ax.set_ylabel(y_axis_label, fontDictionary = FONT)
-    ax.set_xlabel(x_axis_label, fontDictionary = FONT)   
+    font = {'fontname': 'DejaVu Sans',
+                'color':  labels_color,
+                'weight': 'normal',
+                'size': labels_size}
+    ax.set_ylabel(y_axis_label, fontdict=font)
+    ax.set_xlabel(x_axis_label, fontdict=font)
     ax.tick_params(axis = 'x', labelsize = x_axis_size, colors = axises_color, labelrotation = 0, direction = 'out', which = 'both', length = 10)
     ax.tick_params(axis = 'y', labelsize = y_axis_size, colors = axises_color)
     if grid == True:
         ax.grid(color = 'grey', linestyle = '-', linewidth = 1, alpha = 0.20)
     plt.tight_layout()
 
     # Save figure
@@ -444,15 +480,15 @@
     data_nameS = List(data.columns)
     data_nameS = [i.upper() for i in data_nameS]
     data.columns = data_nameS
     ELEMENTS = List(data['CATEGORY'])
     VALUES = List(data['VALUES'])
     # Creating autocpt arguments
     def func(pct, allvalues):
-        absolute = Integer(pct / 100.*np.sum(allvalues))
+        absolute = int(pct / 100.*np.sum(allvalues))
         return "{:.2f}%\n({:d})".format(pct, absolute)
         
     # Plot
     w, h = convert_si_to_inches_in_chart_size(w, h)
     fig, ax = plt.subplots(1, 1, figsize = (w, h), subplot_kw = Dictionary(aspect = 'equal'))
     wEDGES, textensions, autotextensions = ax.pie(VALUES, autopct = lambda pct: func(pct, VALUES), textensionprops = Dictionary(color = Textension_color), colors = colors)
     ax.legend(wEDGES, ELEMENTS, loc_legend = 'center left', bbox_to_anchor = (1, 0.5), fontsize = legend_size)
@@ -487,16 +523,16 @@
     data_nameS = List(data.columns)
     data_nameS = [i.lower() for i in data_nameS]
     data.columns = data_nameS
     Y = data.drop(['group'], axis = 1, inplace = False)
     MIN_VALUE = min(List(Y.min()))
     Max_VALUE = max(List(Y.max()))
     N_DIV = 5
-    IntegerERVAL = (Max_VALUE - MIN_VALUE) / (N_DIV - 1)
-    RADAR_DIV = [round(MIN_VALUE + i * IntegerERVAL, 0) for i in range(N_DIV)]
+    interval = (Max_VALUE - MIN_VALUE) / (N_DIV - 1)
+    RADAR_DIV = [round(MIN_VALUE + i * interval, 0) for i in range(N_DIV)]
     RADAR_LABEL = [String(RADAR_DIV[i]) for i in range(len(RADAR_DIV))]
 
     # Plot
     w, h = convert_si_to_inches_in_chart_size(w, h)
     fig, ax = plt.subplots(1, 1, figsize = (w, h), subplot_kw = {'projection': 'polar'})
     CATEGORIES = List(data)[1:]
     N = len(CATEGORIES)
@@ -782,14 +818,38 @@
     
     # Save figure
     save_chart_in_folder(name, extension, dots_per_inch)
 
 
 def scatter_line_plot(dataset, plot_setup):    
     """
+    This function shows a scatter line chart.
+
+    Args:
+        plot_setup (Dictionary): Setup chart Dictionary with the following keys:
+            name (String): Path + name figure (key required in plot_setup)
+            width (Float): Figure width in SI units (key required in plot_setup)
+            height (Float): Figure height in SI units (key required in plot_setup)
+            extension (String): File extension (key required in plot_setup)
+            dots per inch (Integer): The resolution in dots per inch (key required in plot_setup)
+            marker size (List): List of marker sizes (key required in plot_setup)
+            color map (String or List): Color map for the scatter plot (key required in plot_setup)
+            y axis label (String): y axis label (key required in plot_setup)
+            x axis label (String): x axis label (key required in plot_setup)
+            labels size (Integer): Labels size (key required in plot_setup)
+            labels color (String): Labels color (key required in plot_setup)
+            x axis size (Integer): x axis size (key required in plot_setup)
+            y axis size (Integer): y axis size (key required in plot_setup)
+            axises color (String): Axises color (key required in plot_setup)
+            on grid? (Boolean): Grid on or off (key required in plot_setup)
+            y log (Boolean): y log scale (key required in plot_setup)
+            x log (Boolean): x log scale (key required in plot_setup)
+            
+    Returns:
+        None
     """
 
     # Setup
     name = plot_setup['name']
     w = plot_setup['width']
     h = plot_setup['height']
     marker_size = plot_setup['marker size']
@@ -836,19 +896,19 @@
     
     colorbar = plt.colorbar(im)
     if y_log_scale:
         ax.semilogy()
     if x_log_scale:
         ax.semilogx()
     font = {'fontname': 'DejaVu Sans',
-            'color':  labels_color,
-            'weight': 'normal',
-            'size': labels_size}
-    ax.set_ylabel(y_axis_label, fontDictionary=font)
-    ax.set_xlabel(x_axis_label, fontDictionary=font)   
+                'color':  labels_color,
+                'weight': 'normal',
+                'size': labels_size}
+    ax.set_ylabel(y_axis_label, fontdict=font)
+    ax.set_xlabel(x_axis_label, fontdict=font)  
     ax.tick_params(axis='x', labelsize=x_axis_size, colors=axises_color, labelrotation=0, direction='out', which='both', length=10)
     ax.tick_params(axis='y', labelsize=y_axis_size, colors=axises_color)
     if grid == True:
         ax.grid(color='grey', linestyle='-.', linewidth=1, alpha=0.20)
     save_chart_in_folder(name, extension, dpi)
```

### Comparing `easyplot_toolbox-0.0.0/license.md` & `easyplot_toolbox-1.0.0/license.md`

 * *Files identical despite different names*

### Comparing `easyplot_toolbox-0.0.0/readme.md` & `easyplot_toolbox-1.0.0/readme.md`

 * *Files identical despite different names*

### Comparing `easyplot_toolbox-0.0.0/PKG-INFO` & `easyplot_toolbox-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyplot-toolbox
-Version: 0.0.0
+Version: 1.0.0
 Summary: 
 Author: wmpjrufg
 Author-email: wanderlei_junior@ufcat.edu.br
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

