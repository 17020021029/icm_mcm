潜在的温度


% SW_PTMP $Id: SW_PTMP。m,v 1.1 2003/12/12 04:23:22 pen078 Exp $

版权所有(C) CSIRO，菲尔摩根1992。

%

%使用情况:ptmp = sw_ptmp(S,T,P,PR)

%

%的描述:

%根据联合国教科文组织1983年的报告计算潜在温度。

%

%输入:(所有必须有相同的尺寸)

% S =盐度[psu (PSS-78)]

% T =温度[摄氏(ITS-90)]

% P =压力[db]

参考压力[db]

%(对于S(mxn)， P & PR可以有dims 1x1, mx1, 1xn或mxn))

%

%输出:

% ptmp =相对于PR的潜在温度[摄氏度(ITS-90)]

%
