---
title: "假如钥匙丢了应该怎么找？概率密度估算"
date: 2022-09-12T11:22:30-04:00
categories:
  - blog
tags:
  - Searching Algorithm
  - Interesting but useless 
excerpt: "Who doesn't like math?"
---
<script type="text/javascript" async
src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.7/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

最近帮婉茹找钥匙突发奇想:假如回到家发现钥匙掉了，该怎么找呢？

首先模型离散化，一个无序序列，乍一想是遍历寻找就ok了，每个地方掉的几率是一样的，trivial。但是其实这个序列其实是有序的，因为假如很早就掉了，后面就不会再掉了，假如很晚掉的，说明之前没有掉，这样一想，假设掉落几率是常函数=c<1（时间和距离就作一个变量，因为回家的时候假设走路的速度不变是线性的），能得到结论只要c<1,都是有可能到家还有钥匙的，所以路上掉的可能性<1，而且容易发现随着距离/时间变大，掉的几率越小（之前没掉的几率*c）。

但假如不是常函数呢，建立一个随着时间掉落几率越来越大的模型也是很合理，比如钥匙挂在书包上，每走一步往下掉一点。由这个理念，我们建立如下概率函数f: f(x)为概率密度，F(x)为 0-x为真的可能性即f的积分，G表示有钥匙的时候每一个点掉钥匙的概率函数, $\mathbf{f=G(x)(1-F(x))}$ 。若为之前的常函数模型，$f=c\*(1-F)$易得$F=1-exp(-cx)$(初始条件$x=0,F=0$)$,f=c\*exp(-cx)$,概率确实是递减的。若是钥匙掉在越后面概率越大的情况，i.e. $\\frac{df}{dx}=\\frac{d^2 F}{dx^2}>0$, 展开后化简为$\\frac{dG'}{G}>-\frac{d(1-F)}{1-F}$, 解得$G>\\frac{G_0}{1-F}$, 代入常函数模型验证正确。若我们想要钥匙掉在任何地方的概率相等假设$f=c,F=cx$,易得$G(x)= \\frac{c}{1-cx}$，代入不等式果然取等。

回到概率函数f的微分方程，可得通解$\\mathbf{F=1-exp(-\\int_0^x G(x') dx')}$,代入以上不等式得$ln(\frac{G(x)}{G(0)})> \\int_0^x G(x') dx'$(钥匙不等式)时钥匙掉在越后面概率越大(对于验证该不等式的点x)，反之亦然。(当然也可以用F(总路程/2)和0.5比较，总之有各种决定办法。)所以钥匙掉了不要急，根据记得钥匙最后拿着的位置，建立合理的物理模型G，代入钥匙不等式就能知道掉钥匙的概率分布，就知道该从前往后找还是从后往前找了，大部分时候都应该从前往后找。  

Second thought, if you are at home right now, you'll probably start looking from home to school and vice versa. So I guess calculating a probability density isn't all that useful. But if you are on a bike...

May 20, 2023 update: We found the key at last in one of my girlfriend's pants unexpectedly...
