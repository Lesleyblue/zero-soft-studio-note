# 什么是响应式设计

### 响应式布局是Ethan Marcotte在2010年5月份提出的一个概念，简而言之，就是一个网站能够兼容多个终端——而不是为每个终端做一个特定的版本。这个概念是为解决移动互联网浏览而诞生的。
### 响应式布局可以为不同终端的用户提供更加舒适的界面和更好的用户体验，而且随着目前大屏幕移动设备的普及，用“大势所趋”来形容也不为过。随着越来越多的设计师采用这个技术，我们不仅看到很多的创新，还看到了一些成形的模式。

#### 优点
##### 面对不同分辨率设备灵活性强
##### 能够快捷解决多设备显示适应问题

#### 缺点
##### 兼容各种设备工作量大，效率低下
#####  代码累赘，会出现隐藏无用的元素，加载时间加长
#####  其实这是一种折中性质的设计解决方案，多方面因素影响而达不到最佳效果
#####  一定程度上改变了网站原有的布局结构，会出现用户混淆的情况

### 其中一种响应式设计为media Query（媒体查询）
### 在css样式中有两种应用方式：

####  一种是直接在link中判断设备的尺寸，然后引用不同的css文件

```
<link rel="stylesheet" type="text/css" href=" css文件" media="媒体类型 and (媒体功能)  ">

```
#### 另一种是在样式表中内嵌@media

```
@media 媒体类型 and (媒体功能){
    
}

```
| 媒体类型  | 描述|
|:-:|:-:|
|screen |  计算机屏幕（默认）|
|print      |  打印预览模式/打印页面|
|all |适用于所有设备|
|speech|屏幕阅读器等发声设备|



|媒体功能|  描述|
|:-:|:-:|
|aspect-ratio    |定义输出设备中的页面可见区域宽度与高度的比率|
|color   |定义输出设备每一组彩色原件的个数。如果不是彩色设备，则值等于0|
|device-height   |定义输出设备的屏幕可见高度|
|device-width    |定义输出设备的屏幕可见宽度|
|max-aspect-ratio|定义输出设备的屏幕可见宽度与高度的最大比率    |
|max-color-index |定义在输出设备的彩色查询表中的最大条目数|
|max-device-aspect-ratio |定义输出设备的屏幕可见宽度与高度的最大比率|
|max-device-height   |定义输出设备的屏幕可见的最大高度|
|max-device-width    |定义输出设备的屏幕最大可见宽度|
|max-height  |定义输出设备中的页面最大可见区域高度|
|max-width  |定义输出设备中的页面最大可见区域宽度|
|min-aspect-ratio   |定义输出设备中的页面可见区域宽度与高度的最小比率|
|min-color | 定义输出设备每一组彩色原件的最小个数 |
|min-color-index |定义在输出设备的彩色查询表中的最小条目数|
|min-device-width   |定义输出设备的屏幕最小可见宽度|
|min-device-height   |定义输出设备的屏幕的最小可见高度|
|min-height |定义输出设备中的页面最小可见区域高度|
|min-resolution  |定义设备的最小分辨率|
|min-width   |定义输出设备中的页面最小可见区域宽度|
|width   |定义输出设备中的页面可见区域宽度|
|height|定义输出设备中的页面可见区域高度|
