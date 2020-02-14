# icm_mcm
## Problem A
与英格兰鲱鱼和鲭鱼当全球海洋气温升高时从他们现在栖息地开始的潜在迁移有关的问题
## 鲱鱼
鲱鱼属季节性鱼类，鲱科，冷水性上层洄游性鱼类。
## 代码含义
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


