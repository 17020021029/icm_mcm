西南GPAN位势异常

%版权所有（C）CSIRO，Phil Morgan 1992。

%

%用法：[gpan]=sw_gpan（S，T，P）

%

%说明：

%作为svan积分计算的位势异常

%海面到海底。因此相对于海面。

%

%输入：（所有维度必须相同）

%S=盐度[psu（PSS-78）]

%T=温度[摄氏度（ITS-90）]

%P=压力[db]

%（对于S（mxn），P可能有尺寸1x1、mx1、1xn或mxn）

%

%输出：

%GPAN＝位势异常[M^ 3 kg^ - 1 Pa=＝m ^ 2 s^ - 2＝j kg^－1 ]
