# About Mathmatica

## 快捷键
shift+Enter 计算

## 计算

**积分**
```
Integrate[f[x],x]
Integrate[f[x],{x,x_inf,x_sup}]
Integrate[f[x1,x2,...,xn],{x1,x1_inf,x1_sup},{x2,x2_inf,x2_sup},...,{x_n,xn_inf,xn_sup}]

ImplicitRegin[#eq/odds,{x1,x2,...,xn}]#多个等式或不等式间用&&连接
ParmetricRegion[{f1,f2,...,fn},{x1,x2,...,xn}]#由多个函数表达式给定的区域
```
**矢量图计算**
```
#流线图
Module[{mu, g, L}, mu = 0.5; g = 9.8; L = 4;
StreamPlot[{y, -mu y - (g/L) Sin[x]}, {x, -5, 5}, {y, -5, 5}]]

#矢量图
Module[{mu, g, L}, mu = 0.5; g = 9.8; L = 4;
VectorPlot[{y, -mu y - (g/L) Sin[x]}, {x, -5, 5}, {y, -5, 5}]]

#解微分方程
mu = 0.5; g = 9.8; L = 4;
sol = NDSolveValue[{x''[t] == -mu x'[t] - (g/L) Sin[x[t]], 
x[0] == Pi/3, x'[0] == 0}, x, {t, 0, 10}]; 
Plot[sol[\[FormalX]], {\[FormalX], 0., 10.}]
 ```
 
