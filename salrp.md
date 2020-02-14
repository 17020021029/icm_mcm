电导率Rp(S,T,P) = C(S,T,P)/C(S,T,0)


% SW_SALRP $Id: SW_SALRP。m,v 1.1 2003/12/12 04:23:22 pen078 Exp $

版权所有(C) CSIRO，菲尔摩根1993。

%

%使用情况:Rp = sw_salrp(R,T,P)

%

%的描述:

公式Rp(S,T,P) = C(S,T,P)/C(S,T,0)

%联合国教科文组织1983多项式。

%

%输入:(所有形状必须相同)

% R =电导率R = C(S,T,P)/C(35,15(IPTS-68)，0)[无单元]

% T =温度[摄氏(ITS-90)]

% P =压力[db]

%

%输出:

Rp(S,T,P) = C(S,T,P)/C(S,T,0)[无单位]
