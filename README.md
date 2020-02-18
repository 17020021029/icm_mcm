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

### 建模方法
#### 灰度模型（待研究）
没有可用的代码matlab
预测规则模糊，不知道如何确定第二问
#### 多元回归分析（舍弃）
确定主要因素对水温的影响函数
找到可变的因素，模拟多组数据，找到最好最坏情况，回答第二题

模拟出某一苏格兰地区的水温年际变化曲线，再根据洋流的特点模拟出温度随洋流的变化规律，模拟出近五十年每年的数据，达到合适温度即记录此时的位置

模拟水温后，鲱鱼和鲭鱼的习性、分布不同也会影响到后续分析

就目前思路来看，要考虑洋流等实际因素，因此模拟某一地区的水温变化只是一小部分
## 假设
1.鲱鱼鲭鱼的生境的主要性质水温，其他因素如浮游生物含量、盐分等海水热性质等 都与水温有直接的线性关系

使用的海温为海表温度，假设鲱鱼鲭鱼生存水层的水温相差不大或有线性关系，则用海表温度代表生境温度

2. 假设鲱鱼鲭鱼生境迁徙与目前的海温等温线梯度方向大体一致且每点的升温速度大致相等，则可用模拟曲线斜率值评估好坏情况
（具体可以再扩展）

3.预测成本 收益 净收益，数据处理同一二问，结合分析（经济学不是很懂

4.可以根据联合国海洋法公约等对领海公海的描述，查出所预测范围内各国领海及公海等，结合分析

## 数据处理过程
来源于美国海洋局，下载了2000-2018年1 7 10 月份 e330-e360，n50-n80 e0-e15，n50-n80 经纬度跨度都为1的海温数据，通过算法一获得各个点对应的2000-2018的海温数据，例如下图（表格1）

将海温数据带入灰度模型，得到预测的海温，横轴代表年份2000-2068，竖轴代表各个点，对应位置表中竖轴

####目前想到的等温线画法是得到横纵坐标对应的某一年的预测海温，正在尝试代码。。。然后还需要画出各年度某温度下的等温线，做好表格之后应该也好弄。。

可能要缩小纬度-> 50-75，个别不合理数据不知道会不会对画图有影响，先画画试试，可能没多大影响。

2.拟合每个点的海温线性变化曲线，斜率代表水温变化速度，舍掉不合理的点，取平均值-最可能情况，最大值-最坏情况，最小值-最好情况，进而分析

已经得到了拟合数值-水温变化，一把面条，####但是数据还是有问题，然后我另写了程序跑飞了。实在没心情弄了。。或许谁能改一下代码->代码能跑通了且已经得到了水温变化速度的拟合数据，现在的想法是通过概率来算最可能的速度和最快最慢的速度，如果是正态分布，则设置置信区间，找到最小值，最大值和最可能的值 利用海温数据，得到每点的水温数据，在得到等温线图，超出英国领海范围停止，记录年份：：：因此还要再写一份代码

## 步骤
q2:将第一问得到的数据进行拟合，得到了各个点的温度变化的拟合值

通过概率分析将拟合值的斜率（代表水温变化的速度），得到正态分布曲线，得到概率最高的斜率值，通过设置置信水平，得到置信区间，得到合理情况下的斜率最小值和最大值，代表最好和最坏情况

用概率分析得到的三个斜率值建立水温变化模型，即t=t0+斜率*年份。画出50年内，每隔十年的水温图

根据水温图，分析分别大概多少年

## 数据处理及错误
p1:开始使用的50-80的数据，带入灰度模型后得到的数据简单分析后，在76-80的数据误差很大 ，可能是以为高纬度地区的值由零下到零上的变化比较大

开始分析的是1 7 10月三个月份的数据，简单分析数据发现7 月温度是呈上升趋势的，1 10月有些点的温度有下降趋势，根据题目分析，结合鲱鱼 鲭鱼的捕捞时间，最终取7月份数据进一步分析

**结果：分析未来五十年内每隔十年的海温图，鲱鱼和鲭鱼的迁徙路线可能主要是从苏格兰附近海域沿北大西洋暖流到挪威附近迁徙，或者向格陵兰岛附近迁徙。

p2:用第一问得到的N50°-75°的海温数据进行拟合，得到了各点的温度变化，斜率即代表海温变化速度，通过概率分析得到了斜率的正态分布函数，u值为0.0924，置信区间0.0422-0.1446 （单位:℃/year）

error：得到的所有点的变化速度不仅相同 因此我们不断缩小范围得到了一个较可靠的正态分布函数，此过程中可能存在较大的误差，不是很严谨

结果：（因为三个温度变化速率 都相差0.05，所以最终分析的年份应该是相差五年左右，但是都是化的相差十年的图，那就大概一描述就可以，比如：根据分析得到的最可能的水温变化速度，最慢的和最快的水温变化速度，得到海温预测值，画出几十年后每隔十年的海温图，空白部分为陆地，见图（第一问模型里写的那个），分析英国领海大致范围，最好的情况是40年，最坏的情况是20年，最可能的情况是30年。

p3:用第一问建立的灰度模型分析找到的 鲱鱼鲭鱼捕获量-即某范围内各点的捕捞量，由于matlab能处理的数值有限，得到的预测值接近奇异，改换数量单位后有三个点的预测值非奇异，但不具有普遍性，因此得到的变化趋势不具有普遍性

## 更新
**附录：1.看到往年的论文里在附录中还加了各种折线图什么的，我觉得可以把第二问的面条，正态分布的图形加上

 2.或许前边添加的一些表格什么的也可以加在附录里显得更清晰
 
**创新点：1.海洋大学学生，接触过海洋学基本知识，找到了物理海洋学最基本的海水库，虽然真正用在建模上，但在分析问题上起到了很大作用，最终确定了用海温来预测鱼类迁徙的轨迹<\br>
2. 查阅了海洋法相关的内容，在问题三和四的分析上更加具有适用性<\br>
3.队员中有经管类学生，在问题三经营策略的分析上具有专业性，并提出了不限于问题提出的策略中的经营策略<\br>
4.模型得到的数据较为可靠。例如第一题分析得到鱼类向格陵兰岛和挪威方向迁徙，正好与北大西洋洋流的流向基本相同,且与此前专家预测的情况大致相同；第二问所得海温变化速度，最可能的是每年变化0.09摄氏度，每十年升高1摄氏度的规律也与此前的研究报告大致相同

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


