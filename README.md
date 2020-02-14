# icm_mcm
## Problem A
与英格兰鲱鱼和鲭鱼当全球海洋气温升高时从他们现在栖息地开始的潜在迁移有关的问题.
1. 建立一个数学模型，以识别未来 50 年内这两种鱼类最可能的位置，假设水温将发 生足够的变化以导致种群移动。 
 
2. 根据海水温度变化发生的速度，使用您的模型预测最佳情况，最坏情况以及最可能经 过的时间，直到小型渔业公司继续捕捞这些种群将使小型渔业公司无法收获为止在其当 前位置之外进行操作。 
 
3. 根据您的预测分析，这些小型捕捞公司是否应该改变其经营方式？ 
 
a. 如果是，请使用您的模型为小型捕捞公司识别和评估实用且经济上有吸引力的 策略。您的策略应考虑但不限于现实的选择，包括： - 将渔业公司的部分或全部资产从苏格兰港口的当前位置迁移到两个鱼类种 群都移动的附近； - 使用一定比例的小型渔船，这些渔船可以在没有陆上支持的情况下运行一 段时间，同时仍确保渔获物的新鲜度和高质量。 - 您的团队可能会识别和建模的其他选项。 b. 如果您的团队拒绝进行任何更改，请根据您的建模结果说明拒绝的理由，因 为它们与您的团队所做的假设有关。 

4.使用你的模型来说明如果某一比例的鱼进入另一个国家的领海（海），你的提案会受到怎样的影响

5.除了你的技术报告。为410杂志准备一到两页的文章，帮助渔民了解问题的严重性以及你提出的解决方案将如何改善他们未来的商业前景
### 鲱鱼
鲱鱼属季节性鱼类，鲱科，冷水性上层洄游性鱼类。

## 数学模型
求出各纬度水温随时间的变化曲线，包括各种影响因素，其中有些因素可变。</br>
1.确定最可能的影响因素，获得预测结果</br>
2.使可变因素可变，找到最好、最坏、以及最可能的情况。水温变化曲线斜率评价好坏</br>
3.根据第二问结果及渔业规律合理推断</br>
4.根据《国际海洋法》内容</br>
5.杂志文章，需要找一些参考文章，尽量写好</br>https://wenku.baidu.com/view/1aab598469eae009591bec6e.html

## 数据来源
https://oceanwatch.pifsc.noaa.gov/erddap/info/index.html?page=1&itemsPerPage=1000

https://www.metoffice.gov.uk/services/data/datapoint
## 海水库
md文件是海水库代码的注释</br>
s 盐度 t 温度 p 压力

adtg 绝热温度梯度(s,t,p)

alpha 热膨胀系数(s,t,p,keyword=用于标识temp或ptmp是否通过的可选字符串。)

beta 盐收缩系数(s,t,p,keyword)

aonb alpha/beta

bfrq 维萨拉布伦特频率平方/浮力频率(s,t,p,lat)

c3515 在S=35PSU，T=15C[ITPS 68]和P=0dB时返回电导率。

cndr 电导率(s,t,p)

cp 海水热容量(s,t,p)

dens0 大气压海水密度(s,t)

dist 距离（经度，纬度，单位）

dpth 距压力的深度（p，lat）

f 科里奥利系数(lat)

fp 海水冰点

g 重力加速度(lat,z高度)

gpan 位势异常 （s,t,p）

gvel 地转速度 
% INPUT:
%    ga   = geopotential anomoly relative to the sea surface.
%           dim(mxnstations)
%    lat  = latitude  of each station (+ve = N, -ve = S) [ -90.. +90]
%    lon  = longitude of each station (+ve = E, -ve = W) [-180..+180]

pden 潜在的密度(s,t,p,pr)

pres 深度的压力(深度，北纬十进度lat）

ptmp 潜在的温度（s,t,p,pr）

salds 

salrp 电导率(r,t,p) r =  C(S,T,P)/C(35,15(IPTS-68),0) 

sals 海水盐度(rt,t) Rt = Rt(S,T) = C(S,T,0)/C(35,T(IPTS-68)，0)

salt 盐度(t,p)

satar 海水中砷的含量

seck 海水体积模量(K)的正割（s,t,p）

smow 标准平均海水(纯水)密度(t)

svan 具体体积异常（S,T,P）

svel 海水声速

swvel 表面波声速

temp 位温引起的温度

test 测试海水图书馆例行程序


