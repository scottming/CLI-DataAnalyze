## 观察数据

### 查看文件（csv）unicode 

* 识别率要高，识别类型要广。比如识别 GB18030、GBK 数据

### 观察头部、尾部数据

* 能自定义观看条数

### 各列变量类型

*  能识别数值型（numeric）、分类型（category）、字符型（string）

- example

 ![](http://7xqyb4.com1.z0.glb.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202016-09-11%20%E4%B8%8B%E5%8D%8811.30.25.png)

### 缺失值

* 各变量缺失值具体数值与所占百分比

## 清洗数据

* 待定

## 描述数据

* 针对数值型、分类型进行描述
* 输出下图表格

![](http://7xqyb4.com1.z0.glb.clouddn.com/%E5%B1%8F%E5%B9%95%E5%BF%AB%E7%85%A7%202016-09-07%20%E4%B8%8B%E5%8D%886.54.30.png)

-  连续变量字段说明（Continuous Features）
	+ Feature: 列变量
	+ Count: 各列行总数
	+ Miss(%): 列变量缺失百分比
	+ Card: 连续变量不同数值的统计（比如价格有 100 个观察值，其中 1 个缺失，有 9 个数值相同，则 Card 为 90）
	+ Min: 最小值
	+ 1st Qrt: 第 25 位百分数
	+ Mean:  平均值
	+ Median: 中位数
	+ 3rd Qrt: 第 75 位百分数
	+ Max: 最大值
	+ Std Dev: 标准差

-  分类变量字段说明（ Category Features）
	+ Feature: 列变量
	+ Count: 各列行总数
	+ Miss(%): 列变量缺失百分比
	+ Card: 属性数量（比如性别，只有男与女，属性数量为 2）
	+ Mode: 频次最高的属性名称（比如性别男性 80 人 ，女性 20 人，Mode 为男性）
	+ Mode Freq:频次最高的属性统计个数（80）
	+ Mode(%):  频次最高的属性统计个数百分比（80 % = 80 / 100）
	+ 2nd Mode: 频次第二高的属性名称（女）
	+ 2nd Mode Freq: 频次第二高的属性统计个数（20）
	+ 2nd Mode(%): 频次第二高的属性统计个数百分比（20 %）

