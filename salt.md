盐度来自cndr, T, P

% = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =

$Id: SW_SALT。m,v 1.2 2004/03/18 20:27:03 pen078 Exp $

版权所有(C) CSIRO，菲尔摩根1993。

%

%用量:S = sw_salt(cndr,T,P)

%

%的描述:

%根据电导率计算盐度。联合国教科文组织1983年多项式。

%

%的输入:

% cndr =电导率R = C(S,T,P)/C(35,15(IPTS-68)，0)[无单位]

% T =温度[摄氏(ITS-90)]

% P =压力[db]

%

%输出:

% S =盐度[psu (PSS-78)]
