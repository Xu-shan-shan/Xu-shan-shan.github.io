---
title: Implementing .shp boundaries for batch cropping TIF images with Python, processed with some errors
date: '2021-03-01T22:08:31'

# Summary for listings and search engines
summary: A simple python code for batch cropping of .shp file boundaries 

subtitle: "A useful but imperfect python code for batch cropping of TIF image files at .shp file boundaries"

# Link this post with a project
projects: []

# Date published
date: '2022-09-22T23:08:21'

# Date updated
lastmod: '2023-12-22T23:08:21'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: ''
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - Python
  - Tutorials

categories:
  - Python
  - Tutorials


---

## Causes
Because the .nc original image to tiff format is also processed by the code, there is some error in the data inside after cropping. No reason for this has been found

## Ideas
The following code can be compiled with the GUI compiler that comes with ARCGIS, and can also be compiled with the python that comes with ARCGIS PRO, which is also on the Internet to find the relevant code for modification, the source code is now impossible to find, there are a lot of the Internet, and you should have viewed in the process of searching again.

## Realization: python code
```python
import arcpy
import os
 
arcpy.CheckOutExtension("spatial")
 
arcpy.env.workspace = "H:/LAB/LABDATA/ECMWF/3/TIF/si10" # 工作目录
 
rasters = arcpy.ListRasters("*", "TIF") # 获取所有的TIF影像
 
mask= "H:/LAB/LABDATA/landsat/shp/caohai2013.shp" # 获取掩膜边界
 
for raster in rasters:
 
    print(raster)
 
    out= "H:/LAB/LABDATA/ECMWF/3/TIF/caohai/si10/"+"clip_"+raster # 输出路径及文件名
 
    arcpy.Clip_management(raster,"#", out, mask, "0", "ClippingGeometry") # arcpy调用ARCMAP里的Clip工具
 
    print("clip_"+raster+"  has done")
 
print("All done")
```
The results are for reference only, if no errors are reported in the middle, when you see this information as shown, it should be correct!



**This blog first appeared on [CSDN](https://blog.csdn.net/weixin_47818240/article/details/114272879)**
