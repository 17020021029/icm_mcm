## 注释翻译
%SW_-ADTG绝热温度梯度

%===========================================================================

%编号：SW_ADTG.m，v 1.1 2003/12/12 04:23:22 pen078 Exp$

%版权所有（C）CSIRO，Phil Morgan 1992。

%

%adtg=sw_adtg（S，T，P）

%

%说明：

%根据联合国教科文组织1983年的惯例计算绝热温度梯度。

%

%输入：（所有维度必须相同）

%S=盐度[psu（PSS-78）]

%T=温度[摄氏度（ITS-90）]

%P=压力[db]

%（对于S（mxn），P可能有尺寸1x1、mx1、1xn或mxn）

%

%输出：

%ADTG=绝热温度梯度[摄氏度/分贝]

%

%作者：Phil Morgan，Lindsay Pender（Lindsay.Pender@csiro.au）

%

%免责声明：

%本软件按“原样”提供，不作任何保证。

%使用条件和许可证见sw_copy.m文件。

%

%参考文献：

%Fofonoff，P.和Millard，R.C.Jr

%联合国教科文组织1983年。基本性质的计算算法

%海水。联合国教科文组织技术部。《科学》3月第44、53页，第31页，第39页

%

%布莱登，H.1973。

%“新的热膨胀多项式，绝热温度梯度

%以及海水的潜在温度。”

%《深海研究》，1973年，第20401-408卷。

%=========================================================================


%修改

%99-06-25号。Lindsay Pender，行向量的固定转置。

%2012年12月3日。Lindsay Pender，改装成ITS-90。


%-------------

%检查输入
## 参数含义
根据压力、水温、盐度计算海洋绝热梯度

