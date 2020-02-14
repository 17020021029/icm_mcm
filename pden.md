
## 潜在的密度


## 翻译
% SW_PDEN $Id: SW_PDEN。m,v 1.1 2003/12/12 04:23:22 pen078 Exp $

版权所有(C) CSIRO，菲尔摩根1992。

%

%使用情况:pden = sw_pden(S,T,P,PR)

%

%的描述:

%计算相对于规定的水质量的势密度

参考压力由pden = sw_dens(S,ptmp,PR)

%

%输入:(所有必须有相同的尺寸)

% S =盐度[psu (PSS-78)]

% T =温度[摄氏(ITS-90)]

% P =压力[db]

参考压力[db]

% (P可以有dims 1x1, mx1, 1xn或mxn表示S(mxn))

%

%输出:

% pden =相对于参考压力的电势密度[kg/m^3]
