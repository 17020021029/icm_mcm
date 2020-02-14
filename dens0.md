## 大气压海水密度
海水的密度是指单位体积内海水的质量。海水密度一般在1.02～1.07之间，它取决于温度、盐度和压力(或深度)。在低温、高盐和深水压力大的情况下，海水密度大。而在高温、低盐的表层水域，海水密度就小。一般情况下，由赤道向两极，温度逐渐变低，密度则逐渐变大。到了两极海域，由于水温低，海水结冰，剩下的海水盐分高，所以密度更大
## 翻译
大气压海水密度

%=========================================================================

%编号：SW_DENS0.m，v 1.1 2003/12/12 04:23:22 pen078 Exp$

%版权所有（C）CSIRO，Phil Morgan 1992

%

%用法：dens0=sw_dens0（S，T）

%

%说明：

%大气压下海水密度

%联合国教科文组织1983（EOS 1980）多项式。

%

%输入：（所有维度必须相同）

%S=盐度[psu（PSS-78）]

%T=温度[摄氏度（ITS-90）]

%

%输出：

%dens0=具有S、T特性的盐水密度[kg/m^3]，

%P=0（0分贝表压）

%

%作者：Phil Morgan 92-11-05，Lindsay Pender（Lindsay.Pender@csiro.au）

%

%免责声明：

%本软件按“原样”提供，不作任何保证。

%使用条件和许可证见sw_copy.m文件。