%SW_α热膨胀系数（α）

%================================================================

%西南阿尔法$编号：西南阿尔法，v 1.1 2003/12/12 04:23:22 pen078 Exp$

%版权所有（C）CSIRO，Nathan Bindoff 1993。

%

%用法：[ALPHA]=ALPHA（S，T，P，keyword）

%

%[α]=α（S，T，P，'temp'）%默认值

%[α]=α（S，PTMP，P，'PTMP'）

%

%说明：

%计算热膨胀系数的函数。

%

%输入：

%S=盐度[psu（PSS-78）]

%*PTMP=电位温度[摄氏度（ITS-90）]

%*T=温度[摄氏度（ITS-90）]

%P=压力[db]

%（对于S（mxn），P可能有尺寸1x1、mx1、1xn或mxn）

%

%keyword=用于标识temp或ptmp是否通过的可选字符串。

%=没有参数默认为“temp”

%‘temp’假设（S，T，P）通过。会执行得更慢

%因为ptmp将在内部计算。

%‘ptmp’假定（S，ptmp，P）通过。会执行得更快。

%

%输出：

%α=热膨胀系数（α）[摄氏度^-1]

%

%作者：N.L.Bindoff 1993，Lindsay Pender（Lindsay.Pender@csiro.au）

%

%免责声明：

%本软件按“原样”提供，不作任何保证。

%使用条件和许可证见sw_copy.m文件。

%

%参考：

%McDougall，T.J.1987年。”中性表面”

%物理海洋学杂志第17卷1950-1964页，

%

%检查值：

%见sw_beta.m和sw_aonb.m

%================================================================


%修改

%93-04-22号。Phil Morgan，帮助显示修改为适合库

%93-04-23号。Phil Morgan，输入参数检查

%2015年10月94日。Phil Morgan，通过S，T，P和“ptmp”的关键字

%99-06-25号。Lindsay Pender，行向量的固定转置。

%2012年12月3日。Lindsay Pender，改装成ITS-90。


%检查输入参数
