计算α/β（a对b）

%一、引用====

%SW AONB$版次：1.1$日期：2003/12/12 04:23:22$

%版权所有（C）CSIRO，Nathan Bindoff 1993

%

%用法：[AONB]=AONB（S，T，P，{keyword}

%

%[AONB]=AONB（S，T，P，'temp'）%默认值

%[AONB]=AONB（S，PTMP，P，'PTMP'）

%

%说明

%计算α/β。参见SW alpha.m和SW beta.m

%

%输入：（所有维度必须相同）

%S=盐度[psu（PSS-78）]

%*PTMP=电位温度[摄氏度（ITS-90）]

%*T=温度[摄氏度（ITS-90）]

%P=压力[db]

%（P可以有尺寸1x1、mx1、1xn或mxn表示S（mxn）

%

%keyword=用于标识temp或ptmp是否通过的可选字符串。

%=没有参数默认为'temp'

%“温度”假设（S，T，P）通过。会执行得更慢

%因为ptmp将在内部计算。

%='ptmp'假设（S，ptmp，P）通过。威尔跑得很快。

%

%输出

%AONB=α/β[psu/摄氏度]

%

%作者：N.L.Bindoff 1993，Lindsay Pender（Lindsay.Pender@csiro.au）

%

%免责声明：

%本软件按“原样”提供，不对任何儿童提供担保。

有关使用条件和许可证，请参阅swu copy.m文件。

%

%参考：

%McDougall，T.J.1987年。中性表面。”

%物理海洋学杂志第17卷1950-1964页，

%

%检查值：

%aonb=0.34763 psu C^-1，S=40.0 psu，ptmp=10.0 C，p=4000分贝

%一、引用====


%修改

%93-04-22号。Phil Morgan，帮助显示修改为适合库

%93-04-23号。Phil Morgan，输入参数检查

%2015年10月94日。Phil Morgan，通过S，T，P和'ptmp'的关键字

%99-06-25号。Lindsay Pender，行向量的固定转置。

%2012年12月3日。Lindsay Pender，改装成ITS-90。


%检查输入参数
