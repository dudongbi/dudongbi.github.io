---
title: jm6s1
date: 2008-12-30 12:28:50
tags: jm
---

# 第八章 重积分和曲线积分

## 1. 重积分

1. 二重积分的直接计算法：所谓连续函数\( f(x,y) \)展布在有限封闭可求积二位域\( \Omega \)内的二重积分乃是指的数

\[
\iint_{D} f(x, y) d x d y
= \lim_{\substack{m y+\left|\Delta \Delta_{n}\right| \\ \max \left|\Delta y_{1}\right| \rightarrow 6}}
\sum_{i} \sum_{j} f\left(x_{1}, y_{2}\right) \Delta x_{1} \Delta y_{1}
\]

其中\( \delta x_i = x_{i+1} - x_i \), \( \delta y_i = y_{i+1} - y_i \)，而其和为对所有\( i,j \)使\( (x_i, y_i) \in \Omega \)
的那些悳杀水的\( j_i \)

若域\( \Omega \)由目的不等式所给定

\[
a \leqslant x \leqslant b, y_{1}(x) \leqslant y \leqslant y_{2}(x)
\]

其中\( y_1(x) \)和\( y_2(x) \)为在闭区间\( [a,b] \)上的连续函数，则对应的二重积分。

2. 二重积分中的变量代换：若可微分的连续函数
把平面\( Oxy \)上的有限闭域\( \Omega \)单值唯一地映射为平面\( Ouv \)上的域\( \Omega' \)及

\[
\iint_{\Omega} f(x, y) d x d y=\int_{a}^{b} d x \int_{y_{1}(x)}^{y_{2}(x)} f(x, y) d y .
\]

\[
x=r(u, v), y=y(u, v)
\]

雅撷比式

\[
I=\frac{D(x, y)}{D(u, v)} \neq 0,
\]

则下之公式玉确：

\[
\int_{u}^{n} f(x, y) d x d y=\int_{a} f(x(u, v), y(u, v))|I| d u d v .
\]

特别是，根据公式\( x=r\cos\varphi, y=r\sin\varphi \)变换为极坐标\( r \)和\( \varphi \)的情形，有

\[
\iint_{a} f(x, y) d x d y=\iiint f(r \cos \varphi, r \sin \varphi) r d r d \varphi .
\]

3901. 把积分\( \iint_{0} x y d x d y \)当胙积分和的极垠, 由直线

\[
x=\frac{i}{n}, y=\frac{j}{n}(i, j=1,2, \cdots, n-1)
\]

把秎分域分力许多正方形，并选取被积函数在这些王方形之右顶点的值，计算所论积分的值

解：由

\[
\sum_{i=1}^{n} \sum_{1=1}^{n} \frac{i}{n} \cdot \frac{j}{n} \cdot \frac{1}{n^{2}} \cdot \frac{n^{2}(n+1)^{2}}{4 n^{5}} \rightarrow \overbrace{4}^{1} \quad(n \rightarrow
\]

其中

\[
\sum_{i=1}^{n} i=\frac{n(n+1)}{2}, \sum_{j=1}^{n} j=\frac{n(n+1)}{2},
\]

故

\[
\iint\limits_{\substack{0\leqslant x\leqslant1 \\ 0\leqslant x\leqslant1}}
xydxdy = \frac14
\]

3902. 用直线

\[
x=1+\frac{i}{n}, y=1+\frac{2 j}{n}(i, j=0,1, \cdots, n)
\]

把域\(1 \leqslant x \leqslant 2,1 \leqslant y \leqslant 3\)分为许多矩形.
作出函数\( f(x, y)=x^{2}+y^{2} \)在此域内的积分下和\( S \)与积分上和\( S \). 
当\( n \rightarrow \infty \)时上和.
与下和的柘限等于们么?

下和

\[
\begin{aligned}
S & \left.=\sum_{i=0}^{n-1} \sum_{j=0}^{N-1}\left(\mid 1+\frac{i}{n}\right)^{2}+\left(1+\frac{2 j}{n}\right)^{2}\right) \cdot \frac{1}{n} \cdot \frac{2}{n} \\
= & \frac{2 n}{n^{2}}\left[n+\frac{2}{n} \sum_{1-0}^{n-2} i+\frac{1}{n^{2}} \sum_{i=0}^{n-1} i^{2}+n+\frac{4}{n} \sum_{j=n}^{n-1} j\right. \\
& \left.\quad+\frac{4}{n^{2}} \sum_{r=0}^{n-1} j^{2}\right) \\
= & \frac{40}{3}-\frac{11}{n}+\frac{5}{3 n^{2}}
\end{aligned}
\]

荮草

\[
\begin{aligned}
& \sum_{i=n}^{n} i^{2}=\frac{(n-1) n(2 n-1)}{6}, \\
& \sum_{i=0}^{n} j^{2}=\frac{(n-1) n(2 n-1)}{6} ;
\end{aligned}
\]

用上和

\[
\begin{aligned}
\bar{S}= & \left.\sum_{i=1}^{n} \sum_{i=1}^{n}\left(11+\frac{i}{n}\right)^{2}+\left(1+\frac{2 j}{n}\right)^{2}\right) \cdot \frac{1}{n} \cdot \frac{2}{n} \\
& =\frac{40}{3}+\frac{11}{n}+\frac{5}{3 n^{2}}
\end{aligned}
\]

当\( n\to \infty \)时，\( \underline{S} \)和\( \bar{S} \)的极限均等于\( \frac{40}3 \)

3903. 用系列内接正方形作为积分域的近似域这些止方形的顶点\( A_u \)，
在晸数点并取被积函数在每个功讴形喍原点的最迁的顶点之值近似地计算积分

\[
\int_{y^{2}:=25}-\frac{d x d y}{\sqrt{24+x^{2}+y^{2}}}
\]

并与精确的值加以比较。

解：由题意矨愔取的正方形顶点为\( (1,1) (1,2),(1,3) (1,4),(2.1),(2,2),(2,3),(2,4),(3,1),(3,2), (3,3),(3,4),(4,1),(4,2),(4,3)\), 故利用对称性知

\[
\begin{aligned}
\frac{1}{4} \iint_{x^{2}+y^{2}<25} \frac{d x d y}{\sqrt{24+x^{2}+y^{2}}} \doteq \frac{1}{\sqrt{26}}+\frac{2}{\sqrt{29}}+\frac{2}{\sqrt{34}} \\
+\frac{2}{\sqrt{41}}+\frac{1}{\sqrt{32}}+\frac{2}{\sqrt{37}}+\frac{2}{\sqrt{44}}+-\frac{1}{\sqrt{42}}+\frac{2}{\sqrt{49}} \\
\doteq 0.196+0.371+0.343+0.312+0.177 \\
+0.329+0.302+0.154+0.285 \\
\doteq 2.470
\end{aligned}
\]

即

\[
\iint_{x^{2}+y^{2} \in 25} \frac{d x d y}{\sqrt{24}+x^{2}+y^{2}}=9.880
\]

下面计算积分的精确值：

\[
\begin{aligned} & \iint_{x^{2}+y^{2}: 225} \frac{d x d y}{\sqrt{24+x^{2}+y^{2}}} \\ = & \left.4 \int_{0}^{5} \ln \left(y+\sqrt{24+x^{2}+y^{2}}\right)\right|_{2} ^{\sqrt{25-x^{2}}} d x \\ = & 4 \int_{0}^{5} \ln \left(\sqrt{25}-x^{2}+7\right) d x-2 \int_{0}^{5} \ln \left(24+x^{2}\right) d x .
\end{aligned}
\]

由于

\[
\int \ln \left(24+x^{2}\right) d x=x \ln \left(24+x^{2}\right)-\int \frac{2 x^{2}}{24+x^{2}} d x
\]

\[
=x \ln \left(24+x^{2}\right)-2 x+\frac{24}{\sqrt{6}} \operatorname{arctg} \frac{x}{\sqrt{24}}+C
\]

从而

\[
\begin{aligned}
& 2 \int_{0}^{5} \ln \left(24+x^{2}\right) d x \\
& =\left.\left(2 x \ln \left(24+x^{2}\right)-4 x+\frac{48}{\sqrt{6}} \operatorname{arctg} \frac{x}{\sqrt{24}}\right)\right|_{0} ^{5}
\end{aligned}
\]

\[
=20 \ln 7-20+8 \sqrt{6} \operatorname{arctg} \frac{5}{\sqrt{24}}
\]

又

\[
\begin{aligned}
& 4 \int_{0}^{15} \ln \left(\sqrt{25-x^{2}}+7\right) d x \\
& =\left.4\left[x \ln \left(\sqrt{25-x^{2}}+7\right)\right)\right|_{0} ^{5} \\
& +4 \int_{0}^{5} \frac{x^{2} d x}{\left(\sqrt{25-x^{2}}+7\right) \sqrt{25-x^{2}}} \\
& \left.=20 \ln 7+4 \int_{0}^{5} \frac{x^{2} d x}{\left(\sqrt{25}-x^{2}\right.}+7\right) \sqrt{25-x^{2}},
\end{aligned}
\]

再令\( x=5 \sin t \), 有

\[
\begin{aligned}
& \int_{0}^{5} \frac{x^{2} d x}{\left(\sqrt{25-x^{2}}+7\right) \sqrt{25-x^{2}}}=\int_{0}^{\frac{\pi}{2}} \frac{-25 \cos ^{2} t+25}{5 \cos t+7} d t \\
& =-\int_{0}^{\frac{\pi}{2}}(5 \cos t-7) d t-\int_{0}^{\frac{\pi}{2}} \frac{24}{5 \cos t+7} d t \\
& =\left.(7 t-5 \sin t)\right|_{0} ^{\frac{\pi}{2}}-\left.24\left[\frac{1}{\sqrt{6}} \operatorname{arctg}\left(\frac{1}{\sqrt{6}} \operatorname{tg} \frac{t}{2}\right)\right]\right|_{0} ^{\frac{\pi}{2}} \\
& =\frac{7 \pi}{2}-5-4 \sqrt{6} \operatorname{arctg} \frac{2}{\sqrt{24}}, \\
& \text { 内而 } \\
& 4 \int_{0}^{5} \ln \left(\sqrt{25-x^{2}}+7\right) d x \\
& =20 \ln 7+14 \pi-20-16 \sqrt{6} \operatorname{arctg} \frac{2}{\sqrt{24}} .
\end{aligned}
\]

注意到

\[
2 \operatorname{arctg} \frac{2}{\sqrt{24}}-\operatorname{arctg} \frac{5}{\sqrt{24}}=\frac{\pi}{2},
\]

最后使得到

\[
\begin{aligned}
& \iint_{x^{2}} \int_{y^{2} .25} \frac{d x d y}{\sqrt{2} 4+x^{2}-y^{2}} \\
& =14 \pi-4 \sqrt{24}\left(2 \operatorname{arctg}-\frac{2}{\sqrt{24}}+\operatorname{arctg}-\frac{5}{\sqrt{24}}\right)
\end{aligned}
\]

\[
\ddot{-} 2 \pi(7-\sqrt{24}) \doteq 13.19
\]

精确值与近似值作比较，显见误差较大，其原因在于有不少不是正方形的域都被忽略，因而产生较大的绝对误差\( 4.31 \)及较大的相对误差\( \frac{4.31}{13.19}-32.7 \% \).
注意，求\( \iint_{x^{2} y_{25}}-\frac{d x d y}{\sqrt{24+x^{2}}+y^{2}} \)的精确值若采用极坐标则较为简单：

\[
\begin{aligned}
\int_{,^{2}+y^{2}<25} \cdots \frac{d x d y}{\sqrt{24+x^{2}+}-\overline{y^{2}}} & =\int_{, 1}^{3 \pi} d \theta \int_{0}^{3} \cdot \frac{r d r}{\sqrt{2} \cdot \overline{+} r^{3}} \\
& =2 \pi(7 \cdots \sqrt{24}) .
\end{aligned}
\]

但按原习题集灼安排，似产堵3937题以庑才开始使用极坐标。故本题仍用直角坐标进行计笙.

3904. 用直线\( x- \)常数\( y= \)常数，\( x+y= \)常数把域分为烟个相管的二角形，
并取被积函数在牳个二角形的中线交点乙值近似地讣算积分

\[
\iint_{1} \sqrt{x+y} d S,
\]

其中，\( S \)衣昌直线\( x=0, y=0 \)及\( x+y=1 \)所围成的三角形

解：我们分须以\( x=\frac{1}{2}, y=\frac{1}{2} \)及\( x+y=\frac{1}{2} \)分戓\( S \)
即得四个相等的三角形，它们的面积均为\( \frac18 \)，重心为

\[
\left(-\frac{1}{6}, \frac{1}{6} \mid \cdot\left(\frac{1}{3}, \frac{1}{3}\right),\left(\frac{2}{3}, \frac{1}{6}\right) \text { 及 }\left(\frac{1}{6}, \frac{2}{3}\right)\right. 
\]

于是, 得此积分的迉似佶为

\[
\iint_{i} \sqrt{x+y} d S
\doteq \frac{1}{8}\left(\sqrt{\frac{1}{6}+\frac{1}{6}}+\sqrt{\frac{1}{3}+\frac{1}{3}}+2 \sqrt{\frac{2}{3}+\frac{1}{6}}\right)
\]

\( \therefore \frac{1}{8}(0.577-0.816+2.0913) \doteq 0.402 \),

共精确值为

\[
\begin{aligned}
\iint_{\pi} \sqrt{x+y} d S & =\int_{0}^{1} d x \int_{0}^{1-x} \sqrt{x-y} d y \\
& =\frac{2}{3} \int_{0}^{1}\left(1-x^{\frac{3}{2}}\right) d x=\frac{2}{5}=0.4 .
\end{aligned}
\]

3905. 把域\( S\left\{x^{2}+y^{2} \leqslant 1\right\} \)
分为有限个直径小于\( \delta \)的讨求积的
子域\( \Delta S i(i=1.2, \cdots, n) \)
对\( \mp \)什么样的值\( \delta \)能保证不等式

\[
\left|\iint \sin (x+y) d S-\sum_{i=1}^{n} \sin \left(x_{1}+y_{2}\right) \Delta S_{2}\right|<0.001
\]

成立？其中，\( \left(x,, y_{1}\right) \in \Delta S_{i} \).

解：记函数\( \sin (x+y) \)在\( \Delta S_{2} \)中的振幅
为\( \omega_{i} \)，则

\[
\begin{aligned}
~& \left|\iint \sin (x+y) d S-\sum_{i=1}^{n} \sin \left(x_{i}+y_{i}\right) \Delta S_{i}\right| \\
=& \left|\sum_{i=1}^{n} \iint_{\sum_{1}}\left[\sin (x+y)-\sin \left(x_{0}+y_{1}\right)\right] d S\right| \\
\leqslant & \sum_{i=1}^{n} \iint_{i \leqslant_{i}}\left|\sin (x+y)-\sin \left(x_{t}+y_{i}\right)\right| d S \\
\leqslant & \sum_{i=1}^{n} \iint_{\Delta S_{i}} \omega_{i} d S \\
=& \sum_{i=1}^{n} \omega_{r} \Delta S_{i}
\end{aligned}
\]


由于域\( S\left\{x^{2}+y^{2} \leqslant 1\right\} \)
的自积等于\( \pi \), 故只要\( \omega_{i}<\frac{0.001}{\pi} \),
使能满足原圧等式的要求。倡柶兰

\[
\begin{aligned}
w_{z} =& \sup _{\left(x_{r}, y_{2}\right) \gamma_{\Delta s_{t}}}\left|\sin \left(x_{r}^{\prime}+y_{r}^{\prime}\right)-\sin \left(x_{1}+y_{r}\right)\right| \\
& \left(x_{1}, y, 3 \in \Delta s_{1}\right. \\
\leqslant & \sup _{\substack{x_{1}, y_{i}, \sum_{1}}}\left|\left(x_{i}^{\prime}+y\right)-\left(x_{i}+y_{i}\right)\right| \\
& \left(x_{1}, x_{1}\right) \in \Delta r_{1} \\
\leqslant & \sup _{\left(x_{1}, y_{0}\right) \in \Delta_{s},}\left[\left|x_{r}^{\prime}-x_{1}\right|+\left|y_{2}^{\prime}-y_{r}\right|\right] \\
& \left(x_{1} \cdot y_{1}\right) \in \Delta s \text {, } \\
\leqslant & \sup _{\substack{\left.x_{r}, y_{j}\right) \in \Sigma_{+} \\\left(a, y_{t}\right) \in \Delta s_{i}}} \sqrt{2\left[\left(x_{i}^{\prime}-x_{i}\right)^{2}+\left(y_{i}^{\prime}-y_{t}\right)^{2}\right]} \\
=& \sqrt{2} \delta \text {, }
\end{aligned}
\]

故只要取

\[
\delta<\frac{1}{\sqrt{2} \pi} \times 0.001 \doteq 0.00022,
\]

则有

\[
\left|\iint_{1} \sin (x+y) d S-\sum_{i=1}^{n} \sin \left(x_{i}+y_{i}\right) \Delta S_{1}\right|<0.001 .
\]

*) 对平任意非负实数\( a, b \)有

\[
2 a b \leqslant a^{2}+b^{2} \text { 或 }(a+b)^{2} \leqslant 2\left(a^{2}+b^{2}\right) \text {, }
\]

从而

\[
a+b \leqslant \sqrt{2\left(a^{2}+b^{2}\right)} .
\]
