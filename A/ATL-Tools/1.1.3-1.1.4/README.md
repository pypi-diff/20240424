# Comparing `tmp/atl_tools-1.1.3.tar.gz` & `tmp/atl_tools-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atl_tools-1.1.3.tar", last modified: Thu Apr 18 10:35:35 2024, max compression
+gzip compressed data, was "atl_tools-1.1.4.tar", last modified: Wed Apr 24 06:59:00 2024, max compression
```

## Comparing `atl_tools-1.1.3.tar` & `atl_tools-1.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.449017 atl_tools-1.1.3/
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.445017 atl_tools-1.1.3/ATL_Tools/
--rw-rw-r--   0 atl       (1002) atl       (1002)    28826 2024-04-18 10:32:41.000000 atl_tools-1.1.3/ATL_Tools/ATL_gdal.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.3/ATL_Tools/ATL_path.py
--rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.3/ATL_Tools/__init__.py
-drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-18 10:35:35.449017 atl_tools-1.1.3/ATL_Tools.egg-info/
--rw-r--r--   0 atl       (1002) atl       (1002)     4545 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/SOURCES.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/dependency_links.txt
--rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-18 10:35:35.000000 atl_tools-1.1.3/ATL_Tools.egg-info/top_level.txt
--rw-r--r--   0 atl       (1002) atl       (1002)     4545 2024-04-18 10:35:35.449017 atl_tools-1.1.3/PKG-INFO
--rw-rw-r--   0 atl       (1002) atl       (1002)     4247 2024-04-18 10:34:04.000000 atl_tools-1.1.3/README.md
--rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-18 10:33:27.000000 atl_tools-1.1.3/pyproject.toml
--rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-18 10:35:35.449017 atl_tools-1.1.3/setup.cfg
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/ATL_Tools/
+-rw-rw-r--   0 atl       (1002) atl       (1002)    30179 2024-04-24 06:51:21.000000 atl_tools-1.1.4/ATL_Tools/ATL_gdal.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4295 2024-04-16 11:35:05.000000 atl_tools-1.1.4/ATL_Tools/ATL_path.py
+-rw-rw-r--   0 atl       (1002) atl       (1002)     2695 2024-04-16 11:17:35.000000 atl_tools-1.1.4/ATL_Tools/__init__.py
+drwxrwxr-x   0 atl       (1002) atl       (1002)        0 2024-04-24 06:59:00.921746 atl_tools-1.1.4/ATL_Tools.egg-info/
+-rw-r--r--   0 atl       (1002) atl       (1002)     4715 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)      222 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)        1 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 atl       (1002) atl       (1002)       10 2024-04-24 06:59:00.000000 atl_tools-1.1.4/ATL_Tools.egg-info/top_level.txt
+-rw-r--r--   0 atl       (1002) atl       (1002)     4715 2024-04-24 06:59:00.921746 atl_tools-1.1.4/PKG-INFO
+-rw-rw-r--   0 atl       (1002) atl       (1002)     4417 2024-04-24 06:58:56.000000 atl_tools-1.1.4/README.md
+-rw-rw-r--   0 atl       (1002) atl       (1002)      448 2024-04-24 06:58:55.000000 atl_tools-1.1.4/pyproject.toml
+-rw-rw-r--   0 atl       (1002) atl       (1002)       38 2024-04-24 06:59:00.921746 atl_tools-1.1.4/setup.cfg
```

### Comparing `atl_tools-1.1.3/ATL_Tools/ATL_gdal.py` & `atl_tools-1.1.4/ATL_Tools/ATL_gdal.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,16 @@
             geo_to_pix,         # 根据GDAL的仿射变换参数模型将给定的投影或地理坐标转为影像图上坐标（行列号）
             Mosaic_all_imgs,    # ✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
             Mosaic_2img_to_one, # 将两幅影像镶嵌至同一幅影像
             raster_overlap,     # 两个栅格数据集取重叠区或求交集（仅测试方形影像）
             crop_tif_with_json_zero, # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为0
             crop_tif_with_json_nan,  # ✔将带有坐标的图像按照json矢量进行裁切,无数据区域为nan,支持alpha
             Merge_multi_json,   # ✔将多个小的json合并为一个大的json,
-            resample_image      # ✔使用GDAL对图像进行重采样
+            resample_image,      # ✔使用GDAL对图像进行重采样
+            shp_to_geojson,      # ✔将shp文件转为geojson文件
         )
                             
     ________________________________________________________________
     >>> # 示例1-读取影像为数组并返回信息
     >>> img = read_img_to_array_with_info(img_path) # 读取图片，并输出图片信息
     ________________________________________________________________
     >>> # 示例2-读取影像为数组
@@ -153,14 +154,15 @@
         Datatype (int): 保存数据格式（位深），默认为6，GDT_Float32
 
     Returns: 
         输出影像文件
     """
 
     h,w,c= img_array.shape
+
     print(img_array.shape)
     driver = gdal.GetDriverByName("GTiff")
     ds = driver.Create(out_path, w, h, c, Datatype)
     if not Transform==None:
         ds.SetGeoTransform(Transform) 
     if not Projection==None:
         ds.SetProjection(Projection)  
@@ -255,15 +257,16 @@
     
     return np.linalg.solve(a, b)
     
 def Mosaic_all_imgs(img_file_path: str,
                     output_path: str,
                     add_alpha_chan: bool=False,
                     nan_or_zero: str='zero',
-                    output_band_chan: int=1) -> None:
+                    output_band_chan: int=1,
+                    img_list:List[str]=None) -> None:
     
     '''✔将指定路径文件夹下的tif影像全部镶嵌到一张影像上
         细节测试:
         mosaic图像：
         ✔ 镶嵌根据矢量裁切后的图像，无数据区域为nan
         ✔ 镶嵌矩形的图像，无数据区域为nan
         mosaic标签：
@@ -279,45 +282,50 @@
     Args:
         img_file_path (str)：tif 影像存放路径
         output_path (str): 输出镶嵌后 tif 的路径
         add_alpha_chan (bool): 是否添加alpha通道，将无数据区域显示为空白，默认为False
         Nan_or_Zero (str): 'nan'或'zero'镶嵌后的无效数据nan或0,默认为0
                            'nan'更适合显示，'0更适合训练'
         output_band_chan (int): 对于多光谱图像，如果只想保存前3个通道的话，指定通道数
+        img_list (List[str]):  需要镶嵌的影像列表，默认为None
         
         例子: Mosaic_all_imgs(img_path_all, output_path, add_alpha_chan=True) # 对于RGB标签，添加alpha通道
               Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为zero
               Mosaic_all_imgs(img_path_all, output_path, Nan_or_Zero='zero') # 对于float32 img，mosaic为nan #展示用
 
     Returns: 
         镶嵌合成的整体影像
     '''
 
     # os.chdir(img_file_path) # 切换到指定路径
     #如果存在同名影像则先删除
     if os.path.exists(output_path):
-        print(f"存在{output_path}, 已覆盖")
+        print(f"  【ATL-LOG】存在{output_path}, 已覆盖")
         os.remove(output_path)
 
-    all_files = find_data_list(img_file_path, suffix='.tif') # 寻找所有tif文件
+    # 如果不指定的话，就找所有的tif文件
+    if img_list == None:
+        print("  【ATL-LOG】未指定img_list, 寻找所有tif文件...")
+        all_files = find_data_list(img_file_path, suffix='.tif') # 寻找所有tif文件
+       
+    elif img_list != None:
+        print("  【ATL-LOG】指定img_list, 寻找指定的tif文件...")
+        all_files = img_list
     assert all_files!=None, 'No tif files found in the path'
+    print(f"  【ATL-LOG】本次镶嵌的影像有{len(all_files)}张")
 
     #获取待镶嵌栅格的最大最小的坐标值
     min_x,max_y,max_x,min_y=read_img_get_geo(all_files[0]) 
     for in_fn in all_files:
         minx, maxy, maxx, miny=read_img_get_geo(in_fn)
         min_x = min(min_x, minx)
         min_y = min(min_y, miny)
         max_x = max(max_x, maxx)
         max_y = max(max_y, maxy)
-    # print("待镶嵌栅格的最大最小的坐标值")
-    # print(f'min_x:{min_x}, min_y:{min_y}')
-    # print(f'max_x:{max_x}, max_y:{max_y}')
 
-    
     #计算镶嵌后影像的行列号
     in_ds=gdal.Open(all_files[0])
     geotrans=list(in_ds.GetGeoTransform())
     
     # 这一行代码获取了数据集的地理转换信息，包括地理坐标系的变换参数。
     # in_ds.GetGeoTransform() 返回一个包含六个浮点数的元组，
     # 分别表示左上角的X坐标、水平像素分辨率、X方向的旋转（通常为0）、
@@ -331,21 +339,20 @@
     columns=math.ceil((max_x-min_x)/width_geo_resolution) 
     rows=math.ceil((max_y-min_y)/(-heigh_geo_resolution))
     
     bands = in_ds.RasterCount  # 读进来的bands
     if not output_band_chan==None:
         bands = output_band_chan
         print("  【ATL-LOG】人为指定输出波段数为:", bands)
-    print(f'新合并图像的尺寸: {rows, columns, bands}')
+    print(f'  【ATL-LOG】新合并图像的尺寸: {rows, columns, bands}')
 
     in_band_DataType = in_ds.GetRasterBand(1).DataType
 
     driver=gdal.GetDriverByName('GTiff')
-    # out_ds=driver.Create(output_path, columns, rows, bands, in_band_DataType)
-    out_ds=driver.Create(output_path, columns, rows, 3, in_band_DataType)
+    out_ds=driver.Create(output_path, columns, rows, bands, in_band_DataType)
     out_ds.SetProjection(in_ds.GetProjection())
     geotrans[0] = min_x
     geotrans[3] = max_y
     out_ds.SetGeoTransform(geotrans)
 
 
     #定义仿射逆变换
@@ -357,27 +364,27 @@
         in_ds = gdal.Open(in_fn)
         in_gt = in_ds.GetGeoTransform()
         #仿射逆变换
         offset = gdal.ApplyGeoTransform(inv_geotrans, in_gt[0], in_gt[3])
         x, y = map(int, offset)
         # print(f'逆变换后的像素：x:{x}, y:{y}')
         # 该函数返回一个转换器对象 trans，可以使用这个对象执行从输入数据集到输出数据集的坐标转换
-        trans = gdal.Transformer(in_ds, out_ds, [])       #in_ds是源栅格，out_ds是目标栅格
-        success, xyz = trans.TransformPoint(False, 0, 0)  #计算in_ds中左上角像元对应out_ds中的行列号
+        trans = gdal.Transformer(in_ds, out_ds, [])       # in_ds是源栅格，out_ds是目标栅格
+        success, xyz = trans.TransformPoint(False, 0, 0)  # 计算in_ds中左上角像元对应out_ds中的行列号
         x, y, z = map(int, xyz)
         # print(f'小图(0, 0)变换到大图的像素：(x:{x}, y:{y}, z:{z})')
 
         for band_num in range(bands):
             # 小图的单通道，(h,w),无数据全是nan
             in_ds_array = in_ds.GetRasterBand(band_num + 1).ReadAsArray() #(h,w)
             # 无效数据的地方全是nan,这也符合下载下来的图，空缺的地方是nan、
             # 把nan的地方，用0替代
             in_ds_array = np.nan_to_num(in_ds_array, nan=0.)
 
-            # 大图的单通道，(h,w)，没数据的地方全是0
+            # 最后合并的大图的波段通道，(h,w)，没数据的地方全是0
             big_out_band = out_ds.GetRasterBand(band_num + 1)
             # 大图中，小图区域的数据
             Tiny_in_BigOut_data = big_out_band.ReadAsArray(x, y, in_ds_array.shape[1], in_ds_array.shape[0])
             Tiny_in_BigOut_data = np.nan_to_num(Tiny_in_BigOut_data, nan=0.)
             # 最后要写入大图的数据：如果是根据矢量裁切完的应该不会有重合，直接相加就行
             # 但是如果是矩形大图的话，有重叠的话，则需要舍弃小图的重叠部分。
             # 第一步：找到大图中有数据的区域：即大图不为零的地方
@@ -759,13 +766,43 @@
 
     # 使用gdal.Warp函数进行重采样
     gdal.Warp(output_path, input_ds, format='GTiff', width=new_cols, height=new_rows)
 
     # 关闭数据集
     input_ds = None
 
+def shp_to_geojson(input_shp: str, output_geojson: str) -> None:
+    """把 Shapefile 文件转换为 GeoJSON 文件
+    
+    Args:
+        input_shp (str): 输入的shp路径xxx.shp 
+        output_geojson (str): 输出的json路径xxx.json
+        
+    Returns:
+        保存输入的shp为Geojson
+    
+    示例：
+    >>> # 将一个shp文件转换为geojson文件
+    >>> shp_path = './nan值的shp文件/'
+    >>> shp_list = find_data_list(shp_path, '.shp')
+    >>> for shp_ in tqdm(shp_list):
+    >>> output_geojson = os.path.join('./nan的json/', os.path.basename(shp_).split('.')[0]+'.json')
+    >>> shp_to_geojson(shp_, output_geojson)
+
+    """
+    # 构建ogr2ogr命令
+    ogr2ogr_cmd = [
+        'ogr2ogr',   # 命令名称
+        '-f', 'GeoJSON',   # 输出格式为GeoJSON
+        output_geojson,    # 输出文件路径
+        input_shp   # 输入Shapefile文件路径
+    ]
+
+    # 调用ogr2ogr工具执行转换
+    subprocess.run(ogr2ogr_cmd)
+
```

### Comparing `atl_tools-1.1.3/ATL_Tools/ATL_path.py` & `atl_tools-1.1.4/ATL_Tools/ATL_path.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.3/ATL_Tools/__init__.py` & `atl_tools-1.1.4/ATL_Tools/__init__.py`

 * *Files identical despite different names*

### Comparing `atl_tools-1.1.3/ATL_Tools.egg-info/PKG-INFO` & `atl_tools-1.1.4/ATL_Tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -85,7 +85,8 @@
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
+- 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
```

### Comparing `atl_tools-1.1.3/PKG-INFO` & `atl_tools-1.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ATL_Tools
-Version: 1.1.3
+Version: 1.1.4
 Summary: AI-Tianlong的Tools打包，开箱即用, 包含ATL_path和ATL_gdal,可用于文件夹创建、文件搜索、遥感图像处理
 License: MIT License
 Keywords: ATL_Tools,GDAL,AI-Tianlong,Chinese
 Description-Content-Type: text/markdown
 
 # ATL_Tools 使用指南
 ## 0. 简介
@@ -85,7 +85,8 @@
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
+- 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
```

### Comparing `atl_tools-1.1.3/README.md` & `atl_tools-1.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -77,7 +77,8 @@
 - 2024-04-09 v1.0.7 修复ATL_gdal模块中对于ATL_path的引用，`__init__.py` 注释掉`from ATL_gdal import *`, 可不安装gdal使用ATL_Tools
 - 2024-04-16 v1.0.8 修复 `ValueError: cannot convert float NaN to integer` in ATL_gdal Line 371
 - 2024-04-16 v1.0.9 修复 修复`Mosaic_all_images()`对于mosaic RGB uint8标签的支持，优化`find_data_list()`函数显示，优化`_init_.py`, 优化`Readme.md`显示
 - 2024-04-16 v1.1.0 pypi页面增加`ATL_Tools`Github贡献地址。
 - 2024-04-16 v1.1.1 `crop_tif_with_json_nan()`增加可选参数`add_alpha_chan: bool`控制是否为RGB标签增加 alpha 通道
 - 2024-04-16 v1.1.2 修复 ATL_gdal Line 397 变量使用错误
 - 2024-04-18 v1.1.3 修复 ATL_gdal Mosaic中对float32图像背景设置为nan的支持
+- 2024-04-24 v1.1.4 修复 ATL_gdal Mosaic中指定img_list功能的支持，可以指定Mosaic的图像，增加`shp`转换为`Geojson`的功能函数`shp_to_geojson()`
```

