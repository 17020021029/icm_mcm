盐收缩系数

===============================================================

%SW=U Beta$id：SW=U Beta.M.V 1.1 2003//12/

%%Copyright（）CSIRO，Nathan Bindoff 1993.

页：1

%use:[（beta）]=sw \ \ u beta（、t、p、.keyword）]

页：1

%[（Beta）]=SW&U Beta（，T，P，'Temp'）%

%[[+Beta]=SW=U Beta（+S，PTMP，P，'PTMP'）

页：1

%

T.J.McDougall确定的盐收缩系数

页：1

%Input：（（all must have same dimensions）

%S=Salinity[（PSU）（（PSS-78））]

%*ptmp=potential temperature[×degree c（-90）]

%*t=温度[℃（-90）

%P=压力[DB]

%（p may have dims 1x1，mx1，1xn or mxn for s（）mxn）

页：1

%Keyword=Optional String to identify if Temp or PTMP passed.

%=No argument defaults to'

%=“Temp suspenses”（,t.p）passed.威尔执行慢动作

%as PTMP will be calculated internally.

%=“'PTMP suspenses”（S.ptmp.p）passed.Will Execute Faster.

页：1

输出

贝塔=盐收缩系数

页：1

%Author：N.L.Bindoff 1993，Lindsay Pender（（Lindsay.pender@csiro.au）

页：1

%Disclaimer：

%This software is provided as“without warranty of any kind.

%see the file sw@u copy.m for conditions of use and list.

页：1

%Reference：

“%McDougall，T.J.1987.”中性表面

%Journal of Physical Oceanography vol.17 pages 1950-1964，

页：1

%check value：

%beta=0.72088e-3 psu.^ 1 at S=40.0 psu，ptmp=10.0 c（-its-68），p=4000 db

===============================================================


%

93-04-22%Phil Morgan，help display modified to follow library

93-04-23%Phil Morgan，Input Argument Checking

%94-10-15.Phil Morgan，pass s，t，p and keyword for'

99-06-25%Lindsay Pender，固定矢量移植。

页：1Lindsay Pender，converted to its-90.


检查输入参数
