# GEE_LST_Guangzhou
*解决广州市LST计算波段缺失问题的GEE代码*
## （一）核心问题：
* Landsat collection1 停用，GEE上跑不了，目前找到不存在波段缺失问题的代码用的都是collection1数据集
* Landsat8 c2 由于数据压缩导致B10波段缺失（来自CSDN某位老师）
## （二）解决思路：
* 用MODIS数据集算出来的LST填补缺失部分
* 用b10toa数据，发射率不要用asterged的（cr:小红书 @HowDopC）

## （三）最终方案
* MODIS
* B10toa （推荐）

***代码时间：20250613***