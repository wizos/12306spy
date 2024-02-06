# 12306spy

## 背景
从12306购票, 从A点到B点没有票, 但是可以补票或者多买一段票. 

比如一列车有100站, 我上车的站点是50 , 终点站是80. 需要保证我能上车,可以这样操作 : 
1. 补票类型 : 可以买 50-70的票, 然后再补70-80的票
2. 多买一段票 : 买20-80的票, 或者20-90, 这样多买了一段票, 但是保证了我能上车.
3. 多买且补票 : 买20-70的票, 然后再补70-80的票


## 配置
需要指定起始站,终点站,日期,车次,以及需要过滤的车次.
```python
#起始站-终点站,日期,车次
station_start = "赣榆"
station_end = "常州"
date = "2024-02-19"
filter_train_names = ["D2923"] 
```

## 如何使用 
### 1. windows : 
 点击`install.bat`安装依赖, 会自动打开浏览器. 修改第一个`cell`的配置信息, 点击运行全部,如下图所示.

<img src="resources/image.png" width=500   style="box-shadow: 2px 2px 2px 2px grey;">

### 2. linux :
1. 安装python3.7+
2. 安装依赖 `pip install -r requirements.txt`
3. 使用ide打开 `main.ipynb`修改最上面的配置信息, 点击jupyter的`全部运行`
4. 结果在jupyter的最后.



### 结果 : 按照价格排序
<img src="resources/img.png" style="box-shadow: 2px 2px 2px 2px grey;">

## ide推荐
- pycharm
- vscode + jupyter插件