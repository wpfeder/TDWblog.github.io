<dependency>
    <groupId>com.github.houbb</groupId>
    <artifactId>markdown-toc</artifactId>
    <version>${maven-version}</version>
</dependency>

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
