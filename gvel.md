地转速度

% = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = = =

% GEOVEL $Id: sw_gvel。m,v 1.1 2003/12/12 04:23:22 pen078 Exp $

版权所有(C) CSIRO，菲尔摩根1992

%

%使用情况:vel = sw_gvel(ga,lat,lon)

%

%的描述:

根据位势异常计算地转速度

和各工位的位置。

%

%的输入:

相对于海面的位势异常。

%的(mxnstations)

% lat =各站纬度(+ve = N， -ve = S) [-90.]+ 90)

% lon =各站经度(+ve = E， -ve = W) [-180..+180]

%

%输出:

相对于海面的地转速度。

%的(m, nstations-1)
