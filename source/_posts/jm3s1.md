---
title: jm3s1
date: 2008-12-30 11:03:48
tags: jm
---

# 第三章 不定积分  §1. 最筒单的不定积分

\( 1^\circ \) 不定积分的概念
若\( f(x) \)为连续抣数及
\( F^{\prime}(x)=f(x) \)，则

\[
\int f(x) d x=F(x)+C
\]

式中\(C\)为任意常数.

\( 2^\circ \)不定积分的荃本性质：

(a) \( d\left[\int f(x) d x\right]=f(x) d x ;(\sigma) \int d \Phi(x)=\Phi(x)+C \);

(b) \( \int A f(x) d x=A \int f(x) d x \quad(A= \) 常数);

(c) \(\int[f(x)+g(x)] d x=\int f(x) d x+\int g(x) d x\).

\( 3^\circ \) 最箔积分表：

\(\int x^{*} d x=\frac{x^{n+1}}{n+1}+C \quad(n \neq-1)\);

I. \(\int \frac{d x}{x}=\ln |x|+C(x \neq 0)\);

I. \(\int \frac{d x}{1+x^{2}}=\left\{\begin{array}{l}\operatorname{arctg} x+C, \\ -\operatorname{arcctg} x+C ;\end{array}\right.\)

N. \(\int \frac{d x}{1-x^{2}}=\frac{1}{2} \ln \left|\frac{1+x}{1-x}\right|+C *\)

v. \(\int \frac{d x}{\sqrt{1-x^{2}}}=\left\{\begin{array}{l}\arcsin x+C \text {; } \\ -\arccos x+C \text {; }\end{array}\right.\)

ท. \(\int \frac{d x}{\sqrt{x^{2} \pm 1}}=\ln \left|x+\sqrt{x^{2} \pm 1}\right|+C\); n. \(\int a^{x} d x=\frac{a^{\prime}}{\ln a}+\left((a>0, a \neq 1) ; \int e^{x} d x=e^{x}+C\right.\);

v. \(\int \sin x d x=-\cos x+C_{7}\)

x. \(\int \cos x d x=\sin x+C\)

\(x, \int \frac{d x}{\sin ^{2} x}=-\operatorname{ctg} x+C\)

\(\mathrm{x}\). \(\int \frac{d x}{\cos ^{2} x}=\mathrm{tg} x+C\);

XI \(. \int \operatorname{sh} x d x=\operatorname{ch} x+C ;\)

XI . \(\int \operatorname{ch} x d x=\operatorname{sh} x+C\);

XV. \(\int \frac{d x}{\operatorname{sh}^{2} x}=-\operatorname{cth} x+C_{7}\)

XV. \(\int \frac{d x}{\operatorname{ch}^{2} x}=\operatorname{th} x+C\).

\( 4^\circ \) 积分的基本击法

(a) 引入新变数法 若

\[
\int f(x) d x=F(x)+C,
\]

则 \(\int f(u) d u=F(u)+C\), 式中 \(u=\varphi(x)\).

(6) 分项积分法 若

\[
f(x)=f_{1}(x)+f_{2}(x) .
\]

则

\[
\int f(x) d x=\int f_{1}(x) d x+\int f_{2}(x) d x .
\]

(B) 代入法 假设

\(x=\varphi(t)\),式中 \(\varphi(t)\) 及其导函数 \(\varphi^{\prime}(t)\) 为连续的,

则俉

\[
\int f(x) d x=\int f(\varphi(t)] \varphi^{\prime}(t) d t .
\]

（「）分部积分法 若 \(u\) 和 \(v\) 为 \(x\) 的可僮分函数,

则

\[
\int u d v=u v-\int v d u .
\]

利用最简积分表, 求出下列积分:

1627. \(\displaystyle \int\left(3-x^{2}\right)^{3} d x\).

\[
\begin{aligned}
 & \int\left(3-x^{2}\right)^{3} d x \\
=& \int\left(27-27 x^{2}+9 x^{4}-x^{6}\right) d x \\
=& 27 x-9 x^{3}+\frac{9}{5} x^{5}-\frac{1}{7} x^{7}+C
\end{aligned}
\]

1628. \(\displaystyle \int x^{2}(5-x)^{4} d x\).

\[
\begin{aligned}
~& \int x^{2}(5-x)^{4} d x \\
=& \int\left(625 x^{2}-500 x^{3}+150 x^{4}-20 x^{5}+x^{6}\right) d x \\
=& \frac{625}{3} x^{3}-125 x^{4}+30 x^{5}-\frac{10}{3} x^{6}+\frac{1}{7} x^{7}+C \text {. }
\end{aligned}
\]

1629. \(\displaystyle \int(1-x)(1-2 x)(1-3 x) d x\).

\[
\begin{aligned}
~& \int(1-x)(1-2 x)(1-3 x) d x \\
=& \int\left(1-6 x+11 x^{2}-6 x^{3}\right) d x \\
=& x-3 x^{3}+\frac{11}{3} x^{3}-\frac{3}{2} x^{4}+C \text {. }
\end{aligned}
\]

1630. \(\displaystyle \int\left(\frac{1-x}{x}\right)^{2} d x\).

\[
\begin{aligned}
~& \int\left(\frac{1-x}{x}\right)^{2} d x \\
=& \int\left(\frac{1}{x^{2}}-\frac{2}{x}+1\right) d x \\
=& -\frac{1}{x}-2 \ln |x|+x+C .
\end{aligned}
\]

本章在炇述习旦及其解答过侱中, 
凡出現的函数,
无论是被积函数还是原函数, 
均㖵认是在有意义的定义域上进行的. 
洌如最简积分表中 I 里
当\(n \leqslant-2\) 时, 
要求\(x \neq 0\); \(N\)中
要求\(|x| \neq 1 ; N\)中
要求\(|x|<1 ;\) 
以及\(n\)中, 当敢负号时要求
\( |x|>1 \)等等，就未加声明。
在解题中也有相当多的类似情况。
因此，如无特别声明，在一般情形下，
这些定义域是很容易被读者确定的，
此处就不再予以一一指明

1631. \(\displaystyle \int\left(\frac{a}{x}+\frac{a^{2}}{x^{2}}+\frac{a^{3}}{x^{3}}\right) d x\)

\[
\begin{aligned}
~& \int\left(\frac{a}{x}+\frac{a^{2}}{x^{2}}+\frac{a^{3}}{x^{3}}\right) d x \\
=& a \ln |x|-\frac{a^{2}}{x}-\frac{a^{3}}{2 x^{2}}+C 
\end{aligned}
\]

1632. \(\displaystyle \int \frac{x+1}{\sqrt{x}} d x\)

\[
\begin{aligned}
~& \int \frac{x+1}{\sqrt{x}} d x=\int\left(x^{\frac{1}{2}}+x^{-\frac{1}{2}}\right) d x \\
=& \frac{2}{3} x \sqrt{x}+2 \sqrt{x}+C
\end{aligned}
\]

1633. \(\displaystyle \int \frac{\sqrt{x}-2 \sqrt[3]{x^{2}}+1}{\sqrt[4]{x}} d x\)

\[
\begin{aligned}
~& \int \frac{\sqrt{x}-2 \sqrt[3]{x^{2}}+1}{\sqrt[4]{x}} d x \\
=& \int\left(x^{\frac{1}{4}}-2 x^{\frac{5}{12}}+x^{-\frac{1}{4}}\right) d x \\
=& \frac{4}{5} x \sqrt[4]{x}-\frac{24}{17} x \sqrt[12]{x^{5}}+\frac{4}{3} \sqrt[4]{x^{3}}+C .
\end{aligned}
\]

1634. \(\displaystyle \int \frac{(1-x)^{3}}{x \sqrt[3]{x}} d x\)

\[
\begin{aligned}
~& \int \frac{(1-x)^{3}}{x \sqrt[3]{x}} d x \\
=& \int\left(x^{-\frac{4}{3}}-3 x^{-\frac{1}{3}}+3 x^{\frac{2}{3}}-x^{\frac{5}{3}}\right) d x \\
=& -\frac{3}{\sqrt[3]{x}}\left(1+\frac{3}{2} x-\frac{3}{5} x^{2}+\frac{1}{8} x^{3}\right)+C .
\end{aligned}
\]

1635. \(\displaystyle \int\left(1-\frac{1}{x^{2}}\right) \sqrt{x \sqrt{x}} d x\)

\[
\begin{aligned}
~& \int\left(1-\frac{1}{x^{2}}\right) \sqrt{x \sqrt{x}} d x \\
=& \int\left(x^{\frac{3}{4}}-x \frac{5}{4}\right) d x \\
=& \frac{4}{7} x^{\frac{7}{4}}+4 x^{-\frac{1}{4}}+C \\
=& \frac{4\left(x^{z}+7\right)}{7 \sqrt[4]{x}}+C .
\end{aligned}
\]

1636. \(\displaystyle \int \frac{\sqrt{2 x}-\sqrt[3]{3 x})^{2}}{x} d x\)

\[
\begin{aligned}
~& \int \frac{\sqrt{2 x}-\sqrt[3]{3 x})^{2}}{x} d x \\
=& \int\left(2-2 \sqrt[6]{72} x^{-\frac{1}{6}}+\sqrt[3]{9} x^{-\frac{1}{3}}\right) d x \\
=& 2 x-\frac{12}{5} \sqrt[6]{72 x^{5}}+\frac{3}{2} \sqrt[3]{9 x^{2}}+C
\end{aligned}
\]

1637. \(\displaystyle \int \frac{\sqrt{x^{-1}+x^{-4}+2}}{x^{3}} d x\)

\[
\begin{aligned}
~& \int \frac{\sqrt{x^{4}+x^{-4}+2}}{x^{3}} d x \\
=& \int \frac{x^{2}+\frac{1}{x^{2}}}{x^{3}} d x \\
=& \int\left(\frac{1}{x}+\frac{1}{x^{5}}\right) d x \\
=&\ln |x|-\frac{1}{4 x^{4}}+C
\end{aligned}
\]

1638. \(\displaystyle \int \frac{x^{2}}{1+x^{2}} d x\)

\[
\begin{aligned}
~& \int \frac{x^{2}}{1+x^{2}} d x \\
=&\int\left(1-\frac{1}{x^{2}+1}\right) d x \\
=& x-\operatorname{arctg} x+C
\end{aligned}
\]

1639. \(\displaystyle \int \frac{x^{2}}{1-x^{2}} d x\)

\[
\begin{aligned}
~& \int \frac{x^{2}}{1-x^{2}} d x \\
=& \int\left(-1+\frac{1}{1-x^{2}}\right) d x \\
=& -x+\frac{1}{2} \ln \left|\frac{1+x}{1-x}\right|+C
\end{aligned}
\]

1640. \(\displaystyle \int \frac{x^{2}+3}{x^{2}-1} d x\)

\[
\begin{aligned}
~& \int \frac{x^{2}+3}{x^{2}-1} d x \\
=& \int\left(1+\frac{4}{x^{2}-1}\right) d x \\
=& x+2 \ln \left|\frac{x-1}{x+1}\right|+C .
\end{aligned}
\]

1641. \(\displaystyle \int \frac{\sqrt{1+x^{2}}+\sqrt{1-x^{2}}}{\sqrt{1-x^{4}}} d x\)

\[
\begin{aligned}
~& \int \frac{\sqrt{1+x^{2}}+\sqrt{1-x^{2}}}{\sqrt{1-\overline{x^{4}}}} d x \\
=& \int\left(\frac{1}{\sqrt{1-x^{2}}}+\frac{1}{\sqrt{1+x^{2}}}\right) d x \\
=& \arcsin x+\ln \left(x+\sqrt{1+x^{2}}\right)+C
\end{aligned}
\]

1642. \(\displaystyle \int \frac{\sqrt{x^{2}+1}-\sqrt{x^{2}-1}}{\sqrt{x^{4}-1}} d x\)

\[
\begin{aligned}
~& \int \frac{\sqrt{x^{2}+1}-\sqrt{x^{2}-1}}{\sqrt{x^{4}-1}} d x \\
=& \int\left(\frac{1}{\sqrt{x^{2}-1}}-\frac{1}{\sqrt{x^{2}+1}}\right) d x \\
=& \ln \left|\frac{x+\sqrt{x^{2}}-1}{x+\sqrt{x^{2}+1}}\right|+C
\end{aligned}
\]

1643. \(\displaystyle \int\left(2^{x}+3^{x}\right)^{2} d x\)

\[
\begin{aligned}
~& \int\left(2^{x}+3^{x}\right)^{2} d x \\
=& \int\left(4^{x}+2 \cdot 6^{x}+9^{x}\right) d x \\
=& \frac{4^{x}}{\ln 4}+2 \cdot \frac{6^{x}}{\ln 6}+\frac{9^{x}}{\ln 9}+C
\end{aligned}
\]

1644. \(\displaystyle \int \frac{2^{x+1}-5^{x-1}}{10^{x}} d x\)

\[
\begin{aligned}
~& \int \frac{2^{x+1}-5^{x-1}}{10^{x}} d x \\
=& \int\left[2\left(\frac{1}{5}\right)^{x}-\frac{1}{5}\left(\frac{1}{2}\right)^{x}\right] d x \\
=& -\frac{2}{\ln 5}\left(\frac{1}{5}\right)^{x}+\frac{1}{5 \ln 2}\left(\frac{1}{2}\right)^{x}+C
\end{aligned}
\]

1645. \(\displaystyle \int \frac{e^{3 x}+1}{e^{x}+1} d x\)

\[
\begin{aligned}
~& \int \frac{e^{3 x}+1}{e^{x}+1} d x \\
=& \int\left(e^{2 x}-e^{x}+1\right) d x \\
=& \frac{1}{2} e^{2 x}-e^{x}+x+C
\end{aligned}
\]

1646. \(\displaystyle \int(1+\sin x+\cos x) d x\)

\[
\int(1+\sin x+\cos x) d x=x-\cos x+\sin x+C
\]

1647. \(\displaystyle \int \sqrt{1-\sin 2 x} d x\)

\[
\begin{aligned}
~& \int \sqrt{1-\sin 2 x} d x \\
=& \int \sqrt{(\cos x-\sin x)^{2}} d x \\
=& \int \left[\operatorname{sgn}(\cos x-\sin x)\right](\cos x-\sin x) d x \\
=& (\sin x+\cos x) \cdot \operatorname{sgn}(\cos x-\sin x)+C
\end{aligned}
\]

1648. \(\displaystyle \int \operatorname{ctg}^{2} x d x\)

\[
\int \operatorname{ctg}^{2} x d x=\int\left(\csc ^{2} x-1\right) d x=-\operatorname{ctg} x-x+C
\]

1649. \(\displaystyle \int \operatorname{tg}^{2} x d x\)

\[
\int \operatorname{tg}^{2} x d x=\int\left(\sec ^{2} x-1\right) d x=\operatorname{tg} x-x+C
\]

1650. \(\displaystyle \int(a \operatorname{sh} x+b \operatorname{ch} x) d x\)

\[
\int(a \operatorname{sh} x+b \operatorname{ch} x) d x=a \operatorname{ch} x+b \operatorname{sh} x+C
\]

1651. \(\displaystyle \int \operatorname{th}^{2} x d x\)

\[
\int \operatorname{th}^{2} x d x=\int\left(1-\frac{1}{\operatorname{ch}^{2} x}\right) d x=x-\operatorname{th} x+C
\]

1652. \(\displaystyle \int \operatorname{cth}^{2} x d x\)

\[\int \operatorname{cth}^{2} x d x=\int\left(1+\frac{1}{\operatorname{sh}^{2} x}\right) d x=x-\operatorname{cth} x+C
\]

1653. 证明：若

\[
\int f(x) d x=F(x)+C
\]

则

\[
\int f(a x+b) d x=\frac{1}{a} F(a x+b)+C \quad(a \neq 0)
\]

证：由\( \int f(x) d x=F(x)+C \)得知\( F^{\prime}(x)=f(x) \). 
因而有\( F^{\prime}(a x+b)=f(a x+b) \),
且\( \frac{d}{d x}\left[\frac{1}{a} F(a x+b)\right] \),
于是

\[
\begin{aligned}
~& F^{\prime}(a x+b) \\
=& \frac{d}{d x}\left[\frac{1}{a} F(a x+b)\right] \\
=& f(ax+b)
\end{aligned}
\]

所以

\[
\int f(a x+b) d x=\frac{1}{a} F(a x+b)+c
\]

1654. \(\displaystyle \int \frac{d x}{x+a}\)

\[
\begin{aligned}
~& \int \frac{\sqrt[5]{1-2 x+x^{2}}}{1-x} d x \\
=& \int(1-x)^{-\frac{3}{5}} d x \\
=& -\frac{5}{2} \sqrt[5]{(1-x)^{2}}+C
\end{aligned}
\]

1661. \(\displaystyle \int \frac{d x}{2+3 x^{2}}\)

\[
\begin{aligned}
~& \int \frac{d x}{2+3 x^{2}} \\
=& \int \frac{d x}{(\sqrt{2})^{2}+(\sqrt{3} x)^{2}} \\
=& \frac{1}{\sqrt{6}} \operatorname{arctg}\left(x \sqrt{\frac{3}{2}}\right)+C
\end{aligned}
\]

1661. \(\displaystyle \int \frac{d x}{2-3 x^{2}}\)

\[
\begin{aligned}
~& \int \frac{d x}{2-3 x^{2}}=\frac{1}{2} \int \frac{d x}{1-\left(\sqrt{\frac{3}{2}} x\right)^{2}} \\
=& \frac{1}{2} \cdot \sqrt{\frac{2}{3}} \cdot \frac{1}{2} \ln \left|\frac{1+\sqrt{\frac{3}{2}} x}{1-\sqrt{\frac{3}{2}} x}\right|+C \\
=& \frac{1}{2 \sqrt{6}} \ln \left|\frac{\sqrt{2}+x \sqrt{3}}{\sqrt{2}-x \sqrt{3}}\right|+C
\end{aligned}
\]

1662. \(\displaystyle \int \frac{d x}{\sqrt{2-3 x^{2}}}\)

\[
\frac{d x}{\sqrt{2-3 x^{2}}}=\frac{1}{\sqrt{3}} \arcsin \left(x \sqrt{\frac{3}{2}}\right)+C
\]

1663. \(\displaystyle \int \frac{d x}{\sqrt{3 x^{2}-2}}\)

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{3 x^{2}-2}} \\
=& \frac{1}{\sqrt{2}} \int \frac{d x}{\sqrt{\left(\sqrt{\frac{3}{2}} x\right)^{2}}-1} \\
=& \frac{1}{\sqrt{2}} \cdot \sqrt{\frac{2}{3}}\left|x \sqrt{\frac{3}{2}}+\sqrt{\frac{3}{2} x^{2}-1}\right|+C_{1} \\
=& \frac{1}{\sqrt{3}} \ln \left|x \sqrt{3}+\sqrt{3 x^{2}-2}\right|+C
\end{aligned}
\]

1664. \(\displaystyle \int\left(e^{-x}+e^{-2 x}\right) d x\)

\[
\int\left(e^{-r}+e^{-2 x}\right) d x=-\left(e^{-x}+\frac{1}{2} e^{-2 \pi}\right)+C
\]

1665. \(\displaystyle \int(\sin 5 x-\sin 5 \alpha) d x\)

\[
\int(\sin 5 x-\sin 5 \alpha) d x=-\frac{1}{5} \cos 5 x-x \sin 5 \alpha+C
\]

1666. \(\displaystyle \int \frac{d x}{\sin ^{2}\left(2 x+\frac{\pi}{4}\right)}\)

\[
\int \frac{d x}{\sin ^{2}\left(2 x+\frac{\pi}{4}\right)}=-\frac{1}{2} \operatorname{ctg}\left(2 x+\frac{\pi}{4}\right)+C
\]

1667. \(\displaystyle \int \frac{d x}{1+\cos x}\)

\[
\int \frac{d x}{1+\cos x}=\frac{1}{2} \int \frac{d x}{\cos ^{2} \frac{x}{2}}=\operatorname{tg} \frac{x}{2}+C
\]

1668. \(\displaystyle \int \frac{d x}{1-\cos x}\)

\[
\int \frac{d x}{1-\cos x}=\frac{1}{2} \int \frac{d x}{\sin ^{2} \frac{x}{2}}=-\operatorname{ctg} \frac{x}{2}+C
\]

1669. \(\displaystyle \int \frac{d x}{1+\sin x}\)

\[
\begin{aligned}
~& \int \frac{d x}{1+\sin x} \\
=& \int \frac{d x}{1+\cos \left(\frac{\pi}{2}-x\right)} \\
=& -\operatorname{tg}\left(\frac{\pi}{4}-\frac{x}{2}\right)+C
\end{aligned}
\]

1670. \(\displaystyle \int[\operatorname{sh}(2 x+1)+\operatorname{ch}(2 x-1)] d x\)

\[
\begin{aligned}
~& \int[\operatorname{sh}(2 x+1)+\operatorname{ch}(2 x-1)] d x \\
=& \frac{1}{2}[\operatorname{ch}(2 x+1)+\operatorname{sh}(2 x-1)]+C
\end{aligned}
\]

1672. \(\displaystyle \int \frac{d x}{\operatorname{ch}^{2} \frac{x}{2}}\)

\[
\int \frac{d x}{\operatorname{ch}^{2} \frac{x}{2}}=2 \operatorname{th} \frac{x}{2}+C
\]

1673. \(\displaystyle \int \frac{d x}{\operatorname{sh}^{2} \frac{x}{2}}\)

\[
\int \frac{d x}{\operatorname{sh}^{2} \frac{x}{2}}=-2 \operatorname{cth} \frac{x}{2}+C
\]


1674. \(\displaystyle \int \frac{x d x}{\sqrt{1-x^{2}}}\)

\[
\int \frac{x d x}{\sqrt{1-x^{2}}}=-\int \frac{d\left(1-x^{2}\right)}{2 \sqrt{1-x^{2}}}=-\sqrt{1-x^{2}}+C
\]

1675. \(\displaystyle \int x^{2} \sqrt[3]{1+x^{3}} d x\)

\[
\begin{aligned}
~& \int x^{2} \sqrt[3]{1+x^{3}} d x \\
=& \frac{1}{3} \int\left(1+x^{3}\right)^{\frac{1}{3}} d\left(1+x^{3}\right) \\
=& \frac{1}{4}\left(1+x^{3}\right)^{\frac{4}{3}}+C
\end{aligned}
\]

1676. \(\displaystyle \int \frac{x d x}{3-2 x^{2}}\)

\[
\begin{aligned}
~& \int \frac{x d x}{3-2 x^{2}} \\
=& -\frac{1}{4} \int \frac{d\left(3-2 x^{2}\right)}{3-2 x^{2}} \\
=& -\frac{1}{4} \ln \left|3-2 x^{2}\right|+C
\end{aligned}
\]

1677. \(\displaystyle \int \frac{x d x}{\left(1+x^{2}\right)^{2}}\)

\[
\begin{aligned}
~& \int \frac{x d x}{\left(1+x^{2}\right)^{2}} \\
=& \frac{1}{2} \int \frac{d\left(1+x^{2}\right)}{\left(1+x^{2}\right)^{2}} \\
=& -\frac{1}{2\left(1+x^{2}\right)}+C
\end{aligned}
\]

1678. \(\displaystyle \int \frac{x d x}{4+x^{4}}\)

\[
\begin{aligned}
~& \int \frac{x d x}{4+x^{4}} \\
=& \frac{1}{2} \int \frac{d\left(x^{2}\right)}{2^{2}+\left(x^{2}\right)^{2}} \\
=& \frac{1}{4} \operatorname{arctg} \frac{x^{2}}{2}+C
\end{aligned}
\]

1679. \(\displaystyle \int \frac{x^{3} d x}{x^{8}-2}\)

\[
\begin{aligned}
~& \int \frac{x^{3} d x}{x^{8}-2} \\
=& \frac{1}{4} \int \frac{d\left(x^{4}\right)}{\left(x^{4}\right)^{2}-(\sqrt{2})^{2}} \\
=& \frac{1}{8 \sqrt{2}} \ln \left|\frac{x^{4}-\sqrt{2}}{x^{4}+\sqrt{2}}\right|+C
\end{aligned}
\]

1680. \(\displaystyle \int \frac{d x}{\sqrt{x}(1+x)}\)

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{x}(1+x)} \\
=& 2 \int \frac{d(\sqrt{x})}{1+(\sqrt{x})^{2}} \\
=& 2 \operatorname{arctg} \sqrt{x}+C
\end{aligned}
\]

1681. \(\displaystyle \int \sin \frac{1}{x} \cdot \frac{d x}{x^{2}}\)

\[
\begin{aligned}
~& \int \sin \frac{1}{x} \cdot \frac{d x}{x^{2}} \\
=& -\int \sin \frac{1}{x} d\left(\frac{1}{x}\right) \\
=& \cos \frac{1}{x}+C
\end{aligned}
\]

1682. \(\displaystyle \int \frac{d x}{x \sqrt{x^{2}+1}}\)

\[
\begin{aligned}
~& \int \frac{d x}{x \sqrt{x^{2}+1}}=\int \frac{d x}{x|x| \sqrt{1+\frac{1}{x^{2}}}} \\
=& -\int \frac{d\left(\frac{1}{|x|}\right)}{\sqrt{1+\left(\frac{1}{|x|}\right)^{2}}} \\
=& -\ln -\left(\frac{1}{|x|}+\sqrt{1+\frac{1}{x^{2}}}\right)+C \\
=& -\ln \left|\frac{1+\sqrt{x^{2}+1}}{x}\right|+C
\end{aligned}
\]

1683. \(\displaystyle \int \frac{d x}{x \sqrt{x^{2}-1}}\)

\[
\begin{aligned}
~& \int \frac{d x}{x \sqrt{x^{2}-1}} \\
=& \int \frac{d x}{x|x| \sqrt{1-\frac{1}{x^{2}}}} \\
=& -\int \frac{d\left(\frac{1}{|x|}\right)}{\sqrt{1-\left(\frac{1}{|x|}\right)^{2}}} \\
=& -\arcsin \frac{1}{|x|}+C
\end{aligned}
\]

1684. \(\displaystyle \int \frac{d x}{\left(x^{2}+1\right)^{\frac{3}{2}}}\)

\[
\begin{aligned}
~& \int \frac{d x}{\left(x^{2}+1\right)^{\frac{3}{2}}} \\
=& \int \frac{\operatorname{sgn} x d x}{x^{3}\left(1+\frac{1}{x^{2}}\right)^{\frac{3}{2}}} \\
=& -\frac{1}{2} \int\left(1+\frac{1}{x^{2}}\right)^{-\frac{3}{2}} \operatorname{sgn} x d\left(1+\frac{1}{x^{2}}\right) \\
=& \left(1+\frac{1}{x^{2}}\right)^{-\frac{1}{2}} \operatorname{sgn} x+C \\
=& \frac{x}{\sqrt{x^{2}+1}}+C
\end{aligned}
\]

1685. \(\displaystyle \int \frac{x d x}{\left(x^{2}-1\right)^{\frac{3}{2}}} \)

\[
\begin{aligned}
~& \int \frac{x d x}{\left(x^{2}-1\right)^{\frac{3}{2}}} \\
=& \frac{1}{2} \int\left(x^{2}-1\right)^{-\frac{3}{2}} d\left(x^{2}-1\right) \\
=& -\frac{1}{\sqrt{x^{2}-1}}+C
\end{aligned}
\]

1686. \(\displaystyle \int \frac{x^{2} d x}{\left(8 x^{3}+27\right)^{\frac{2}{3}}}\)

\[
\begin{aligned}
~& \int \frac{x^{2} d x}{\left(8 x^{3}+27\right)^{\frac{2}{3}}} \\
=& \frac{1}{24} \int\left(8 x^{3}+27\right)^{-\frac{2}{3}} d\left(8 x^{3}+27\right) \\
=& \frac{1}{8} \sqrt[3]{8 x^{3}+27}+C
\end{aligned}
\]

1687. \(\displaystyle \int \frac{d x}{\sqrt{x(1+x)}}\)

由\( x(1+x)>0 \)知\( x>0 \)或\( x<-1 \)，当\( x>0 \)时

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{x(1+x)}} \\
=& 2 \int \frac{d(\sqrt{x})}{\sqrt{1+(\sqrt{x})^{2}}} \\
=& 2 \ln (\sqrt{x}+\sqrt{1+x})+C
\end{aligned}
\]

当\( x<-1 \)时，

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{x(1+x)}} \\
=& -\int \frac{d[-(1+x)]}{\sqrt{(-x)[-(1+x)]}} \\
=& -2 \int \frac{d(\sqrt{-(1+x)}}{\sqrt{1+(\sqrt{-(1+x)})^{2}}} \\
=& -2 \ln (\sqrt{-x}+\sqrt{-(1+x)})+C
\end{aligned}
\]

总之，得

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{x(1+\pi)}} \\
=& 2 \operatorname{sgn} \cdot \ln (\sqrt{|x|}+\sqrt{|1+x|}+C
\end{aligned}
\]

1688. \(\displaystyle \int \frac{d x}{\sqrt{x(1-x)}}\)

由\( x(1-x)>0 \)知，\( 0<x<1 \)，于是

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{x(1-x)}} \\
=& 2 \int \frac{d(\sqrt{x})}{\sqrt{1-(\sqrt{x})^{2}}} \\
=& 2 a r c \sin \sqrt{x}+C
\end{aligned}
\]

1689. \(\displaystyle \int x e^{-x^{2}} d x\)

\[
\begin{aligned}
~& \int x e^{-x^{2}} d x \\
=& -\frac{1}{2} \int e^{-x^{2}} d\left(-x^{2}\right) \\
=& -\frac{1}{2} e^{-x^{2}}+C
\end{aligned}
\]

1690. \(\displaystyle \int \frac{e^{x} d x}{2+e^{x}}\)

\[
\begin{aligned}
~& \int \frac{e^{x} d x}{2+e^{x}} \\
=& \int \frac{d\left(2+e^{x}\right)}{2+e^{x}} \\
=& \ln \left(2+e^{x}\right)+C
\end{aligned}
\]

1691. \(\displaystyle \int \frac{d x}{e^{x}+e^{-x}}\)

\[
\begin{aligned}
~& \int \frac{d x}{e^{x}+e^{-r}} \\
=& \int \frac{d\left(e^{x}\right)}{1+\left(e^{x}\right)^{2}} \\
=& \operatorname{arctg}\left(e^{x}\right)+C
\end{aligned}
\]

1692. \(\displaystyle \int \frac{d x}{\sqrt{1+\epsilon^{2 x}}}\)

\[
\begin{aligned}
~& \int \frac{d x}{\sqrt{1+e^{2 r}}} \\
=& -\int \frac{d\left(e^{-r}\right)}{\sqrt{1+\left(e^{-r}\right)^{2}}} \\
=& -\ln \left(e^{-x}+\sqrt{1+e^{-2 r}}\right)+C
\end{aligned}
\]

1693. \(\displaystyle \int \frac{\ln ^{2} x}{x} d x\)

\[
\begin{aligned}
~& \int \frac{\ln ^{2} x}{x} d x \\
=& \int \ln ^{2} x d(\ln x) \\
=& \frac{1}{3} \ln ^{3} x+C
\end{aligned}
\]

1694. \(\displaystyle \int \frac{d x}{x \ln x \ln (\ln x)}\)

\[
\begin{aligned}
~& \int \frac{d x}{x \ln x \ln (\ln x)} \\
=& \int \frac{d(\ln x)}{\ln x \ln (\ln x)} \\
=& \int \frac{d(\ln (\ln x))}{\ln (\ln x)} \\
=& \ln |\ln (\ln x)|+C
\end{aligned}
\]

1695. \(\displaystyle \int \sin ^{5} x \cos x d x\)

\[
\begin{aligned}
~& \int \sin ^{5} x \cos x d x \\
=& \int \sin ^{5} x d(\sin x) \\
=& \frac{1}{6} \sin ^{6} x+C
\end{aligned}
\]

1696. \(\displaystyle \int \frac{\sin x}{\sqrt{\cos ^{3} x}} d x\)

\[
\begin{aligned}
~& \int \frac{\sin x}{\sqrt{\cos ^{3} x}} d x \\
=& -\int(\cos x)^{-\frac{3}{2}} d(\cos x) \\
=& \frac{2}{\sqrt{\cos x}}+C
\end{aligned}
\]

1697. \(\displaystyle \int \operatorname{tg} x d x\)

\[
\begin{aligned}
~& \int \operatorname{tg} x d x \\
=& \int \frac{\sin x}{\cos x} d x \\
=& -\int \frac{d(\cos x)}{\cos x} \\
=& -\ln |\cos x|+C
\end{aligned}
\]

1698. \(\displaystyle \int \operatorname{ctg} d x\)

\[
\begin{aligned}
~& \int \operatorname{ctg} x d x \\
=& \int \frac{\cos x}{\sin x} d x \\
=& \int \frac{d(\sin x)}{\sin x} \\
=& \ln |\sin x|+C
\end{aligned}
\]

1699. \(\displaystyle \int \frac{\sin x+\cos x}{\sqrt[3]{\sin x-\cos x}} d x\)

\[
\begin{aligned}
~& \int \frac{\sin x+\cos x}{\sqrt[3]{\sin x-\cos x}} d x \\
=& \int(\sin x-\cos x)^{-\frac{1}{3}} d(\sin x-\cos x) \\
=& \frac{3}{2} \sqrt[3]{(\sin x-\cos x)^{2}}+C \\
=& \frac{3}{2} \sqrt[3]{1-\sin 2 x}+C .
\end{aligned}
\]

1700. \(\displaystyle \int \frac{\sin x \cos x}{\sqrt{a^{2} \sin ^{2} x+b^{2} \cos ^{2} x}} d x\)

当\(|a|=|b| \neq 0\)时

\[
\begin{aligned}
~& \int \frac{\sin x \cos x}{\sqrt{a^{2} \sin ^{2} x+b^{2} \cos ^{2} x}} d x \\
=& \frac{1}{|a|} \int \sin x \cos x d x \\
=& \frac{1}{2|a|} \sin ^{2} x+C
\end{aligned}
\]

当\(|a| \neq|b|\)时

\[
\begin{aligned}
~& \int \frac{\sin x \cos x}{\sqrt{a^{2} \sin ^{2} x+b^{2} \cos ^{2} x}} d x \\
=& \frac{1}{2} \int \frac{d\left(\sin ^{2} x\right)}{\sqrt{\left(a^{2}-b^{2}\right) \sin ^{2} x+b^{2}}} \\
=& \frac{1}{a^{2}-b^{2}} \sqrt{\left(a^{2}-b^{2}\right) \sin ^{2} x+b^{2}}+C \\
=& \frac{\sqrt{a^{2} \sin ^{2} x+b^{2} \cos ^{2} x}}{a^{2}-b^{2}}+C
\end{aligned}
\]

1701. \(\displaystyle \int \frac{d x}{\sin ^{2} x \sqrt[1]{\operatorname{ctg} x}}\)

\[
\begin{aligned}
~& \int \frac{d x}{\operatorname{sh} x} \\
=& \int \frac{\frac{1}{2 \operatorname{ch}^{2} \frac{x}{2}}}{\operatorname{th} \frac{x}{2}} d x \\
=& \int \frac{d\left(\operatorname{th} \frac{x}{2}\right)}{\operatorname{th} \frac{x}{2}} \\
=& \ln \left|\mathbf{t h} \frac{x}{2}\right|+C
\end{aligned}
\]

1706. \(\displaystyle \int \frac{d x}{\operatorname{ch} x}\)

\[
\begin{aligned}
~& \int \frac{d x}{\operatorname{ch} x} \\
=& \int \frac{2 d x}{e^{r}+e^{-r}} \\
=& 2 \int \frac{d\left(e^{r}\right)}{1+\left(e^{r}\right)^{2}} \\
=& 2 \operatorname{arctg}\left(e^{x}\right)+C
\end{aligned}
\]

1707. \(\displaystyle \int \frac{\operatorname{sh} x \operatorname{ch} x}{\sqrt{\operatorname{sh}^{4} x+\operatorname{ch}^{4} x}} d x\)

\[
\begin{aligned}
~& \operatorname{sh}^{4} x+\operatorname{ch}^{4} x \\
=& \left(\operatorname{sh}^{2} x+\operatorname{ch}^{2} x\right)^{2}-2 \operatorname{sh}^{2} x \operatorname{ch}^{2} x \\
=& \operatorname{ch}^{2} 2 x-\frac{1}{2} \operatorname{sh}^{2} 2 x \\
=& \frac{1+\operatorname{ch}^{2} 2 x}{2}
\end{aligned}
\]

所以, 得

\[
\begin{aligned}
~& \int \frac{\operatorname{sh} x \operatorname{ch} x}{\sqrt{\operatorname{sh}^{4} x+\operatorname{ch}^{4} x}} d x \\
=& \int \frac{\frac{1}{4} d(\operatorname{ch} 2 x)}{\frac{1}{\sqrt{2}} \sqrt{1+\operatorname{ch}^{2} 2 x}} \\
=& \frac{1}{2 \sqrt{2}} \ln \left(\operatorname{ch} 2 x+\sqrt{1+\operatorname{ch}^{2} 2 x}-C_{1}\right. \\
=& \frac{1}{2 \sqrt{2}} \ln \left(\frac{\operatorname{ch} 2 x}{\sqrt{2}}+\sqrt{\operatorname{sh}^{4} x+\operatorname{ch}^{4} x}\right)+C
\end{aligned}
\]

1708. \(\displaystyle \int \frac{d x}{\operatorname{ch}^{2} x \cdot \sqrt[3]{\mathrm{th}^{2} x}}\)

\[
\begin{aligned}
~& \int \frac{d x}{\operatorname{ch}^{2} x \cdot \sqrt[3]{\operatorname{th}^{2} x}} \\
=& \int(\operatorname{th} x)^{-\frac{2}{3}} d(\operatorname{th} x) \\
=& 3 \sqrt[3]{\mathrm{th}} x+C
\end{aligned}
\]

1709. \(\displaystyle \int \frac{\operatorname{arctg} x}{1+x^{2}} d x\)

\[
\begin{aligned}
~& \int \frac{\operatorname{arctg} x}{1+x^{2}} d x \\
=& \int \operatorname{arctg} x d(\operatorname{arctg} x) \\
=& \frac{1}{2}(\operatorname{arctg} x)^{2}+C
\end{aligned}
\]

1710. \(\displaystyle \int \frac{d x}{(\arcsin x)^{2} \sqrt{1-x^{2}}}\)

\[
\begin{aligned}
~& \int \frac{d x}{(\arcsin x)^{2} \sqrt{1-x^{2}}} \\
=& \int \frac{d(\arcsin x)}{(\arcsin x)^{2}} \\
=& -\frac{1}{\arcsin x}+C
\end{aligned}
\]

<!--




\begin{enumerate}
  \setcounter{enumi}{1710}
  \item \(\int \sqrt{\frac{\ln \left(x+\sqrt{1+x^{2}}\right)}{1+x^{2}}} d x\).
\end{enumerate}

\[
\text { A } \begin{aligned}
& \int \sqrt{\frac{\ln \left(x+\sqrt{1+x^{2}}\right)}{1+x^{2}}} d x \\
= & \int\left(\ln \left(x+\sqrt{1+x^{2}}\right)\right]^{\frac{1}{2}} d\left[\ln \left(x+\sqrt{1+x^{2}}\right)\right] \\
= & \frac{2}{3} \ln \frac{3}{2}\left(x+\sqrt{1+x^{2}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1711}
  \item \(\int \frac{x^{2}+1}{x^{4}+1} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x^{2}+1}{x^{4}+1} d x=\int \frac{1+\frac{1}{x^{2}}}{x^{2}+\frac{1}{x^{2}}} d x=\int \frac{d\left(x-\frac{1}{x}\right)}{\left(x-\frac{1}{x}\right)^{2}+2} \\
= & \frac{1}{\sqrt{2}} \operatorname{arctg} \frac{x^{2}-1}{x \sqrt{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1712}
  \item \(\int \frac{x^{2}-1}{x^{4}+1} d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int \frac{x^{2}-1}{x^{4}+1} d x=\int \frac{1-\frac{1}{x^{2}}}{x^{2}+\frac{1}{x^{2}}} d x=\int \frac{d\left(x+\frac{1}{x}\right)}{\left(x+\frac{1}{x}\right)^{2}-2} \\
&=\frac{1}{2 \sqrt{2}} \ln \left(\frac{x^{2}-x \sqrt{2}+1}{x^{2}+x \sqrt{2}+1}\right)+C . \\
& 1714^{+} \text {. } \int \frac{x^{14} d x}{\left(x^{5}+1\right)^{4}} . \\
& \text { 解 } \int \frac{x^{14} d x}{\left(x^{5}+1\right)^{4}}=\int \frac{x^{14} d x}{x^{20}\left(1+x^{-5}\right)^{4}} \\
&=-\frac{1}{5} \int\left(1+x^{-5}\right)^{-4} d\left(1+x^{-5}\right) \\
&=\frac{1}{15}\left(1+x^{-5}\right)^{-3}+C_{1}=\frac{x^{15}}{15\left(x^{5}+1\right)^{3}}+C_{1} \\
&=\frac{\left(x^{5}+1\right)^{3}-3 x^{10}-3 x^{5}-1}{15\left(x^{5}+1\right)^{3}}+C_{1} \\
&=-\frac{3 x^{10}+3 x^{5}+1}{15\left(x^{5}+1\right)^{3}}+C
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1714}
  \item \(\int \frac{x^{\frac{\pi}{2}} d x}{\sqrt{1+x^{n+2}}}\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}解\end{CJK} \begin{CJK}{UTF8}{mj}当\end{CJK} \(n=-2\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\int \frac{x^{\frac{n}{2}}}{\sqrt{1+x^{n+2}}} d x=\int \frac{d x}{x \sqrt{2}}=\frac{1}{\sqrt{2}} \ln |x|+C ;
\]

\begin{CJK}{UTF8}{mj}当\end{CJK} \(n \neq-2\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{x^{\frac{n}{2}}}{\sqrt{1+x^{n+2}}} d x=\frac{2}{n+2} \int \frac{d\left(x^{\frac{n+2}{2}}\right)}{\sqrt{1+\left(x^{\frac{n+2}{2}}\right)^{2}}} \\
= & \frac{2}{n+2} \ln \left(x^{\frac{n+2}{2}}+\sqrt{1+x^{n+2}}\right)+C .
\end{aligned}
\]

\[
\begin{aligned}
1716^{+} . & \int \frac{1}{1-x^{2}} \ln \frac{1+x}{1-x} d x . \\
\text { 解 } & \int \frac{1}{1-x^{2}} \ln \frac{1+x}{1-x} d x \\
& =\frac{1}{2} \int \ln \frac{1+x}{1-x} d\left(\ln \frac{1+x}{1-x}\right) \\
& =\frac{1}{4} \ln ^{2} \frac{1+x}{1-x}+C .
\end{aligned}
\]

-1717. \(\int \frac{\cos x d x}{\sqrt{2+\cos 2 x}}\).

\[
\text { 解 } \begin{aligned}
& \int \frac{\cos x d x}{\sqrt{2+\cos 2 x}}=\int \frac{d(\sin x)}{\sqrt{3-2 \sin ^{2} x}} \\
= & \frac{1}{\sqrt{2}} \arcsin \left[\sqrt{\frac{2}{3}} \sin x\right]+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1717}
  \item \(\int \frac{\sin x \cos x}{\sin ^{4} x+\cos ^{4} x} d x\).
\end{enumerate}

\[
\text { A解 } \begin{aligned}
& \int \frac{\sin x \cos x}{\sin ^{4} x+\cos ^{4} x} d x \\
= & \frac{1}{2} \int \frac{\sin 2 x d x}{1-\frac{1}{2} \sin ^{2} 2 x} \\
= & -\frac{1}{4} \int \frac{d\left(\cos ^{2} 2 x\right)}{\frac{1+\cos ^{2} 2 x}{2}} \\
= & -\frac{1}{2} \operatorname{arctg}(\cos 2 x)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1718}
  \item \(\int \frac{2^{x}+3^{x}}{9^{x}-4^{x}} d x\).
\end{enumerate}

\[
\sin ^{2} \int \frac{2^{x} \cdot 3^{x}}{9^{x}-4^{x}} d x=\int \frac{\left(\frac{3}{2}\right)^{x}}{\left(\left(\frac{3}{2}\right)^{x}\right)^{2}-1} d x
\]

\[
\begin{aligned}
& =\frac{1}{\ln 3-\ln 2} \int \frac{d\left[\left(\frac{3}{2}\right)^{2}\right]}{\left(\left(\frac{3}{2}\right)^{2}\right]^{2}-1} \\
& =\frac{1}{2(\ln 3-\ln 2)} \ln \left|\frac{3^{x}-2^{x}}{3^{x}+2^{x}}\right|+C . \\
& \text { 1720. } \int \frac{x d x}{\sqrt{1+x^{2}+\sqrt{\left(1+x^{2}\right)^{3}}}} \text {. } \\
& \text { 解 } \int \frac{x d x}{\sqrt{1+x^{2}+\sqrt{\left(1+x^{2}\right)^{3}}}} \\
& =\frac{1}{2} \int \frac{d\left(1+x^{2}\right)}{\sqrt{1+x^{2}} \cdot \sqrt{1+\sqrt{1+x^{2}}}} \\
& =\int \frac{d\left(1+\sqrt{1+x^{2}}\right)}{\sqrt{1+\sqrt{1+x^{2}}}} \\
& =2 \sqrt{1+\sqrt{1+x^{2}}}+C \text {. }
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}用分项积分法计算下列积分\end{CJK}:

\begin{enumerate}
  \setcounter{enumi}{1720}
  \item \(\int x^{2}\left(2-3 x^{2}\right)^{2} d x\).
\end{enumerate}

\[
\begin{aligned}
& =\frac{4}{3} x^{3}-\frac{12}{5} x^{5}+\frac{9}{7} x^{7}+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1721}
  \item \(\int \frac{1+x}{1-x} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{1+x}{1-x} d x=\int\left(-1+\frac{2}{1-x}\right) d x \\
= & -x-2 \ln |1-x|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1722}
  \item \(\int \frac{x^{2}}{1+x} d x\).
\end{enumerate}

\begin{center}
\includegraphics[max width=\textwidth]{2022_12_26_c19bf7cf4ca87c30c547g-026}
\end{center}

\[
\begin{aligned}
& \int \frac{x^{2}}{1+x} d x=\int\left(x-1+\frac{1}{1+x}\right) d x \\
= & \frac{1}{2} x^{2}-x+\ln |1+x|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1723}
  \item \(\int \frac{x^{3}}{3+x} d x\)
\end{enumerate}

\[
\text { A } \begin{aligned}
& \int \frac{x^{3}}{3+x} d x=\int\left(x^{2}-3 x+9-\frac{27}{3+x}\right) d x \\
= & \frac{1}{3} x^{3}-\frac{3}{2} x^{2}+9 x-27 \ln |3+x|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1724}
  \item \(\int \frac{(1+x)^{2}}{1+x^{2}} d x\).
\end{enumerate}

\[
\begin{aligned}
& A \int \frac{\left(1+x^{2}\right.}{1+x^{2}} d x=\int\left(1+\frac{2 x}{1+x^{2}}\right) d x \\
& =x+\ln \left(1+x^{2}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1725}
  \item \(\int \frac{(2-x)^{2}}{2-x^{2}} d x\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{(2-x)^{2}}{2-x^{2}} d x=\int \frac{\left(x^{2}-2\right)-4 x+6}{2-x^{2}} d x \\
= & \int\left(-1-\frac{4 x}{2-x^{2}}+\frac{6}{2-x^{2}}\right) d x \\
= & -x+2 \ln \left|2-x^{2}\right|+\frac{3}{\sqrt{2}} \ln \left|\frac{\sqrt{2}+x}{\sqrt{2}-x}\right|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1726}
  \item \(\int \frac{x^{2}}{(1-x)^{100}} d x\)
\end{enumerate}

\[
\text { A } \begin{aligned}
& \int \frac{x^{2}}{(1-x)^{100}} d x=\int \frac{(x-1+1)^{2}}{(1-x)^{100}} d x \\
= & \int\left[(1-x)^{-98}-2(1-x)^{-99}+(1-x)^{-100}\right] d x \\
= & \frac{1}{97(1-x)^{97}}-\frac{-1}{49(1-x)^{98}}+\frac{1}{99(1-x)^{99}}+C
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1727}
  \item \(\int \frac{x^{5}}{x+1} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x^{5}}{x+1} d x=\int\left(x^{4}-x^{3}+x^{2}-x+1-\frac{1}{x+1}\right) d x \\
= & \frac{1}{5} x^{5}-\frac{1}{4} x^{4}+\frac{1}{3} x^{3}-\frac{1}{2} x^{2}+x-\ln |1+x|+C .
\end{aligned}
\]

1729.

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{x+1}+\sqrt{x-1}} . \\
& \text { 解 } \int \frac{d x}{\sqrt{x+1}+\sqrt{x-1}} \\
& =\int \frac{1}{2}(\sqrt{x+1}-\sqrt{x-1}) d x \\
& =\frac{1}{3}\left[(x+1)^{\frac{3}{2}}-(x-1)^{\frac{3}{2}}\right]+C .
\end{aligned}
\]

1730

\[
\begin{aligned}
\int x & \sqrt{2-5 x} d x . \\
& \iint x \sqrt{2-5 x} d x \\
= & \int\left[-\frac{1}{5}(2-5 x)+\frac{2}{5}\right](2-5 x)^{\frac{1}{2}} d x \\
= & \int\left[-\frac{1}{5}(2-5 x)^{\frac{3}{2}}+\frac{2}{5}(2-5 x)^{\frac{1}{2}}\right] d x \\
= & \frac{2}{125}(2-5 x)^{\frac{5}{2}}-\frac{4}{75}(2-5 x)^{\frac{3}{2}}+C \\
= & -\frac{8+30 x}{375}(2-5 x)^{\frac{3}{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1730}
  \item \(\int \frac{x d x}{\sqrt[3]{1-3 x}}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x d x}{\sqrt[3]{1-3 x}}=-\frac{1}{3} \int \frac{(1-3 x)-1}{(1-3 x)^{\frac{1}{3}}} d x \\
= & -\frac{1}{3} \int\left[(1-3 x)^{\frac{2}{3}}-(1-3 x)^{-\frac{1}{3}}\right] d x
\end{aligned}
\]

\[
\begin{aligned}
& =\frac{1}{15}(1-3 x)^{\frac{5}{3}}-\frac{1}{6}(1-3 x)^{\frac{2}{3}}+C \\
& =-\frac{1+2 x}{10}(1-3 x)^{\frac{2}{3}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1731}
  \item \(\int x^{3} \sqrt[3]{1+x^{2}} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int x^{3} \sqrt[3]{1+x^{2}} d x \\
= & \frac{1}{2} \int\left[\left(x^{2}+1\right)-1\right]\left(1+x^{2}\right)^{\frac{1}{3}} d\left(1+x^{2}\right) \\
= & \frac{1}{2} \int\left[\left(1+x^{2}\right)^{\frac{4}{3}}-\left(1+x^{2}\right)^{\frac{1}{3}}\right] d\left(1+x^{2}\right) \\
= & \frac{3}{14}\left(1+x^{2}\right)^{\frac{7}{3}}-\frac{3}{8}\left(1+x^{2}\right)^{\frac{4}{3}}+C \\
= & \frac{12 x^{2}-9}{56}\left(1+x^{2}\right)^{\frac{4}{3}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1732}
  \item \(\int \frac{d x}{(x-1)(x+3)}\).
\end{enumerate}

\[
\text { ง7 } \begin{aligned}
& \int \frac{d x}{(x-1)(x+3)}=\frac{1}{4} \int\left(\frac{1}{x-1}-\frac{1}{x+3}\right) d x \\
= & \frac{1}{4} \ln \left|\frac{x-1}{x+3}\right|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1733}
  \item \(\int \frac{d x}{x^{2}+x-2}\).
\end{enumerate}

\[
\text { 昭 } \begin{aligned}
& \int \frac{d x}{x^{2}+x-2}=\frac{1}{3} \int\left(\frac{1}{x-1}-\frac{1}{x+2}\right) d x \\
= & \frac{1}{3} \ln \left|\frac{x-1}{x+2}\right|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1734}
  \item \(\int \frac{d x}{\left(x^{2}+1\right)\left(x^{2}+2\right)}\).
\end{enumerate}

\[
\text { 䨐 } \int \frac{d x}{\left(x^{2}+1\right)\left(x^{2}+2\right)}=\int\left(\frac{1}{x^{2}+1}-\frac{1}{x^{2}+2}\right) d x
\]

\[
=\operatorname{arctg} x-\frac{1}{\sqrt{2}} \operatorname{arctg} \frac{x}{\sqrt{2}}+C .
\]

\begin{enumerate}
  \setcounter{enumi}{1735}
  \item \(\int \frac{d x}{\left(x^{2}-2\right)\left(x^{2}+3\right)}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{d x}{\left(x^{2}-2\right)\left(x^{2}+3\right)}=\frac{1}{5} \int\left(\frac{1}{x^{2}-2}-\frac{1}{x^{2}+3}\right) d x \\
= & \frac{1}{10 \sqrt{2}} \ln \left|\frac{x-\sqrt{2}}{x+\sqrt{2}}\right|-\frac{1}{5 \sqrt{3}} \operatorname{arctg} \frac{x}{\sqrt{3}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1736}
  \item \(\int \frac{x d x}{(x+2)(x+3)}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x d x}{(x+2)(x+3)}=\int\left(\frac{3}{x+3}-\frac{2}{x+2}\right) d x \\
& =\ln \frac{|x+3|^{3}}{(x+2)^{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1737}
  \item \(\int \frac{x d x}{x^{4}+3 x^{2}+2}\).
\end{enumerate}

\[
\text { 生 } \begin{aligned}
& \int \frac{x d x}{x^{4}+3 x^{2}+2}=\frac{1}{2} \int \frac{d\left(x^{2}\right)}{\left(x^{2}+1\right)\left(x^{2}+2\right)} \\
= & \frac{1}{2} \int\left(\frac{1}{x^{2}+1}-\frac{1}{x^{2}+2}\right) d\left(x^{2}\right) \\
= & \frac{1}{2} \ln \frac{x^{2}+1}{x^{2}+2}+C,
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1738}
  \item \(\int \frac{d x}{(x+a)^{2}(x+b)^{2}}(a \neq b)\).
\end{enumerate}

\[
\text { คip } \begin{aligned}
& \int \frac{d x}{(x+a)^{2}(x+b)^{2}} \\
= & \frac{1}{(a-b)^{2}} \int\left(\frac{1}{x+a}-\frac{1}{x+b}\right)^{2} d x \\
= & \frac{1}{(a-b)^{2}} \int\left[\frac{1}{(x+a)^{2}}+\frac{1}{(x+b)^{2}}\right. \\
& \left.-\frac{2}{(x+a)(x+b)}\right] d x
\end{aligned}
\]

\[
\begin{aligned}
& =\frac{1}{2} \int[\cos \alpha-\cos (2 x+\alpha)] d x \\
& =\frac{x}{2} \cos \alpha-\frac{1}{4} \sin (2 x+\alpha)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1743}
  \item \(\int \sin 3 x \cdot \sin 5 x d x\)
\end{enumerate}

\[
\begin{aligned}
& \int \sin 3 x \cdot \sin 5 x d x=\frac{1}{2} \int(\cos 2 x-\cos 8 x) d x \\
= & \frac{1}{4} \sin 2 x-\frac{1}{16} \sin 8 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1744}
  \item \(\int \cos \frac{x}{2} \cdot \cos \frac{x}{3} d x\).
\end{enumerate}

\[
\text { Aि } \begin{aligned}
& \int \cos \frac{x}{2} \cdot \cos \frac{x}{3} d x=\frac{1}{2} \int\left(\cos \frac{5 x}{6}+\cos \frac{x}{6}\right) d x \\
= & \frac{3}{5} \sin \frac{5 x}{6}+3 \sin \frac{x}{6}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1745}
  \item \(\int \sin \left(2 x-\frac{\pi}{6}\right) \cdot \cos \left(3 x+\frac{\pi}{4}\right) d x\).
\end{enumerate}

\[
\text { 龶 } \begin{aligned}
& \int \sin \left(2 x-\frac{\pi}{6}\right) \cdot \cos \left(3 x+\frac{\pi}{4}\right) d x \\
= & \frac{1}{2} \int\left[\sin \left(5 x+\frac{\pi}{12}\right)-\sin \left(x+\frac{5 \pi}{12}\right)\right] d x \\
= & -\frac{1}{10} \cos \left(5 x+\frac{\pi}{12}\right)+\frac{1}{2} \cos \left(x+\frac{5 \pi}{12}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1746}
  \item \(\int \sin ^{3} x d x\).
\end{enumerate}

\[
\begin{aligned}
& \int \sin ^{3} x d x=\int\left(\cos ^{2} x-1\right) d(\cos x) \\
= & \frac{1}{3} \cos ^{3} x-\cos x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1747}
  \item \(\int \cos ^{3} x d x\)
\end{enumerate}

\[
\text { A } \int \cos ^{3} x d x=\int\left(1-\sin ^{2} x\right) d(\sin x)
\]

\[
=\sin x-\frac{1}{3} \sin ^{3} x+C .
\]

\begin{enumerate}
  \setcounter{enumi}{1748}
  \item \(\int \sin ^{4} x d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \sin ^{4} x d x=\int\left(\frac{1-\cos 2 x}{2}\right)^{2} d x \\
= & \frac{1}{4} \int\left(1-2 \cos 2 x+\frac{1+\cos 4 x}{2}\right) d x \\
= & \frac{1}{8} \int(3-4 \cos 2 x+\cos 4 x) d x \\
= & \frac{3}{8} x-\frac{1}{4} \sin 2 x+\frac{1}{32} \sin 4 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1749}
  \item \(\int \cos ^{4} x d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \cos ^{4} x d x=\int\left(\frac{1+\cos 2 x}{2}\right)^{2} d x \\
= & \frac{1}{4} \int\left(1+2 \cos 2 x+\frac{1+\cos 4 x}{2}\right) d x \\
= & \frac{1}{8} \int(3+4 \cos 2 x+\cos 4 x) d x \\
= & \frac{3}{8} x+\frac{1}{4} \sin 2 x+\frac{1}{32} \sin 4 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1750}
  \item \(\int \operatorname{ctg}^{2} x d x\).
\end{enumerate}

\[
\text { 1. } \int \operatorname{ctg}^{2} x d x=\int\left(\csc ^{2} x-1\right) d x=-\operatorname{ctg} x-x+C \text {. }
\]

\begin{enumerate}
  \setcounter{enumi}{1751}
  \item \(\int \operatorname{tg}^{3} x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { Aา } \int \operatorname{tg}^{3} x d x=\int \operatorname{tg} x \cdot\left(\sec ^{2} x-1\right) d x \\
& =\int \operatorname{tg} x d(\operatorname{tg} x)-\int \operatorname{tg} x d x \\
& =\frac{1}{2} \operatorname{tg}^{2} x+\ln |\cos x|+C \text {, } 
\end{aligned}
\]

\section{其中第二个积分见 1697 题.}
\begin{enumerate}
  \setcounter{enumi}{1752}
  \item \(\int \sin ^{2} 3 x \cdot \sin ^{3} 2 x d x\).
\end{enumerate}

\section{解冭为}
\[
\begin{aligned}
\sin ^{2} 3 x & \cdot \sin ^{3} 2 x=\frac{1}{2}(1-\cos 6 x) \cdot \frac{1}{4}(3 \sin 2 x-\sin 6 x) \\
= & \frac{1}{8}(3 \sin 2 x-3 \cos 6 x \cdot \sin 2 x-\sin 6 x \\
& +\sin 6 x \cdot \cos 6 x) \\
= & \frac{3}{8} \sin 2 x+\frac{3}{16} \sin 4 x-\frac{1}{8} \sin 6 x-\frac{3}{16} \sin 8 x \\
& +\frac{1}{16} \sin 12 x
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}所以\end{CJK}, \begin{CJK}{UTF8}{mj}得\end{CJK}

\[
\begin{array}{r}
\int \sin ^{2} 3 x \cdot \sin ^{3} 2 x d x=-\frac{3}{16} \cos 2 x-\frac{3}{64} \cos 4 x \\
+\frac{1}{48} \cos 6 x+\frac{3}{128} \cos 8 x-\frac{1}{192} \cos 12 x+C .
\end{array}
\]

\begin{enumerate}
  \setcounter{enumi}{1753}
  \item \(\int \frac{d x}{\sin ^{2} x \cdot \cos ^{2} x}\).
\end{enumerate}

\[
\text { 告 } \begin{aligned}
& \int \frac{d x}{\sin ^{2} x \cdot \cos ^{2} x}=\int\left(\frac{1}{\sin ^{2} x}+\frac{1}{\cos ^{2} x}\right) d x \\
= & -\operatorname{ctg} x+\operatorname{tg} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1754}
  \item \(\int \frac{d x}{\sin ^{2} x \cdot \cos x}\).
\end{enumerate}

\[
\text { 册 } \begin{aligned}
& \int \frac{d x}{\sin ^{2} x \cdot \cos x}=\int\left(\frac{1}{\cos x}+\frac{\cos x}{\sin ^{2} x}\right) d x \\
= & \int \frac{d x}{\cos x}+\int \frac{d(\sin x)}{\sin ^{2} x} \\
= & \ln \left|\operatorname{tg}\left(\frac{\pi}{2}+\frac{\pi}{4}\right)\right|-\frac{1}{\sin x}+C,
\end{aligned}
\]

\section{其中第一个积分见 1704 题.}
\[
\text { 1756. } \begin{aligned}
& \int \frac{d x}{\sin x \cdot \cos ^{3} x}, \\
& \text { An } \quad \int \frac{d x}{\sin x \cdot \cos ^{3} x}=\int\left(\frac{\sin x}{\cos ^{3} x}+\frac{1}{\sin x \cos x}\right) d x \\
= & -\int \frac{d(\cos x)}{\cos ^{3} x}+\int \frac{d(2 x)}{\sin 2 x} \\
= & \frac{1}{2 \cos ^{2} x}+\ln |\operatorname{tg} x|+C,
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}其中第二个积分见\end{CJK} 1703 \begin{CJK}{UTF8}{mj}题\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1756}
  \item \(\int \frac{\cos ^{3} x}{\sin x} d x\).
\end{enumerate}

\[
\text { 偰 } \begin{aligned}
& \int \frac{\cos ^{3} x}{\sin x} d x=\int \frac{1-\sin ^{2} x}{\sin x} \cos x d x \\
= & \int\left(\frac{1}{\sin x}-\sin x\right) d(\sin x) \\
= & \ln |\sin x|-\frac{1}{2} \sin ^{2} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1757}
  \item \(\int \frac{d x}{\cos ^{4} x}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{d x}{\cos ^{4} x}=\int \sec ^{2} x \cdot \frac{d x}{\cos ^{2} x}=\int\left(1+\operatorname{tg}^{2} x\right) d(\operatorname{tg} x) \\
= & \operatorname{tg} x+\frac{1}{3} \operatorname{tg}^{3} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1758}
  \item \(\int \frac{d x}{1+e^{x}}\).
\end{enumerate}

\[
\text { 情 } \int \frac{d x}{1+e^{x}}=\int\left(1-\frac{e^{x}}{1+e^{x}}\right) d x=x-\ln \left(1+e^{x}\right)+C \text {. }
\]

\begin{enumerate}
  \setcounter{enumi}{1759}
  \item \(\int \frac{\left(1+e^{x}\right)^{2}}{1+e^{2 X}} d x\).
\end{enumerate}

\[
\text { n) } \int \frac{\left(1+e^{x}\right)^{2}}{1+e^{2 x}} d x=\int\left(1+\frac{2 e^{x}}{1+e^{2 x}}\right) d x
\]

\[
=x+2 \operatorname{arc} \operatorname{tg}\left(e^{x}\right)+C
\]

\begin{enumerate}
  \setcounter{enumi}{1760}
  \item \(\int \operatorname{sh}^{2} x d x\)
\end{enumerate}

\[
\text { A } \int \operatorname{sh}^{2} x d x=\int \frac{\operatorname{ch} 2 x+1}{2} d x=\frac{1}{4} \operatorname{sh} 2 x+\frac{x}{2}+C \text {. }
\]

\(1762+\int \operatorname{ch}^{2} x d x\)

\[
\text { \$ } \int \operatorname{ch}^{2} x d x=\int \frac{\operatorname{ch} 2 x+1}{2} d x=\frac{1}{4} \operatorname{sh} 2 x+\frac{x}{2}+C
\]

\begin{enumerate}
  \setcounter{enumi}{1762}
  \item \(\int \operatorname{sh} x \cdot \operatorname{sh} 2 x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { NP } \int \operatorname{sh} x \cdot \operatorname{sh} 2 x d x=2 \int \operatorname{sh}^{2} x \operatorname{ch} x d x=2 \int \operatorname{sh}^{2} x d(\operatorname{sh} x) \\
& =\frac{2}{3} \operatorname{sh}^{3} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1763}
  \item \(\int \operatorname{ch} x \cdot \operatorname{ch} 3 x d x\).
\end{enumerate}

\[
\begin{aligned}
& \int \operatorname{ch} x \cdot \operatorname{ch} 3 x d x=\frac{1}{2} \int(\operatorname{ch} 4 x+\operatorname{ch} 2 x) d x \\
= & \frac{1}{8} \operatorname{sh} 4 x+\frac{1}{4} \operatorname{sh} 2 x+C
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1764}
  \item \(\int \frac{d x}{\operatorname{sh}^{2} x \cdot \mathrm{ch}^{2} x}\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{d x}{\operatorname{sh}^{2} x \cdot \operatorname{ch}^{2} x}=\int\left(\frac{1}{\operatorname{sh}^{2} x}-\frac{1}{\operatorname{ch}^{2} x}\right) d x \\
= & -(\operatorname{cth} x+\operatorname{th} x)+C .
\end{aligned}
\]

\section{用适当的仹抰求下列和分：}
\begin{enumerate}
  \setcounter{enumi}{1765}
  \item \(\int x^{2} \sqrt[3]{1-x} d x\)
\end{enumerate}

\(A\) \begin{CJK}{UTF8}{mj}设\end{CJK} \(1-x=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x=1-t, d x=-d t\), \begin{CJK}{UTF8}{mj}故得\end{CJK}

\[
\begin{aligned}
& \int x^{2} \sqrt[3]{1-x} d x=-\int(1-t)^{2} t^{\frac{1}{3}} d t \\
& =-\int\left(t^{\frac{1}{3}}-2 t^{\frac{4}{3}}+t^{\frac{7}{3}}\right) d t \\
& =-\frac{3}{4} t^{\frac{1}{3}}+\frac{6}{7} t^{\frac{7}{3}}-\frac{3}{10} t^{\frac{10}{3}}+C \\
& =-\frac{3}{140}\left(9+12 x+14 x^{2}\right)(1-x)^{\frac{1}{3}}+C \\
& \text { 1767. } \int x^{3}\left(1-5 x^{2}\right)^{10} d x \text {. } \\
& \rightarrow \text { 设 } 1-5 x^{2}=t \text {, 则 } x^{2}=\frac{1}{5}(1-t), \text { 从而 } x^{3} d x \\
& =\frac{1}{2} x^{2} d\left(x^{2}\right)=\frac{1}{10}(1-t)\left(-\frac{1}{5}\right) d t \\
& =-\frac{1}{50}(1-t) d t \text {, 故得 } \\
& \int x^{3}\left(1-5 x^{2}\right)^{10} d x=-\frac{1}{50} \int\left(t^{10}-t^{11}\right) d t \\
& =-\frac{1}{550} t^{11}+\frac{1}{600} t^{12}+C \\
& =-\frac{1+55 x^{2}}{6600}\left(1-5 x^{2}\right)^{11}+C \text {. } \\
& \text { 1768. } \int \frac{x^{2}}{\sqrt{2-x}} d x \text {. } \\
& \text { 午 设 } 2-x=t \text {, 则 } x=2-t, d x=-d t \text {, 故得 } \\
& \int \frac{x^{2}}{\sqrt{2-x}} d x=-\int t^{-\frac{1}{2}}(2-t)^{2} d t \\
& =-\int\left(4 t^{-\frac{1}{2}}-4 t^{\frac{1}{2}}+t^{\frac{3}{2}}\right) d t \\
& =-8 t^{\frac{1}{2}}+\frac{8}{3} t^{\frac{3}{2}}-\frac{2}{5} t^{\frac{5}{2}}+C \\
& =-\frac{2}{15}\left(32+8 x+3 x^{2}\right) \sqrt{2-x}+C \text {. } 
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1768}
  \item \(\int \frac{x^{5}}{\sqrt{1-x^{2}}} d x\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}解\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(1-x^{2}=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x^{2}=1-t\), \begin{CJK}{UTF8}{mj}从而\end{CJK} \(x^{5} d x=\frac{1}{2}\left(x^{2}\right)^{2}\)

\begin{itemize}
  \item \(d\left(x^{2}\right)=-\frac{1}{2}(1-t)^{2} d t\), \begin{CJK}{UTF8}{mj}故得\end{CJK}
\end{itemize}

\(\int \frac{x^{5}}{\sqrt{1-x^{2}}} d x=-\frac{1}{2} \int t^{-\frac{1}{2}}(1-t)^{2} d t\)

\(=-\frac{1}{2} \int\left(t^{-\frac{1}{2}}-2 t^{\frac{1}{2}}+t^{\frac{3}{2}}\right) d t\)

\(=-t^{\frac{1}{2}}+\frac{2}{3} t^{\frac{3}{2}}-\frac{1}{5} t^{\frac{5}{2}}+C\)

\(=-\frac{1}{15}\left(8+4 x^{2}+3 x^{4}\right) \sqrt{1-x^{2}}+C\).

\begin{enumerate}
  \setcounter{enumi}{1769}
  \item \(\int x^{5}\left(2-5 x^{3}\right)^{\frac{2}{3}} d x\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}解\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(2-5 x^{3}=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x^{3}=\frac{1}{5}(2-t)\), \begin{CJK}{UTF8}{mj}从而\end{CJK} \(x^{5} d x=\frac{1}{3} x^{3} d\left(x^{3}\right)=-\frac{1}{75}(2-t) d t\)

\begin{CJK}{UTF8}{mj}故得\end{CJK}

\(\int x^{5}\left(2-5 x^{3}\right)^{\frac{2}{3}} d x=-\frac{1}{75} \int t^{\frac{2}{3}}(2-t) d t\)

\(=-\frac{1}{75} \int\left(2 t^{\frac{2}{3}}-t^{\frac{5}{3}}\right) d t=-\frac{2}{125} t^{\frac{5}{3}}+\frac{1}{200} t^{\frac{8}{3}}+C\)

\(=-\frac{6+25 x^{3}}{1000}\left(2-5 x^{3}\right)^{\frac{5}{3}}+C\).

\(1771^{+} . \int \cos ^{5} x \sqrt{\sin x} d x\).

\begin{CJK}{UTF8}{mj}媈\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(\sin x=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(\cos ^{5} x d x=\left(1-\sin ^{2} x\right)^{2} d(\sin x)\)

\(=\left(1-t^{2}\right)^{z} d t\),

\begin{CJK}{UTF8}{mj}故得\end{CJK}

36

\[
\begin{aligned}
& \int \cos ^{5} x \sqrt{\sin x} d x=\int\left(1-t^{2}\right)^{2} t^{\frac{1}{2}} d t \\
= & \int\left(t^{\frac{1}{2}}-2 t^{\frac{5}{2}}+t^{\frac{9}{2}}\right) d t \\
= & \frac{2}{3} t^{\frac{3}{2}}-\frac{4}{7} t^{\frac{7}{2}}+\frac{2}{11} t^{\frac{11}{2}}+C \\
= & \left(\frac{2}{3}-\frac{4}{7} \sin ^{2} x+\frac{2}{11} \sin ^{4} x\right) \sqrt{\sin ^{3} x}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1771}
  \item \(\int \frac{\sin x \cos ^{3} x}{1+\cos ^{2} x} d x\)
\end{enumerate}

\begin{CJK}{UTF8}{mj}用\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(\cos ^{2} x=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(\sin x \cos x d x=-\frac{1}{2} d t\), \begin{CJK}{UTF8}{mj}故得\end{CJK}

\[
\begin{aligned}
& \int \frac{\sin x \cos ^{3} x}{1+\cos ^{2} x} d x=-\frac{1}{2} \int \frac{t}{1+t} d t \\
= & -\frac{1}{2} \int\left(1-\frac{1}{1+t}\right) d t=-\frac{1}{2} t+\frac{1}{2} \ln (1+t)+C \\
= & -\frac{1}{2} \cos ^{2} x+\frac{1}{2} \ln \left(1+\cos ^{2} x\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1772}
  \item \(\int \frac{\sin ^{2} x}{\cos ^{6} x} d x\)
\end{enumerate}

A \begin{CJK}{UTF8}{mj}论\end{CJK} \(\operatorname{tg} x=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(\frac{1}{\cos ^{4} x} d x=\left(1+t^{2}\right) d t\), \begin{CJK}{UTF8}{mj}敇得\end{CJK}

\[
\begin{aligned}
& \int \frac{\sin ^{2} x}{\cos ^{6} x} d x=\int\left(t^{4}+t^{2}\right) d t=\frac{1}{5} t^{5}+\frac{1}{3} t^{3}+C \\
= & \frac{1}{5} \cdot \operatorname{tg}^{5} x+\frac{1}{3} \operatorname{tg}^{3} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1773}
  \item \(\int \frac{\ln x d x}{x \sqrt{1+\ln x}}\)
\end{enumerate}

Aif \begin{CJK}{UTF8}{mj}唼\end{CJK} \(1+\ln x=t \cdot\left[\operatorname{li} \frac{\ln x d x}{x}\right.\)

\[
\begin{aligned}
& =(1+\ln x-1) d(1+\ln x) \\
& =(t-1) d t, \text { 敇㥂 }
\end{aligned}
\]

\[
\begin{aligned}
& \int \frac{\ln x d x}{x \sqrt{1+\ln x}}=\int t^{-\frac{1}{2}}(t-1) d t \\
= & \int\left(t^{\frac{1}{2}}-t^{-\frac{1}{2}}\right) d t=\frac{2}{3} t^{\frac{3}{2}}-2 t^{\frac{1}{2}}+C \\
= & \frac{2}{3}(\ln x-2) \sqrt{1+\ln x}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1774}
  \item \(\int \frac{d x}{e^{\frac{x}{2}}+e^{x}}\)
\end{enumerate}

\[
\text { A朝 } \begin{aligned}
& e^{\frac{x}{2}}=t, \text { 倫 } e^{x}=t^{2}, d x=\frac{2 d t}{t} \text {, 故得 } \\
& \int \frac{d x}{e^{2}+e^{x}}=2 \int \frac{d t}{t^{2}(1+t)}=2 \int\left(\frac{1-t}{t^{2}}+\frac{1}{1+t}\right) d t \\
&=-\frac{2}{t}-2 \ln t+2 \ln (1+t)+C \\
&=-2 e^{-\frac{x}{2}}-x+2 \ln \left(1+e^{\frac{x}{2}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1775}
  \item \(\int \frac{d x}{\sqrt{1+e^{x}}}\)
\end{enumerate}

\begin{CJK}{UTF8}{mj}川\end{CJK} \begin{CJK}{UTF8}{mj}沒\end{CJK} \(\sqrt{1+e^{x}}=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x=\ln \left(t^{2}-1\right), d x=\frac{2 t}{t^{2}-1} d t\), \begin{CJK}{UTF8}{mj}姑得\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{1+e^{x}}} \\
= & 2 \int \frac{d t}{t^{2}-1}=\ln \left(\frac{t-1}{t+1}\right)+C \\
= & \ln \left(\frac{\sqrt{1+e^{x}}-1}{\sqrt{1+e^{x}}+1}\right)+C \\
= & x-2 \ln \left(1+\sqrt{1+e^{x}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1776}
  \item \(\int \frac{\operatorname{arctg} \sqrt{x}}{\sqrt{x}} \cdot \frac{d x}{1+x}\). \begin{CJK}{UTF8}{mj}代入得\end{CJK}
\end{enumerate}

\[
\begin{aligned}
& \int \frac{x^{2} d x}{\sqrt{x^{2}-2}}=2 \int \sec ^{3} t d t=2 \int \frac{d(\sin t)}{\left(1-\sin ^{2} t\right)^{2}} \\
= & \frac{1}{2} \int\left(\frac{1}{1+\sin t}+\frac{1}{1-\sin t}\right)^{2} d(\sin t) \\
= & \frac{1}{2} \int \frac{d(1+\sin t)}{(1+\sin t)^{2}}-\frac{1}{2} \int \frac{d(1-\sin t)}{(1-\sin t)^{2}} \\
& +\int \frac{d(\sin t)}{1-\sin ^{2} t} \\
= & \frac{1}{2}\left(\frac{1}{1-\sin t}-\frac{1}{1+\sin t}\right)+\frac{1}{2} \ln \left(\frac{1+\sin t}{1-\sin t}\right)+C_{1} \\
= & \operatorname{tg} t \cdot \sec t+\ln (\sec t+\operatorname{tg} t)+C_{1} \\
= & \frac{x}{2} \sqrt{x^{2}-2}+\ln \left(x+\sqrt{x^{2}-2}\right)+C .
\end{aligned}
\]

（2）\begin{CJK}{UTF8}{mj}当\end{CJK} \(x<-\sqrt{2}\) \begin{CJK}{UTF8}{mj}时\end{CJK}, \begin{CJK}{UTF8}{mj}仍设\end{CJK} \(x=\sqrt{2} \mathrm{sect}\), \begin{CJK}{UTF8}{mj}但㡾制\end{CJK} \(\pi<t<\frac{3 \pi}{2}\). \begin{CJK}{UTF8}{mj}其余步䎿与上相同\end{CJK}, \begin{CJK}{UTF8}{mj}注意到\end{CJK}, \begin{CJK}{UTF8}{mj}此时\end{CJK} \(\sec t+\operatorname{tg} t\) \(<0\), \begin{CJK}{UTF8}{mj}因此在对数符号里要加绝对值\end{CJK}, \begin{CJK}{UTF8}{mj}即结果为\end{CJK}

\[
\frac{x}{2} \sqrt{x^{2}-2}+\ln \left|x+\sqrt{x^{2}-2}\right|+C .
\]

\begin{CJK}{UTF8}{mj}总之\end{CJK},\begin{CJK}{UTF8}{mj}当\end{CJK} \(|x|>\sqrt{2}\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\int \frac{x^{2} d x}{\sqrt{x^{2}-2}}=\frac{x}{2} \sqrt{x^{2}-2}+\ln \left|x+\sqrt{x^{2}-2}\right|+C .
\]

7780: \(\int \sqrt{a^{2}-x^{2}} d x\).

त\begin{CJK}{UTF8}{mj}单被积函数的存在域为\end{CJK} \(-a \leqslant x \leqslant a\). \begin{CJK}{UTF8}{mj}因此设\end{CJK} \(x=\) \(a \sin t\), \begin{CJK}{UTF8}{mj}并限制\end{CJK} \(-\frac{\pi}{2} \leqslant t \leqslant \frac{\pi}{2}\). \begin{CJK}{UTF8}{mj}从而\end{CJK}

\[
\sqrt{a^{2}-x^{2}}=a \cos t, d x=a \cos t d t .
\]

\begin{CJK}{UTF8}{mj}代入得\end{CJK}

\[
\begin{aligned}
& \int \sqrt{a^{2}-x^{2}} d x=a^{2} \int \cos ^{2} t d t . \\
= & a^{2}\left(\frac{t}{2}+\frac{1}{4} \sin 2 t\right)+C \\
= & \frac{a^{2}}{2} t+\frac{a^{2}}{2} \sin t \cos t+C \\
= & \frac{a^{2}}{2} \arcsin \frac{x}{a}+\frac{x}{2} \sqrt{a^{2}-x^{2}}+C .
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1742 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1780}
  \item \(\int \frac{d x}{\left(x^{2}+a^{2}\right)^{\frac{3}{2}}}\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}羘\end{CJK} \begin{CJK}{UTF8}{mj}被积函数的存在域为\end{CJK} \(-\infty<x<+\infty\), \begin{CJK}{UTF8}{mj}因此可设\end{CJK} \(x=a \operatorname{tg} t\), \begin{CJK}{UTF8}{mj}并限制\end{CJK} \(-\frac{\pi}{2}<t<\frac{\pi}{2}\). \begin{CJK}{UTF8}{mj}从而\end{CJK}

\[
\left(x^{2}+a^{2}\right)^{\frac{3}{2}}=a^{3} \sec ^{3} t, d x=a \sec ^{2} t d t .
\]

\begin{CJK}{UTF8}{mj}代入得\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{\left(x^{2}+a^{2}\right)^{\frac{3}{2}}}=\frac{1}{a^{2}} \int \cos t d t=\frac{1}{a^{2}} \sin t+C \\
= & \frac{1}{a^{2}} \cdot \frac{\operatorname{tg} t}{\sqrt{1+\operatorname{tg}^{2} t}}+C=\frac{x}{a^{2} \sqrt{a^{2}+x^{2}}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1781}
  \item \(\int \sqrt{\frac{a+x}{a-x}} d x\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}觟被积函数的存在域为\end{CJK} \(-a \leqslant x<a\), \begin{CJK}{UTF8}{mj}因此可设\end{CJK} \(x=\) \(a \sin t\), \begin{CJK}{UTF8}{mj}并限制\end{CJK} \(-\frac{\pi}{2}<t<\frac{\pi}{2}\). \begin{CJK}{UTF8}{mj}从而\end{CJK}

\[
\sqrt{\frac{a+x}{a-x}}=\sqrt{\frac{1+\sin t}{1-\sin t}}=\frac{1+\sin t}{\cos t}, d x=a \cos t d t .
\]

\begin{CJK}{UTF8}{mj}代入得\end{CJK}

\[
\begin{aligned}
& \int \sqrt{\frac{a+x}{a-x}} d x \\
= & a \int(1+\sin t) d t=a(t-\cos t)+C \\
= & a \arcsin \frac{x}{a}-\sqrt{a^{2}-x^{2}}+C(-a<x<a) .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}注意上式在端点\end{CJK} \(x=-a\) \begin{CJK}{UTF8}{mj}也戌立\end{CJK}. \begin{CJK}{UTF8}{mj}即\end{CJK} \begin{CJK}{UTF8}{mj}函数\end{CJK} \(F(x)=\) \(\operatorname{aarcsin} \frac{x}{a}-\sqrt{a^{2}-x^{2}}\) \begin{CJK}{UTF8}{mj}在点\end{CJK} \(x=-a\) \begin{CJK}{UTF8}{mj}的\end{CJK}(\begin{CJK}{UTF8}{mj}右\end{CJK}) \begin{CJK}{UTF8}{mj}昌数等于被\end{CJK} \begin{CJK}{UTF8}{mj}积函数\end{CJK} \(f(x)=\sqrt{\frac{a+x}{a-x}}\) \begin{CJK}{UTF8}{mj}在点\end{CJK} \(x=-a\) \begin{CJK}{UTF8}{mj}之值\end{CJK}.\begin{CJK}{UTF8}{mj}事宝上\end{CJK},\begin{CJK}{UTF8}{mj}由\end{CJK} \begin{CJK}{UTF8}{mj}于\end{CJK} \(F(x)\) \begin{CJK}{UTF8}{mj}和\end{CJK} \(f(x)\) \begin{CJK}{UTF8}{mj}都在\end{CJK} \(a \leqslant x<a\) \begin{CJK}{UTF8}{mj}连续\end{CJK} \begin{CJK}{UTF8}{mj}且\end{CJK} \(F^{\prime}(x)=f(x)\) \begin{CJK}{UTF8}{mj}在一\end{CJK} \(a<x<a\) \begin{CJK}{UTF8}{mj}成立\end{CJK}. \begin{CJK}{UTF8}{mj}故由中值定理\end{CJK}, \begin{CJK}{UTF8}{mj}皓当\end{CJK} \(-a<x<a\) \begin{CJK}{UTF8}{mj}时\end{CJK}, tit

\[
\begin{aligned}
& \frac{F(x)-F(-a)}{x+a}=F^{\prime}(\xi)=f(\xi),-a<\xi<x . \\
& \text { 由此可知,(㝒) 导数 } \\
& F^{\prime}(-a)=\lim _{x \rightarrow-4+0} \frac{F(x)-F(-a)}{x+a} \\
&= \lim _{t \rightarrow-\infty} f(\xi)=f(-a) .
\end{aligned}
\]

\section{下面有些题目在端点的情兄可类地迆进行讨论+从垎。～}
\begin{enumerate}
  \setcounter{enumi}{1782}
  \item \(\int x \sqrt{\frac{x}{2 a-x}} d x\).
\end{enumerate}

\includegraphics[max width=\textwidth, center]{2022_12_26_c19bf7cf4ca87c30c547g-042}\\
\(x=2 a \sin ^{2} t\),\begin{CJK}{UTF8}{mj}井限制\end{CJK} \(0 \leqslant t<\frac{\pi}{2} . B\) \begin{CJK}{UTF8}{mj}而\end{CJK}

\(x \sqrt{\frac{x}{2 a-x}}=\frac{2 a \sin ^{3} t}{\cos t}, d x=4 a \sin t \cos t d t\).

\[
\begin{aligned}
& \text { 代入得 } \\
& \int x \sqrt{\frac{x}{2 a-x}} \\
&= 8 a^{2} \int \sin ^{4} t d t \\
&= 8 a^{2}\left(\frac{3}{8} t-\frac{1}{4} \sin 2 t+\frac{1}{32} \sin 4 t\right)+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}注意到\end{CJK} \(\sin 2 t=2 \sin t \cos t=2 \sqrt{\frac{x}{2 a}} \cdot \sqrt{1-\frac{x}{2 a}}=\frac{1}{a}\). \(\sqrt{x(2 a-x)}\) B \(\sin 4 t=2 \sin 2 t \cos 2 t=4 \sin t \cos t(1 \rightarrow\) \(\left.2 \sin ^{2} t\right)=\frac{2}{a^{2}}(a-x) \sqrt{x(2 a-x)}\),\begin{CJK}{UTF8}{mj}最㕆得\end{CJK}

\[
\begin{aligned}
& \int x \sqrt{\frac{x}{2 a-x}} d x=3 a^{2} \operatorname{arc} \sin \sqrt{\frac{x}{2 a}}-2 a^{2} \cdot \\
& \frac{1}{a} \sqrt{x(2 a-x)}+\frac{1}{4} a^{2} \cdot \frac{2}{a^{2}}(a-x \sqrt{x(2 a-x)}+C \\
= & 3 a^{2} \operatorname{arc} \sin \sqrt{\frac{x}{2 a}}-\frac{3 a+x}{2} \sqrt{x(2 a-x)}+C .
\end{aligned}
\]

*)\begin{CJK}{UTF8}{mj}利申\end{CJK} 1749 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1783}
  \item \(\int \frac{d x}{\sqrt{(x-a)(b-x)}}\) *
\end{enumerate}

\includegraphics[max width=\textwidth, center]{2022_12_26_c19bf7cf4ca87c30c547g-043}\\
\begin{CJK}{UTF8}{mj}因此可沒\end{CJK} \(x-a=(b-a) \sin ^{2} t\), \begin{CJK}{UTF8}{mj}并限制\end{CJK} \(0<t<\frac{\pi}{2}\). \begin{CJK}{UTF8}{mj}从而\end{CJK} \(\sqrt{(x-a)(b-x)}=(b-a) \sin t \cos t\)

\[
d x=2(b-a) \sin t \cos t d t
\]

\begin{CJK}{UTF8}{mj}刞入㥂\end{CJK}

\[
\int \frac{d x}{\sqrt{(x-a)(b-x)}}=2 \int d t=2 t+C
\]

\[
\text { = 2arc } \sin \sqrt{\frac{x-a}{b-a}}+C
\]

\begin{enumerate}
  \setcounter{enumi}{1784}
  \item \(\int \sqrt{(x-a)(b-x)} d x\).
\end{enumerate}

\[
\text { A 写上题相同, 作同一代换,并洼意到 } \sin 4 t=4 \sin t
\]

\[
\begin{aligned}
& \cdot \cos t\left(1-2 \sin ^{2} t\right)=4 \sqrt{\frac{x-a}{b-a}} . \\
& \sqrt{1-\frac{\pi-a}{b-a}}\left(1-2 \cdot \frac{x-a}{b-a}\right) \\
& =-4 \cdot \frac{2 x-(a+b)}{(b-a)^{2}} \sqrt{(x-a)(b-x)} \text {, 即得 } \\
& \int \sqrt{(x-a)(b-x)} d x=2\left((b-a)^{2} \int \sin ^{2} t \cos ^{2} t d t\right. \\
& =\frac{(b-a)^{2}}{2} \int \sin ^{2} 2 t d t=\frac{(b-a)^{2}}{4} \int(1-\cos 4 t) d t \\
& =\frac{(b-a)^{2}}{4}\left(t-\frac{1}{4} \sin 4 t\right)+C \\
& =\frac{(b-a)^{2}}{4} \arcsin \sqrt{\frac{x-a}{b-a}} \\
& +\frac{2 x-(a+b)}{4} \sqrt{(x-a)(b-x)}+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}由双曲线佯抰\end{CJK} \(x=a \operatorname{sht} \cdot x=a \operatorname{cht}\) \begin{CJK}{UTF8}{mj}等等\end{CJK}, \begin{CJK}{UTF8}{mj}求无列积分\end{CJK} (\begin{CJK}{UTF8}{mj}㐱数为正的\end{CJK})：

\begin{enumerate}
  \setcounter{enumi}{1785}
  \item \(\int \sqrt{a^{2}+x^{2}} d x\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}玨\end{CJK} \begin{CJK}{UTF8}{mj}袂积函数的存在域为\end{CJK} \(-\infty<x<+\infty\), \begin{CJK}{UTF8}{mj}因此可\end{CJK} \begin{CJK}{UTF8}{mj}改\end{CJK} \(x=a \mathrm{sh} t\).

\[
\sqrt{a^{2}+x^{2}}=a \mathrm{ch} t, d x=a \mathrm{ch} t d t .
\]

\begin{CJK}{UTF8}{mj}什入㥂\end{CJK}

\[
\begin{aligned}
& \int \sqrt{a^{2}+x^{2}} d x=a^{2} \int \operatorname{ch}^{2} t d t \\
= & a^{2}\left(\frac{t}{2}+\frac{1}{4} \operatorname{sh} 2 t\right)^{-2}+C_{1} .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}汢意到\end{CJK} \(x+\sqrt{a^{2}+x^{2}}=a(\operatorname{sh} t+\mathrm{ch} t)=a e^{\prime}\), \begin{CJK}{UTF8}{mj}即\end{CJK} \(t=\) \(\ln \frac{x+\sqrt{a^{2}+x^{2}}}{a}\) \begin{CJK}{UTF8}{mj}及\end{CJK} \(\operatorname{sh} 2 t=2 \operatorname{shcch} t=\frac{2 x \sqrt{a^{2}+x^{2}}}{a^{2}}\),

\section{隼唐厉㥂}
\[
\begin{aligned}
& \int \sqrt{a^{2}+x^{2}} d x=\frac{a^{2}}{2} \ln \left(x+\sqrt{a^{2}+x^{2}}\right) \\
& +\frac{x}{2} \sqrt{a^{2}+x^{2}}+C
\end{aligned}
\]

**) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1762 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1786}
  \item \(\int \frac{x^{2}}{\sqrt{a^{2}+x^{2}}} d x\).
\end{enumerate}

1 \begin{CJK}{UTF8}{mj}与上题相同\end{CJK}, \begin{CJK}{UTF8}{mj}设\end{CJK} \(x=a \operatorname{sh} t\), \begin{CJK}{UTF8}{mj}则\end{CJK}

\[
\frac{x^{2}}{\sqrt{a^{2}+x^{2}}}=\frac{a \operatorname{sh}^{2} t}{\operatorname{ch} t}, d x=a \operatorname{ch} t d t .
\]

\(1+\lambda\) \begin{CJK}{UTF8}{mj}㥂\end{CJK}

\[
\begin{aligned}
& \int \frac{x^{2}}{\sqrt{a^{2}+x^{2}}} d x=a^{2} \int \operatorname{sh}^{2} t d t \\
= & a^{2}\left(\frac{1}{4} \operatorname{sh} 2 t-\frac{t}{2}\right)^{2}+C_{1} \\
= & \frac{x^{t}}{2} \sqrt{a^{2}+x^{2}}-\frac{a^{2}}{2} \ln \left(x+\sqrt{a^{2}+x^{2}}\right)+C .
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1761 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\[
1788^{+} \cdot \int \sqrt{\frac{x-a}{x+a}} d x .
\]

\begin{center}
\includegraphics[max width=\textwidth]{2022_12_26_c19bf7cf4ca87c30c547g-045}
\end{center}

（1）\begin{CJK}{UTF8}{mj}当\end{CJK} \(x>a\) \begin{CJK}{UTF8}{mj}时\end{CJK}, \begin{CJK}{UTF8}{mj}可设\end{CJK} \(x=a c h t\), \begin{CJK}{UTF8}{mj}并限制\end{CJK} \(t>0\). \begin{CJK}{UTF8}{mj}从而\end{CJK}

\[
\begin{aligned}
& \sqrt{\frac{x-a}{x+a}}=\frac{\operatorname{ch} t-1}{\operatorname{sh} t}, d x=a \operatorname{sh} t d t . \\
& \text { 代入得 } \\
& \int \sqrt{\frac{x-a}{x+a}} d x=a \int(\mathrm{ch} t-1) d t \\
&= a \operatorname{sh} t-a t+C_{1}=a \sqrt{c^{2} t-1}-a t+C_{1} \\
&= a \sqrt{\left(\frac{x}{a}\right)^{2}-1}-a \ln \left(\sqrt{\left(\frac{x}{a}\right)^{2}-1}+\frac{x}{a}\right)+C_{1} \\
&= \sqrt{x^{2}-a^{2}}-a \ln \left(\sqrt{x^{2}-a^{2}}+x\right)+C_{2} \\
&= \sqrt{x^{2}-a^{2}}-2 a \ln (\sqrt{x-a}+\sqrt{x+a})+C . \\
& \text { (2) } \text { 当 } x<-a \text { 时,可设 } x=-a \operatorname{ch} t, \text { 并限制 } t>0 . \\
& \text { 从而 } \quad \\
& \sqrt{\frac{x-a}{x+a}}=\frac{c h t}{\operatorname{sh} t}, d x=-a \operatorname{sh} t d t .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}代入得\end{CJK}

\[
\begin{aligned}
& \int \sqrt{\frac{x-a}{x+a}} d x=-a \int(\mathrm{ch} t+1) d t \\
= & -a \operatorname{sh}-a t+C_{1} \\
= & -a \cdot \sqrt{\left(\frac{x}{a}\right)^{2}-1} \\
& -a \ln \left(\sqrt{\left(\frac{x}{a}\right)^{2}-1}-\frac{x}{a}\right)+C_{1} \\
= & -\sqrt{x^{2}-a^{2}}-a \ln \left(\sqrt{x^{2}-a^{2}}-x\right)+C_{2}
\end{aligned}
\]

\[
\begin{aligned}
= & -\sqrt{x^{2}-a^{2}}-2 a \ln (\sqrt{-x+a} \\
& +\sqrt{-x-a})+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}总之\end{CJK}, \begin{CJK}{UTF8}{mj}茂\end{CJK} \(|x|>a\) \begin{CJK}{UTF8}{mj}时\end{CJK}.

\[
\begin{aligned}
& \int \sqrt{\frac{x-a}{x+a}} d x=\operatorname{sgn} x \cdot \sqrt{x^{2}-a^{2}} \\
& -2 a \ln (\sqrt{|x-a|}+\sqrt{|x+a|})+C
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1788}
  \item \(\int \frac{d x}{\sqrt{(x+a)(x+b)}}\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}皿升妨设\end{CJK} \(a<b\). \begin{CJK}{UTF8}{mj}被积函数的存在域为\end{CJK} \(x>-a\) \begin{CJK}{UTF8}{mj}及\end{CJK} \(x<-b\).

（1）\begin{CJK}{UTF8}{mj}当\end{CJK} \(x>-a\) \begin{CJK}{UTF8}{mj}时\end{CJK},\begin{CJK}{UTF8}{mj}可设\end{CJK} \(x+a=(b-a) \operatorname{sh}^{2} t+\) \begin{CJK}{UTF8}{mj}并\end{CJK} \begin{CJK}{UTF8}{mj}偍制\end{CJK} \(>0\). M\begin{CJK}{UTF8}{mj}而\end{CJK}

\[
\begin{aligned}
& \sqrt{(x+a)(x+b)}=(b-a) \operatorname{sh} t \operatorname{ch} t, d x \\
= & 2(b-a) \operatorname{sh} t c h t d t .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}斗\end{CJK} \(\lambda\) \begin{CJK}{UTF8}{mj}䅐\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{(x+a)(x+b)}}=2 \int d t=2 t+C_{1 .} \\
& \text { 洼意到 } \sqrt{x+a}+\sqrt{x+b}=\sqrt{b-a}(\operatorname{sh} t+\operatorname{ch} t)= \\
& \sqrt{b-\bar{a}} e^{r} \text {, 就有 } t=\ln \frac{\sqrt{x+a}+\sqrt{x+b}}{\sqrt{b-a}} \text {, 最居得 } \\
& \int \frac{d x}{\sqrt{(x+a)(x+b)}} \\
& =2 \ln (\sqrt{x+a}+\sqrt{x+b})+C \text {. }
\end{aligned}
\]

（2）\begin{CJK}{UTF8}{mj}当\end{CJK} \(x<-b\) \begin{CJK}{UTF8}{mj}时\end{CJK}. \begin{CJK}{UTF8}{mj}可设\end{CJK} \(x+b=(a-b) \operatorname{sh}^{2} t\), \begin{CJK}{UTF8}{mj}并限\end{CJK} \begin{CJK}{UTF8}{mj}制\end{CJK} \(t>0\). X

\[
\begin{aligned}
& \sqrt{(x+a)(x+b)}=(b-a) \operatorname{sh} t \operatorname{ch} t, d x \\
= & -(b-a) 2 \operatorname{sh} t \operatorname{ch} t d t .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}車入倡\end{CJK}

\[
\begin{gathered}
\int \frac{d x}{\sqrt{(x+a)(x+b)}}=-2 \int d t=-2 t+C_{1} \\
=-2 \ln (\sqrt{-(x+a)}+\sqrt{-(x+b)})+C_{.}
\end{gathered}
\]

e

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{(x+a)(x+b)}} \\
& =\left\{\begin{array}{c}2 \ln (\sqrt{x+\bar{a}}+\sqrt{x+b}), \\\quad \text { 䓀 } x+a>0 \text { 及 } x+b>0 ; \\-2 \ln (\sqrt{-x-a}+\sqrt{-x-b}) . \\\text { 若 } x+a<0 \text { \& } x+b<0 .\end{array}\right.
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1789}
  \item \(\int \sqrt{(x+a)(x+b)} d x\).
\end{enumerate}

\includegraphics[max width=\textwidth, center]{2022_12_26_c19bf7cf4ca87c30c547g-048}\\
\begin{CJK}{UTF8}{mj}中姦动个别地方\end{CJK}. \begin{CJK}{UTF8}{mj}今以\end{CJK} \(x>-a\) \begin{CJK}{UTF8}{mj}时冽\end{CJK}, \begin{CJK}{UTF8}{mj}㸷法如下\end{CJK}:

\[
\begin{aligned}
& \int \sqrt{(x+a)(x+\bar{b})} d x=2(b-a)^{2} \int \operatorname{sh}^{2} t \operatorname{ch}^{2} t d t \\
= & \frac{1}{2}(b-a)^{2} \int \operatorname{sh}^{2} 2 t d t \\
= & \frac{1}{4}(b-a)^{2} \int(\operatorname{ch} 4 t-1) d t \\
= & \frac{1}{4}(b-a)^{2}\left(\frac{1}{4} \operatorname{sh} 4 t-t\right)+C_{1} \\
= & \frac{1}{4}(b-a)^{2}\left[\operatorname{sh} t \operatorname{cht}\left(1+2 \operatorname{sh}^{2} t\right)-t\right]+C_{1} \\
= & \frac{1}{4}(b-a)^{2}\left[\sqrt{\frac{x+a}{b-a}} \cdot \sqrt{1+\frac{x+a}{b-a}}\right.
\end{aligned}
\]

\[
\begin{aligned}
& \text { 解 } \int \ln x d x=x \ln x-\int x \cdot \frac{1}{x} d x=x(\ln x-1)+C \text {. } \\
& \text { 1792. } \int x^{n} \ln x d x \quad(n \neq-1) \text {. } \\
& \text { 解 } \int x^{n} \ln x d x=\frac{1}{n+1} \int \ln x d\left(x^{n+1}\right)=\frac{1}{n+1} x^{n+1} \ln x \\
& -\frac{1}{n+1} \int x^{n+1} \cdot \frac{1}{x} d x=\frac{x^{n+1}}{n+1}\left(\ln x-\frac{1}{n+1}\right)+C \text {. } \\
& \text { 1793. } \int\left(\frac{\ln x}{x}\right)^{2} d x \text {. } \\
& \text { 解 } \int\left(\frac{\ln x}{x}\right)^{2} d x=-\int \ln ^{2} x d\left(\frac{1}{x}\right) \\
& =-\frac{1}{x} \ln ^{2} x+\int \frac{1}{x} \cdot 2 \ln x \cdot \frac{1}{x} d x \\
& =-\frac{1}{x} \ln ^{2} x-2 \int \ln x d\left(\frac{1}{x}\right)=-\frac{1}{x} \ln ^{2} x-\frac{2}{x} \ln x \text {. } \\
& +2 \int \frac{1}{x} \cdot \frac{1}{x} d x=-\frac{1}{x}\left(\ln ^{2} x+2 \ln x+2\right)+C \text {. } \\
& \text { 1794. } \int \sqrt{x} \ln ^{2} x d x \text {. } \\
& \text { 解 } \int \sqrt{x} \ln ^{2} x d x=\frac{2}{3} \int \ln ^{2} x d\left(x^{\frac{3}{2}}\right) \\
& =\frac{2}{3} x^{\frac{3}{2}} \ln ^{2} x-\frac{4}{3} \int x^{\frac{3}{2}} \ln x \cdot \frac{1}{x} d x \\
& =\frac{2}{3} x^{\frac{3}{2}} \ln ^{2} x-\frac{8}{9} \int \ln x d\left(x^{\frac{3}{2}}\right) \\
& =\frac{2}{3} x^{\frac{3}{2}} \ln ^{2} x-\frac{8}{9} x^{\frac{3}{2}} \ln x+\frac{8}{9} \int x^{\frac{3}{2}} \cdot \frac{1}{x} d x \\
& =\frac{2}{3} x^{\frac{3}{2}}\left(\ln ^{2} x-\frac{4}{3} \ln x+\frac{8}{9}\right)+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1794}
  \item \(\int x e^{-x} d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int x e^{-x} d x=-\int x d\left(e^{-x}\right)=-x e^{-x}+\int e^{\cdots x} d x \\
& =-e^{-x}(x+1)+C \text {. } \\
& \text { 1796. } \int x^{2} e^{-2 x} d x \text {. } \\
& m \int x^{2} e^{-2 x} d x=-\frac{1}{2} \int x^{2} d\left(e^{-2 x}\right) \\
& =-\frac{1}{2} x^{2} e^{-2 x}+\frac{1}{2} \int e^{-2 x} \cdot 2 x d x \\
& =-\frac{1}{2} x^{2} e^{-2 x}-\frac{1}{2} \int x d\left(e^{-2 x}\right) \\
& =-\frac{1}{2} x^{2} e^{-2 x}-\frac{1}{2} x e^{-2 x}+\frac{1}{2} \int e^{-2 x} d x \\
& =-\frac{1}{2} e^{-2 x}\left(x^{2}+x+\frac{1}{2}\right)+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1796}
  \item \(\int x^{3} e^{-x^{2}} d x\).
\end{enumerate}

\[
\begin{aligned}
& =-\frac{1}{2} x^{2} e^{-x^{2}}+\frac{1}{2} \int e^{-x^{2}} d\left(x^{2}\right)=-\frac{x^{2}+1}{2} e^{-x^{2}}+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1797}
  \item \(\int x \cos x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { A } f x \cos x d x=\int x d(\sin x) \\
& =x \sin x-\int \sin x d x=x \sin x+\cos x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1798}
  \item \(\int x^{2} \sin 2 x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 䏬 } \int x^{2} \sin 2 x d x=-\frac{1}{2} \int x^{2} d(\cos 2 x) \\
& =-\frac{1}{2} x^{2} \cos 2 x+\frac{1}{2} \int x d(\sin 2 x)
\end{aligned}
\]

\begin{center}
\includegraphics[max width=\textwidth]{2022_12_26_c19bf7cf4ca87c30c547g-050}
\end{center}

\[
\begin{aligned}
& =-\frac{1}{2} x^{2} \cos 2 x+\frac{1}{2} x \sin 2 x-\frac{1}{2} \int \sin 2 x d x \\
& =-\frac{2 x^{2}-1}{4} \cos 2 x+\frac{1}{2} x \sin 2 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1799}
  \item \(\int x \operatorname{sh} x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int x \operatorname{sh} x d x=\int x d(\operatorname{ch} x) \\
& =x \operatorname{ch} x-\int \operatorname{ch} x d x=x \operatorname{ch} x-\operatorname{sh} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1800}
  \item \(\int x^{3} \operatorname{ch} 3 x d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int x^{3} \operatorname{ch} 3 x d x=\frac{1}{3} \int x^{3} d(\operatorname{sh} 3 x) \\
= & \frac{1}{3} x^{3} \operatorname{sh} 3 x-\int x^{2} \operatorname{sh} 3 x d x \\
= & \frac{1}{3} x^{3} \operatorname{sh} 3 x-\frac{1}{3} \int x^{2} d(\operatorname{ch} 3 x) \\
= & \frac{1}{3} x^{3} \operatorname{sh} 3 x-\frac{1}{3} x^{2} \operatorname{ch} 3 x+\frac{2}{3} \int x \operatorname{ch} 3 x d x \\
= & \frac{1}{3} x^{3} \operatorname{sh} 3 x-\frac{1}{3} x^{2} \operatorname{ch} 3 x+\frac{2}{9} \int x d(\operatorname{sh} 3 x) \\
= & \frac{1}{3} x^{3} \operatorname{sh} 3 x-\frac{1}{3} x^{2} \operatorname{ch} 3 x+\frac{2}{9} x \operatorname{sh} 3 x-\frac{2}{9} \int \operatorname{sh} 3 x d x \\
= & \left(\frac{x^{3}}{3}+\frac{2 x}{9}\right) \operatorname{sh} 3 x-\left(\frac{x^{2}}{3}+\frac{2}{27}\right) \operatorname{ch} 3 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1801}
  \item \(\int \operatorname{arctg} x d x\).
\end{enumerate}

\[
\text { 旺 } \begin{aligned}
& \int \operatorname{arc} \operatorname{tg} x d x=x \operatorname{arctg} x-\int \frac{x}{1+x^{2}} d x \\
= & x \operatorname{arctg} x-\frac{1}{2} \ln \left(1+x^{2}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1802}
  \item \(\int \operatorname{arc} \sin x d x\).
\end{enumerate}

\[
\text { 牛 } \begin{aligned}
& \int \operatorname{arc} \sin x d x=x \arcsin x-\int \frac{x}{\sqrt{1-x^{2}}} d x \\
= & x \operatorname{arc} \sin x+\sqrt{1-x^{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1803}
  \item \(\int x \operatorname{arctg} x d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int x \operatorname{arctg} x d x=\frac{1}{2} \int \operatorname{arctg} x d\left(x^{2}\right) \\
= & \frac{1}{2} x^{2} \operatorname{arctg} x-\frac{1}{2} \int \frac{x^{2}}{1+x^{2}} d x \\
= & \frac{1}{2} x^{2} \operatorname{arctg} x-\frac{1}{2} \int\left(1-\frac{1}{1+x^{2}}\right) d x \\
= & \frac{1+x^{2}}{2} \operatorname{arctg} x-\frac{x}{2}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1804}
  \item \(\int x^{2} \operatorname{arc} \cos x d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int x^{2} \operatorname{arc} \cos x d x=\frac{1}{3} \int \operatorname{arc} \cos x d\left(x^{2}\right) \\
= & \frac{1}{3} x^{3} \operatorname{arc} \cos x+\frac{1}{3} \int \frac{x^{3}}{\sqrt{1-x^{2}}} d x \\
= & \frac{1}{3} x^{3} \operatorname{arc~cos} x-\frac{1}{6} \int \frac{x^{2}}{\sqrt{1-x^{2}}} d\left(1-x^{2}\right) \\
= & \frac{1}{3} x^{3} \operatorname{arc} \cos x-\frac{1}{6} \int\left(\frac{1}{\sqrt{1-x^{2}}}-\sqrt{1-x^{2}}\right) \\
& d\left(1-x^{2}\right) \\
= & \frac{1}{3} x^{3} \operatorname{arc} \cos x-\frac{1}{3} \sqrt{1-x^{2}}+\frac{1}{9}\left(1-x^{2}\right)^{\frac{3}{2}}+C \\
= & \frac{1}{3} x^{3} \operatorname{arc} \cos x-\frac{x^{2}+2}{9} \sqrt{1-x^{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1805}
  \item \(\int \frac{\arcsin x}{x^{2}} d x\).
\end{enumerate}

\[
\text { ज } \begin{aligned}
& \int \frac{\operatorname{arc} \sin x}{x^{2}} d x=-\int \arcsin x d\left(\frac{1}{x}\right) \\
= & -\frac{1}{x} \operatorname{arc} \sin x+\int \frac{d x}{x \sqrt{1-x^{2}}} .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}作代换\end{CJK} \(x=\sin t\), \begin{CJK}{UTF8}{mj}得\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{x \sqrt{1-x^{2}}}=\int \frac{\cos t d t}{\sin t \cos t}=\int \frac{d t}{\sin t} \\
= & \ln \left|\operatorname{tg} \frac{t}{2}\right|^{*}+C \\
= & \ln \left|\frac{\sin t}{1+\cos t}\right|+C=-\ln \left|\frac{1+\cos t}{\sin t}\right|+C \\
= & -\ln \left|\frac{1+\sqrt{1-x^{2}}}{x}\right|+C .
\end{aligned}
\]

\section{甶㕄捛得}
\[
\begin{aligned}
& \int \frac{\operatorname{arc} \sin x}{x^{2}} d x=-\frac{1}{x} \operatorname{arc~} \sin x \\
& -\ln \left|\frac{1+\sqrt{1-x^{2}}}{x}\right|+C .
\end{aligned}
\]

\section{*）利軸 1703 题的结㽚.}
\[
\text { 1807. } \begin{aligned}
\int & \ln \left(x+\sqrt{1+x^{2}}\right) d x \\
& \int \ln \left(x+\sqrt{1+x^{2}}\right) d x \\
= & x \ln \left(x+\sqrt{1+x^{2}}\right)-\int \frac{x}{\sqrt{1+x^{2}}} d x \\
= & x \ln \left(x+\sqrt{1+x^{2}}\right)-\sqrt{1+x^{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1807}
  \item \(\int x \ln \frac{1+x}{1-x} d x\)
\end{enumerate}

\[
\text { A } 9 x \ln \frac{1+x}{1-x} d x=\frac{1}{2} \int \ln \frac{1+x}{1-x} d\left(x^{2}\right)
\]

\[
\begin{aligned}
& =\frac{x^{2}}{2} \ln \frac{1+x}{1-x}-\int \frac{x^{2}}{1-x^{2}} d x \\
& =\frac{x^{2}}{2} \ln \frac{1+x}{1-x}+\int\left(1-\frac{1}{1-x^{2}}\right) d x \\
& =x-\frac{1-x^{2}}{2} \ln \frac{1+x}{1-x}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1808}
  \item \(\int \operatorname{arctg} \sqrt{x} d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 㙰 } \int \operatorname{arctg} \sqrt{x} d x=x \operatorname{arctg} \sqrt{x} \\
& -\frac{1}{2} \int \frac{x}{\sqrt{x}(1+x)} d x \\
& =x \operatorname{arctg} \sqrt{x}-\int\left(1-\frac{1}{1+x}\right) d(\sqrt{x}) \\
& =(x+1) \operatorname{arctg} \sqrt{x}-\sqrt{x}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1809}
  \item \(\int \sin x \cdot \ln (\operatorname{tg} x) d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \sin x \cdot \ln (\operatorname{tg} x) d x=-\int \ln (\operatorname{tg} x) d(\cos x) \\
&=-\cos x \cdot \ln (\operatorname{tg} x)+\int \cos x \cdot \operatorname{ctg} x \cdot \sec ^{2} x d x \\
&=-\cos x \cdot \ln (\operatorname{tg} x)+\int \frac{d x}{\sin x} \\
&=-\cos x \cdot \ln (\operatorname{tg} x)+\ln \left|\operatorname{tg} \frac{x}{2}\right|+C . \\
& \text { 求下列积分： }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1810}
  \item \(\int x^{5} e^{x 3} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int x^{5} e^{r^{3}} d x=\frac{1}{3} \int x^{3} d\left(e^{x^{3}}\right) \\
= & \frac{1}{3} x^{3} e^{r 3}-\frac{1}{3} \int e^{x^{3}} d\left(x^{3}\right)
\end{aligned}
\]

\[
=\frac{1}{3}\left(x^{3}-1\right) e^{x 3}+C .
\]

\begin{enumerate}
  \setcounter{enumi}{1811}
  \item \(\int(\arcsin x)^{2} d x\)
\end{enumerate}

\[
\text { AP } \begin{aligned}
& \int(\arcsin x)^{2} d x=x(\arcsin x)^{2}-2 \int \frac{x \operatorname{arc} \sin x}{\sqrt{1-x^{2}}} d x \\
= & x(\operatorname{arc} \sin x)^{2}+2 \int \arcsin x d\left(\sqrt{1-x^{2}}\right) \\
= & x(\arcsin x)^{2}+2 \sqrt{1-x^{2}} \operatorname{arc} \sin x-2 \int d x \\
= & x(\arcsin x)^{2}+2 \sqrt{1-x^{2}} \arcsin x-2 x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1812}
  \item \(\int x(\operatorname{arc} \operatorname{tg} x)^{2} d x\)
\end{enumerate}

\[
\begin{aligned}
& \int x(\operatorname{arctg} x)^{2} d x=\frac{1}{2} \int(\operatorname{arctg} x)^{2} d\left(x^{2}\right) \\
= & \frac{1}{2} x^{2}(\operatorname{arctg} x)^{2}-\int \frac{x^{2} \operatorname{arctg} x}{1+\frac{x^{2}}{1} d x} \\
= & \frac{x^{2}}{2}(\operatorname{arctg} x)^{2}-\int\left(1-\frac{1}{1+x^{2}}\right) \operatorname{arctg} x d x \\
= & \frac{x^{2}}{2}(\operatorname{arctg} x)^{2}-\int \operatorname{arctg} x d x \\
& +\int \operatorname{arctg} x d(\operatorname{arctg} x) \\
= & \frac{x^{2}}{2}(\operatorname{arctg} x)^{2}-x \operatorname{tarctg} x+\int \frac{x d x}{1+x^{2}} \\
& +\frac{1}{2}(\operatorname{arctg} x)^{2} \\
= & \frac{x^{2}+1}{2}(\operatorname{arctg} x)^{2}-x \operatorname{tarctg} x+\frac{1}{2} \ln \left(1+x^{2}\right) \\
& +C+
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{7813}
  \item \(\int x^{2} \ln \frac{1-x}{1+x} d x\).
\end{enumerate}

\[
\text { 怿 } \begin{aligned}
& \int x^{2} \ln \frac{1-x}{1+x} d x \\
= & \frac{1}{3} \int \ln \frac{1-x}{1+x} d\left(x^{3}\right) \\
= & \frac{1}{3} x^{3} \ln \frac{1-x}{1+x}+\frac{2}{3} \int \frac{x^{3}}{1-x^{2}} d x \\
= & \frac{x^{3}}{3} \ln \frac{1-x}{1+x}+\frac{2}{3} \int\left(-x+\frac{x}{1-x^{2}}\right) d x \\
= & \frac{x^{3}}{3} \ln \frac{1-x}{1+x}-\frac{1}{3} x^{2}-\frac{1}{3} \ln \left(1-x^{2}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1814}
  \item \(\int \frac{x \ln \left(x+\sqrt{1+x^{2}}\right)}{\sqrt{1+x^{2}}} d x\).
\end{enumerate}

\[
\text { 腈 } \begin{aligned}
& \int \frac{x \ln \left(x+\sqrt{1+x^{2}}\right)}{\sqrt{1+x^{2}}} d x \\
= & \int \ln \left(x+\sqrt{1+x^{2}}\right) d\left(\sqrt{1+x^{2}}\right) \\
= & \sqrt{1+x^{2}} \ln \left(x+\sqrt{1+x^{2}}\right) \\
& -\int \sqrt{1+x^{2}} \cdot \frac{1}{\sqrt{1+x^{2}}} d x \\
= & \sqrt{1+x^{2}} \ln \left(x+\sqrt{1+x^{2}}\right)-x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1815}
  \item \(\int \frac{x^{2}}{\left(1+x^{2}\right)^{2}} d x\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{x^{2}}{\left(1+x^{2}\right)^{2}} d x=\frac{1}{2} \int \frac{x}{\left(1+x^{2}\right)^{2}} d\left(1+x^{2}\right) \\
= & -\frac{1}{2} \int x d\left(\frac{1}{1+x^{2}}\right)=-\frac{x}{2\left(1+x^{2}\right)}+\frac{1}{2} \int \frac{d x}{1+x^{2}} \\
= & -\frac{x}{2\left(1+x^{2}\right)}+\frac{1}{2} \operatorname{arctg} x+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1816}
  \item \(\int \frac{d x}{\left(a^{2}+x^{2}\right)^{2}}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \text { 当 } a=0 \text { 时, } \\
& \int \frac{d x}{\left(a^{2}+x^{2}\right)^{2}}=\int \frac{d x}{x^{4}}=-\frac{1}{3 x^{3}}+C ; \\
& \text { 当 } a \neq 0 \text { 时, } \\
& \int \frac{d x}{\left(a^{2}+x^{2}\right)^{2}}=\frac{1}{a^{2}} \int \frac{\left(a^{2}+x^{2}\right)-x^{2}}{\left(a^{2}+x^{2}\right)^{2}} d x \\
= & \frac{1}{a^{2}} \int \frac{d x}{a^{2}+x^{2}}-\frac{1}{a^{2}} \int \frac{x^{2}}{\left(a^{2}+x^{2}\right)^{2}} d x \\
= & \left.\left.\frac{1}{a^{3}} \operatorname{arctg} \frac{x}{a}-\frac{1}{a^{3}} \int \frac{\left.\left(\frac{x}{a}\right)^{2} d\left(\frac{x}{a}\right)^{2}+\left(\frac{x}{a}\right)^{2}\right]^{2}}{\left(1+\frac{x}{a}\right.}\right]^{\prime \prime}+\frac{1}{2} \operatorname{arctg} \frac{x}{a}\right]^{\prime}+C \\
= & \frac{1}{a^{3}} \operatorname{arctg} \frac{x}{a} \\
= & \frac{1}{2 a^{3}} \operatorname{arctg} \frac{x}{a}+\frac{x}{2 a^{2}\left(a^{2}+x^{2}\right)}+C .
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1816 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1817}
  \item \(\int \sqrt{a^{2}-x^{2}} d x\).
\end{enumerate}

\[
\text { 鈃 } \begin{aligned}
& \int \sqrt{a^{2}-x^{2}} d x=x \sqrt{a^{2}-x^{2}}+\int \frac{x^{2}}{\sqrt{a^{2}-x^{2}}} d x \\
= & x \sqrt{a^{2}-x^{2}}+\int \frac{a^{2}-\left(a^{2}-x^{2}\right)}{\sqrt{a^{2}-x^{2}}} d x \\
= & x \sqrt{a^{2}-x^{2}}+a^{2} \arcsin \frac{x}{|a|} \\
& -\int \sqrt{a^{2}-x^{2}} d x,
\end{aligned}
\]

\[
\begin{aligned}
= & \frac{3}{4}\left[\frac{1}{3} x\left(a^{2}+x^{2}\right) \sqrt{a^{2}+x^{2}}-\frac{a^{2}}{3} \int \sqrt{a^{2}+x^{2}} d x\right] \\
= & \frac{1}{4} x\left(a^{2}+x^{2}\right) \sqrt{a^{2}+x^{2}} \\
& -\frac{a^{2}}{4}\left[\frac{x}{2} \sqrt{a^{2}+x^{2}}+\frac{a^{2}}{2} \ln \left(x+\sqrt{a^{2}+x^{2}}\right)\right]^{" \prime}+C \\
= & \frac{x\left(2 x^{2}+a^{2}\right)}{8} \sqrt{a^{2}+x^{2}} \\
& -\frac{a^{4}}{8} \ln \left(x+\sqrt{x^{2}+a^{2}}\right)+C .
\end{aligned}
\]

\[
\begin{aligned}
& \text { *) 利用 } 1786 \text { 题的狜果. } \\
& \int x \sin ^{2} x d x \\
& \text { 的 } \int x \sin ^{2} x d x=\frac{1}{2} \int x(1-\cos 2 x) d x \\
&= \frac{1}{2} \int x d x-\frac{1}{2} \int x \cos 2 x d x \\
&= \frac{1}{4} x^{2}-\frac{1}{4} \int x d(\sin 2 x) \\
&= \frac{1}{4} x^{2}-\frac{1}{4} x \sin 2 x+\frac{1}{4} \int \sin 2 x d x \\
&= \frac{1}{4} x^{2}-\frac{x}{4} \sin 2 x-\frac{1}{8} \cos 2 x+C .
\end{aligned}
\]

1822* \(\int e^{\sqrt{s}} d x\).

A \begin{CJK}{UTF8}{mj}设\end{CJK} \(\sqrt{x}=t\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x=t^{2}, d x=2 t d t\), \begin{CJK}{UTF8}{mj}代\end{CJK} \(人\) \begin{CJK}{UTF8}{mj}得\end{CJK}

\[
\begin{aligned}
& \int e^{\sqrt{x}} d x=2 \int t e^{t} d t=2 \int t d\left(e^{t}\right) \\
= & 2 t e^{t}-2 \int e^{t} d t \\
= & 2 t e^{t}-2 e^{t}+C=2(\sqrt{x}-1) e^{\sqrt{x}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1822}
  \item \(\int x \sin \sqrt{x} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \text { 设 } \sqrt{x}=t \text {, 则 } x=t^{2}, d x=2 t d t \text {, 代入得 } \\
& \int x \sin \sqrt{x} d x=2 \int t^{3} \sin t d t=-2 \int t^{3} d(\cos t) \\
= & -2 t^{3} \cos t+6 \int t^{2} \cos t d t \\
= & -2 t^{3} \cos t+6 \int t^{2} d(\sin t) \\
= & -2 t^{3} \cos t+6 t^{2} \sin t-12 \int t \sin t d t \\
= & -2 t^{3} \cos t+6 t^{2} \sin t+12 \int t d(\cos t) \\
= & -2 t^{3} \cos t+6 t^{2} \sin t+12 t \cos t-12 \int \cos t d t \\
= & -2\left(t^{2}-6\right) t \cos t+6\left(t^{2}-2\right) \sin t+C \\
= & 2(6-x) \sqrt{x} \cos \sqrt{x}-6(2-x) \sin \sqrt{x}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1823}
  \item \(\int \frac{x e^{\text {arcclgr }}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int \frac{x e^{\operatorname{arctgr}}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x=\int \frac{x}{\sqrt{1+}+x^{2}} d\left(e^{\operatorname{arccg} x}\right) \\
& =\frac{x}{\sqrt{1+x^{2}}} e^{\operatorname{arctax}}-\int e^{\operatorname{arclg} x} \cdot \frac{1}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x \\
& =\frac{x}{\sqrt{1+x^{2}}} e^{\operatorname{arctg} x}-\int \frac{1}{\sqrt{1+x^{2}}} d\left(e^{\operatorname{arctg} x}\right) \\
& =\frac{x-1}{\sqrt{1+x^{2}}} e^{\text {arelgt }}-\int \frac{x e^{\text {sccles }}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x \text {. } \\
& \text { 于是得 } \\
& \int \frac{x e^{\text {Arstg }}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x=\frac{x-1}{2 \sqrt{1+x^{2}}} e^{\text {arclg } x}+C \text {. } 
\end{aligned}
\]

\[
\begin{aligned}
& \text { 1825. } \int \frac{e^{\text {artug } x}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x \text {. } \\
& \text { 解 } \int \frac{e^{\operatorname{arctg} r}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x=\int \frac{1}{\sqrt{1+x^{2}}} d\left(e^{\operatorname{acctg} r}\right) \\
& =\frac{1}{\sqrt{1+x^{2}}} e^{\operatorname{arctag} x}+\int \frac{x e^{\operatorname{arclg} r}}{\left(1+x^{2}\right)^{\frac{3}{2}}} d x \\
& =\frac{1}{\sqrt{1+x^{2}}} e^{\text {ancent }}+\frac{x-1}{2 \sqrt{1+x^{2}}} e^{\operatorname{arctgr}^{2)}}+C \\
& =\frac{x+1}{2} \frac{\sqrt{1+x^{2}}}{\text { ancegr }}+C \text {. }
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1824 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1825}
  \item \(\int \sin (\ln x) d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int \sin (\ln x) d x=x \sin (\ln x)-\int x \cos (\ln x) \cdot \frac{1}{x} d x \\
& =x \sin (\ln x)-x \cos (\ln x)-\int \sin (\ln x) d x,
\end{aligned}
\]

\section{于是得}
\[
\int \sin (\ln x) d x=\frac{x}{2}[\sin (\ln x)-\cos (\ln x)]+C .
\]

\begin{enumerate}
  \setcounter{enumi}{1826}
  \item \(\int \cos (\ln x) d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 觟 } \int \cos (\ln x) d x=x \cos (\ln x)+\int \sin (\ln x) d x \\
& =x \cos (\ln x)+\frac{x}{2}[\sin (\ln x)-\cos (\ln x))+C \\
& =\frac{x}{2}[\sin (\ln x)+\cos (\ln x)]+C .
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1826 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1827}
  \item \(\int e^{a x} \cos b x d x\).
\end{enumerate}

\[
\text { 觟 } \begin{aligned}
& \text { 如果 } a, b \text { 同时为零,积分显然为 } x+C \text {; 若 } a=0, \\
b \neq & 0 \text {,积分显然为 } \frac{1}{b} \sin b x+C ; \text { 以 下设 } a \neq 0 ; \\
& \int e^{u x} \cos b x d x=\frac{1}{a} \int \cos b x d\left(e^{u r}\right) \\
= & \frac{1}{a} e^{a x} \cos b x+\frac{b}{a} \int e^{u s} \sin b x d x \\
= & \frac{1}{a} e^{u r} \cos b x+\frac{b}{a^{2}} \int \sin b x d\left(e^{a r s}\right. \\
= & \frac{1}{a} e^{u r} \cos b x+\frac{b}{a^{2}} e^{a x} \sin b x-\frac{b^{2}}{a^{2}} \int e^{a x} \cos b x d x
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}于是得\end{CJK}

\[
\begin{aligned}
& \int e^{a x} \cos b x d x=\frac{a^{2}}{a^{2}+b^{2}}\left[\frac{1}{a} e^{a r} \cos b x+\frac{b}{a^{2}} e^{a r} \sin b x\right] \\
& +C=\frac{e^{a x}(a \cos b x+b \sin b x)}{a^{2}+b^{2}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1828}
  \item \(\int e^{a x} \sin b x d x\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}觔\end{CJK} . \begin{CJK}{UTF8}{mj}若\end{CJK} \(a=b=0\), \begin{CJK}{UTF8}{mj}则积分为\end{CJK} \(x+C\); \begin{CJK}{UTF8}{mj}以下设\end{CJK} \(a^{2}+b^{2}\) \(\neq 0\), \begin{CJK}{UTF8}{mj}则有\end{CJK}

\[
\begin{aligned}
& \int e^{u x} \sin b x d x=\frac{1}{a} \int \sin b x d\left(e^{u r}\right) \\
= & \frac{1}{a} e^{a r} \sin b x-\frac{b}{a} \int e^{a x} \cos b x d x \\
= & \frac{1}{a} e^{a x} \sin b x-\frac{b}{a^{2}} \int \cos b x d e^{a x} \\
= & \frac{1}{a} e^{a r} \sin b x-\frac{b}{a^{2}} e^{a x} \cos b x-\frac{b^{2}}{a^{2}} \int e^{a x x} \sin b x d x,
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}故\end{CJK} \(\int e^{a x} \sin b x d x=\frac{e^{a x}(a \sin b x-b \cos b x)}{a^{2}+b^{2}}+C\).

\begin{enumerate}
  \setcounter{enumi}{1829}
  \item \(\int e^{2 x} \sin ^{2} x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int e^{2 x} \sin ^{2} x d x=\frac{1}{2} \int e^{2 x}(1-\cos 2 x) d x \\
& =\frac{1}{2} \int e^{2 x} d x-\frac{1}{2} \int e^{2 r} \cos 2 x d x \\
& =\frac{1}{4} e^{2 x}-\frac{1}{2}\left(\frac{2 \cos 2 x+2 \sin 2 x}{8} e^{2 x}\right)^{\prime \prime}+C \\
& =\frac{1}{8} e^{2}(2-\cos 2 x-\sin 2 x)+C . \\
& \text { *) 利用 } 1828 \text { 题的结果. } \\
& \text { 1831. } \int\left(e^{x}-\cos x\right)^{2} d x \text {. } \\
& \text { 解 } \int\left(e^{2}-\cos x\right)^{2} d x=\int\left(e^{2 x}-2 e^{x} \cos x+\cos ^{2} x\right) d x \\
& =\frac{1}{2} e^{i x}-2 \cdot \frac{e^{x}(\cos x+\sin x)^{* \prime}}{2}+ \\
& \left(\frac{x}{2}+\frac{1}{4} \sin 2 x\right)+C \\
& =\frac{1}{2} e^{z^{x}}-e^{x}(\cos x+\sin x)+\frac{x}{2}+\frac{1}{4} \sin 2 x+c . \\
& \text { *) 利用 } 1828 \text { 题的结果. } \\
& \text { **) 利用 } 1742 \text { 题的狜果. } \\
& \text { 1832. } \int \frac{\operatorname{arcctg} e^{x}}{e^{1}} d x \text {. } \\
& \text { An } \int \frac{\operatorname{arcctg} e^{x}}{e^{x}} d x=-\int \operatorname{arcctg} e^{x} d\left(e^{-x}\right) \\
& =-e^{-x} \cdot \operatorname{arcctg}\left(e^{x}\right)-\int \frac{d x}{1+e^{2 r}} \\
& \left.=-e^{-x} \operatorname{arcctg}\left(e^{x}\right)-\frac{1}{2}\left[2 x-\ln \left(1+e^{2 x}\right)\right]^{*}\right)+C \text {. } \\
& =-e^{-x} \operatorname{arctg}\left(e^{r}\right)-x+\frac{1}{2} \ln \left(1+e^{2 r}\right)+C .
\end{aligned}
\]

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1759 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\[
\text { 1833. } \begin{aligned}
& \int \frac{\ln (\sin x)}{\sin ^{2} x} d x . \\
& \text { 解 } \int \frac{\ln (\sin x)}{\sin ^{2} x} d x=-\int \ln (\sin x) d(\operatorname{ctg} x) \\
&=-\operatorname{ctg} x+\ln (\sin x)+\int \operatorname{ctg}^{2} x d x \\
&=-\operatorname{ctg} x \cdot \ln (\sin x)+(-\operatorname{ctg} x-x)^{*}+C \\
&=-[x+\operatorname{ctg} x \cdot \ln (e \sin x)]+C . \\
&*) \quad \text { 利用 } 1649 \text { 题或 } 1751 \text { 题的结果. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1833}
  \item \(\int \frac{x d x}{\cos ^{2} x}\)
\end{enumerate}

\[
\begin{aligned}
& \text { 解 } \int \frac{x d x}{\cos ^{2} x}=\int x d(\operatorname{tg} x)=x \operatorname{tg} x-\int \operatorname{tg} x d x \\
& =x \operatorname{tg} x+\ln |\cos x|+C . \\
& \text { *) 利用 } 1697 \text { 题的结果. }
\end{aligned}
\]

\[
\text { 1835. } \begin{aligned}
& \int \frac{x e^{x}}{(x+1)^{2}} d x . \\
& \quad \int \frac{x e^{x}}{(x+1)^{2}} d x=-\int x e^{x} d\left(\frac{1}{1+x}\right) \\
&=-\frac{x}{1+x} e^{x}+\int-\frac{1}{1+x} e^{x}(x+1) d x \\
&=-\frac{x}{1+x} e^{x}+e^{x}+C=\frac{e^{x}}{1+x}+C .
\end{aligned}
\]

\section{下列积分的求法需要把二次三项式化成正则型,并利}
\begin{CJK}{UTF8}{mj}用下列公式\end{CJK}:

I. \(\int \frac{d x}{a^{2}+x^{2}}=\frac{1}{a} \operatorname{arctg} \frac{x}{a}+C \quad(a \neq 0)\);

I. \(\int \frac{d x}{a^{2} \cdots x^{2}}=\frac{1}{2 a} \ln \left|\frac{a+x}{a-x}\right|+C \quad(a \neq 0)\);

I. \(\int \frac{x d x}{a^{2} \pm x^{2}}=\pm \frac{1}{2} \ln \left|a^{2} \pm x^{2}\right|+C\);

\[
\begin{aligned}
& \text { N. } \int \frac{d x}{\sqrt{a^{2}-x^{2}}}=\arcsin \frac{x}{a}+C \quad(a>0) \text {; } \\
& \mathrm{V} \cdot \int \frac{d x}{\sqrt{x^{2}} \pm a^{2}}=\ln \left|x+\sqrt{x^{2} \pm a^{2}}\right|+C \text {; } \\
& \text { V. } \int \frac{x d x}{\sqrt{a^{2} \pm x^{2}}}=\pm \sqrt{a^{2} \pm x^{2}}+C ; \\
& \text { VI . } \int \sqrt{a^{2}-x^{2}} d x \\
& =\frac{x}{2} \sqrt{a^{2}-x^{2}}+\frac{a^{2}}{2} \arcsin \frac{x}{a}+C \quad(a>0) \\
& \text { VI } \iint \sqrt{x^{2} \pm a^{2}} d x \\
& =\frac{x}{2} \sqrt{x^{2} \pm a^{2}} \pm \frac{a^{2}}{2} \ln \left|x+\sqrt{x^{2} \pm a^{2}}\right|+C \text {. }
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}求下列稆击\end{CJK}：

\[
\begin{aligned}
1836^{+} \cdot & \int \frac{d x}{a+b x^{2}} \quad(a b \neq 0) \\
& \quad \frac{\text { 当 }}{a b}>0 \text { 时, } \\
& \int \frac{d x}{a+b x^{2}} \\
& =\operatorname{sgna} \cdot \frac{1}{\sqrt{|b|}} \int \frac{d(\sqrt{|b|} x)}{(\sqrt{|a|})^{2}+(\sqrt{|b|} x)^{2}} \\
& =\operatorname{sgn} a \cdot \frac{1}{\sqrt{a b}} \operatorname{atctg}\left[x \sqrt{\frac{b}{a}}\right)+C
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}当\end{CJK} \(a b<0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{d x}{a+b x^{2}}=\operatorname{sgn} a \cdot \int \frac{d x}{|a|-|b| x^{2}} \\
= & \operatorname{sgn} a \cdot \frac{1}{\sqrt{|b|}} \int \frac{d(\sqrt{|b|} x)}{(\sqrt{|a|})^{2}-(\sqrt{|b|} x)^{2}} .
\end{aligned}
\]

\[
=\frac{\operatorname{sgn} a}{2 \sqrt{-a b}} \ln \left|\frac{\sqrt{|a|}+x \sqrt{|b|}}{\sqrt{|a|}-x \sqrt{|b|}}\right|+C .
\]

\begin{enumerate}
  \setcounter{enumi}{1836}
  \item \(\int \frac{d x}{x^{2}-x+2}\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{d x}{x^{2}-x+2}=\int \frac{d\left(x-\frac{1}{2}\right)}{\left(x-\frac{1}{2}\right)^{2}+\left(\frac{\sqrt{7}}{2}\right)^{2}} \\
= & \frac{2}{\sqrt{7}} \operatorname{arctg} \frac{2 x-1}{\sqrt{7}}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1837}
  \item \(\int \frac{d x}{3 x^{2}-2 x-1}\).
\end{enumerate}

\[
\text { n7 } \int \frac{d x}{3 x^{2}-2 x-1}=\frac{1}{3} \int \frac{d x}{x^{2}-\frac{2}{3} x-\frac{1}{3}}
\]

\[
\begin{aligned}
& =\frac{1}{3} \int \frac{d\left(x-\frac{1}{3}\right)}{\left(x-\frac{1}{3}\right)^{2}-\left(\frac{2}{3}\right)^{2}} \\
& =-\frac{1}{3} \cdot \frac{3}{4} \ln \left|\frac{\frac{2}{3}+\left(x-\frac{1}{3}\right)}{\frac{2}{3}-\left(x-\frac{1}{3}\right)}\right|+C_{1} \\
& =\frac{1}{4} \ln \left|\frac{x-1}{3 x+1}\right|+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1838}
  \item \(\int \frac{x d x}{x^{4}-2 x^{2}-1}\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{x d x}{x^{4}-2 x^{2}-1}=\frac{1}{2} \int \frac{d\left(x^{2}-1\right)}{\left(x^{2}-1\right)^{2}-(\sqrt{2})^{2}} \\
= & \frac{1}{4 \sqrt{2}} \ln \left|\frac{x^{2}-(\sqrt{2}+1)}{x^{2}+(\sqrt{2}-1)}\right|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1839}
  \item \(\int \frac{x+1}{x^{2}+x+1} d x\).
\end{enumerate}

\[
\text { 觞 } \begin{aligned}
& \int \frac{x+1}{x^{2}+x+1} d x=\int \frac{\frac{1}{2}(2 x+1)+\frac{1}{2}}{x^{2}+x+1} d x \\
= & \frac{1}{2} \int \frac{2 x+1}{x^{2}+x+1} d x+\frac{1}{2} \int \frac{d\left(x+\frac{1}{2}\right)}{\left(x+\frac{1}{2}\right)^{2}+\left(\frac{\sqrt{3}}{2}\right)^{2}} \\
= & \frac{1}{2} \ln \left(x^{2}+x+1\right)+\frac{1}{\sqrt{3}} \operatorname{arctg}\left(\frac{2 x+1}{\sqrt{3}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1840}
  \item \(\int \frac{x d x}{x^{2}-2 x \cos \alpha+1}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x d x}{x^{2}-2 x \cos \alpha+1}=\int \frac{x-\cos \alpha+\cos \alpha}{(x-\cos \alpha)^{2}+\sin ^{2} \alpha} d x \\
= & \frac{1}{2} \int \frac{d\left[(x-\cos \alpha)^{2}+\sin ^{2} \alpha\right]}{(x-\cos \alpha)^{2}+\sin ^{2} \alpha} \\
& +\cos \alpha \cdot \int \frac{d(x-\cos \alpha)}{(x-\cos \alpha)^{2}+\sin ^{2} \alpha} \\
= & \frac{1}{2} \ln \left(x^{2}-2 x \cos \alpha+1\right) \\
& +\operatorname{ctg} \alpha \cdot \operatorname{arctg}\left(\frac{x-\cos \alpha}{\sin \alpha}\right)+C \\
& (a \neq k \pi, k=0, \pm 1, \pm 2, \cdots) .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1841}
  \item \(\int \frac{x^{3} d x}{x^{4}-x^{2}+2}\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{x^{3} d x}{x^{4}-x^{2}+2} \\
= & \frac{1}{2} \int \frac{x^{2} d\left(x^{2}\right)}{\left(x^{2}-\frac{1}{2}\right)^{2}+\frac{7}{4}}
\end{aligned}
\]

\[
\begin{aligned}
= & \frac{1}{6} \ln \left|x^{6}-x^{3}-2\right| \\
& -\frac{1}{18} \ln \left|\frac{\frac{3}{2}+\left(x^{3}-\frac{1}{2}\right)}{\frac{3}{2}-\left(x^{3}-\frac{1}{2}\right)}\right|+C \\
= & \frac{1}{9} \ln \left\{\left|x^{3}+1\right| \cdot\left(x^{3}-2\right)^{2}\right\}+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}如果本题不化成正则型来作\end{CJK},\begin{CJK}{UTF8}{mj}则有更简单的作法\end{CJK},\begin{CJK}{UTF8}{mj}事英\end{CJK} \begin{CJK}{UTF8}{mj}上\end{CJK}.

\[
\begin{aligned}
& \int \frac{x^{5} d x}{x^{6}-x^{3}-2}=\frac{1}{3} \int \frac{x^{3} d\left(x^{3}\right)}{\left(x^{3}-2\right)\left(x^{3}+1\right)} \\
= & \frac{1}{9} \int\left(\frac{2}{x^{3}-2}+\frac{1}{x^{3}+1}\right) d\left(x^{3}\right) \\
= & \frac{1}{9} \ln \left\{\left|x^{3}+1\right| \cdot\left(x^{3}-2\right)^{2}\right\}+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1843}
  \item \(\int \frac{d x}{3 \sin ^{2} x-8 \sin x \cos x+5 \cos ^{2} x}\).
\end{enumerate}

\[
\text { At } \begin{aligned}
& \int \frac{d x}{3 \sin ^{2} x-8 \sin x \cos x+5 \cos ^{2} x} \\
= & \int \frac{d(\operatorname{tg} x)}{3 \operatorname{tg}^{2} x-8 \operatorname{tg} x+5} \\
= & \frac{1}{3} \int \frac{d\left(\operatorname{tg} x-\frac{4}{3}\right)}{\left(\operatorname{tg} x-\frac{4}{3}\right)^{2}-\left(\frac{1}{3}\right)^{2}} \\
= & \frac{1}{2} \ln \left|\frac{\frac{1}{3}-\left(\operatorname{tg} x-\frac{4}{3}\right)}{\frac{1}{3}+\left(\operatorname{tg} x-\frac{4}{3}\right)}\right|+C_{1} \\
= & \frac{1}{2} \ln \left|\frac{3 \sin x-5 \cos x}{\sin x-\cos x}\right|+C .
\end{aligned}
\]

\[
\text { 1845. } \begin{aligned}
& \int \frac{d x}{\sin x+2 \cos x+3} \cdot \\
& \text { 解 } \int \frac{d x}{\sin x+2 \cos x+3}=\int \frac{\frac{1}{\cos ^{2} \frac{x}{2}} d x}{2 \operatorname{tg} \frac{x}{2}+4+\sec ^{2} \frac{x}{2}} \\
& =2 \int \frac{d\left(\operatorname{tg} \frac{x}{2}\right)}{\left(\operatorname{tg} \frac{x}{2}+1\right)^{2}+4}=\operatorname{arctg}\left[\frac{\operatorname{tg} \frac{x}{2}+1}{2}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1845}
  \item \(\int \frac{d x}{\sqrt{a+b x^{2}}}(b \neq 0)\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}般\end{CJK} \begin{CJK}{UTF8}{mj}当\end{CJK} \(b>0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\int \frac{d x}{\sqrt{a+b x^{2}}}=\frac{1}{\sqrt{b}} \ln \left|x \sqrt{b}+\sqrt{a+b x^{2}}\right|+C ;
\]

\begin{CJK}{UTF8}{mj}当\end{CJK} \(a>0\) \begin{CJK}{UTF8}{mj}及\end{CJK} \(b<0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{a+b x^{2}}}=\frac{1}{\sqrt{-b}} \int \frac{d(\sqrt{-b} x)}{\sqrt{(\sqrt{a})^{2}-(\sqrt{-b x})^{2}}} \\
= & \frac{1}{\sqrt{-b}} \operatorname{arc} \sin \left(x \sqrt{-\frac{b}{a}}\right)+c .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1846}
  \item \(\int \frac{d x}{\sqrt{1-2 x-x^{2}}}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{d x}{\sqrt{1-2 x-x^{2}}}=\int \frac{d(x+1)}{\sqrt{2-(x+1)^{2}}} \\
= & \arcsin \left(\frac{x+1}{\sqrt{2}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1847}
  \item \(\int \frac{d x}{\sqrt{x+x^{2}}}\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{d x}{\sqrt{x+x^{2}}}=\int \frac{\left.d \mid x+\frac{1}{2}\right)}{\sqrt{\left(x+\frac{1}{2}\right)^{2}-\frac{1}{4}}} \\
= & \ln \left|x+\frac{1}{2}+\sqrt{x+x^{2}}\right|+c .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}本题即\end{CJK} 1687 \begin{CJK}{UTF8}{mj}题\end{CJK},\begin{CJK}{UTF8}{mj}注意不同的解法及不同形式的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1848}
  \item \(\int \frac{d x}{\sqrt{2 x^{2}-x+2}}\).
\end{enumerate}

\[
\begin{aligned}
& \text { 㸷 } \int \frac{d x}{\sqrt{2 x^{2}-x+2}}=\frac{1}{\sqrt{2}} \int \frac{d\left(x-\frac{1}{4}\right)}{\sqrt{\left(x-\frac{1}{4}\right)^{2}+\frac{15}{16}}} \\
& =\frac{1}{\sqrt{2}} \ln \left(x-\frac{1}{4}+\sqrt{x^{2}-\frac{x}{2}+1}\right)+C \text {. }
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1849}
  \item \begin{CJK}{UTF8}{mj}证明\end{CJK}: \begin{CJK}{UTF8}{mj}若\end{CJK}
\end{enumerate}

\[
y=a x^{2}+b x+c(a \neq 0),
\]

\begin{CJK}{UTF8}{mj}则当\end{CJK} \(a>0\) \begin{CJK}{UTF8}{mj}时\end{CJK} \(+\int \frac{d x}{\sqrt{y}}=\frac{1}{\sqrt{a}} \ln \left|\frac{y^{\prime}}{2}+\sqrt{a y}\right|+C\);

\begin{CJK}{UTF8}{mj}当\end{CJK} \(a<0\) \begin{CJK}{UTF8}{mj}时\end{CJK}, \(\int \frac{d x}{\sqrt{y}}=\frac{1}{\sqrt{-a}} \operatorname{arc} \sin \frac{-y^{\prime}}{\sqrt{b^{2}-4 a c}}+C\).

\begin{CJK}{UTF8}{mj}证\end{CJK} \begin{CJK}{UTF8}{mj}当\end{CJK} \(a>0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{y}}=\frac{1}{\sqrt{a}} \int \frac{d x}{\sqrt{x^{2}+\frac{b}{a} x+\frac{c}{a}}} \\
= & \frac{1}{\sqrt{a}} \int \frac{d\left(x+\frac{b}{2 a}\right)}{\sqrt{\left(x+\frac{b}{2 a}\right)^{2}+\frac{4 a c-b^{2}}{4 a^{2}}}}
\end{aligned}
\]

72

\[
\begin{aligned}
& =-\frac{1}{\sqrt{a}} \ln \left|x+\frac{b}{2 a}+\sqrt{x^{2}+\frac{b}{a} x+\frac{c}{a}}\right|+C \\
& =\frac{1}{\sqrt{a}} \ln \left|\frac{y^{\prime}}{2}+\sqrt{a y}\right|+C ;
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}当\end{CJK} \(a<0\) \begin{CJK}{UTF8}{mj}时\end{CJK}.

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{y}}=\frac{1}{\sqrt{-a}} \int \frac{d x}{\sqrt{-x^{2}-\frac{b}{a} x-\frac{c}{a}}} \\
= & \frac{1}{\sqrt{-a}} \int \frac{d\left(x+\frac{b}{2 a}\right)}{\sqrt{\frac{b^{2}-4 a c}{4 a^{2}}-\left(x+\frac{b}{2 a}\right)^{2}}} \\
= & \frac{1}{\sqrt{-a}} \arcsin \frac{x+\frac{b}{2 a}}{\frac{\sqrt{b^{2}-4 a c}}{-2 a}}+C \\
= & \frac{1}{\sqrt{-a}} \operatorname{arc} \sin \left(\frac{-y^{\prime}}{\sqrt{b^{2}-4 a c}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1850}
  \item \(\int \frac{x d x}{\sqrt{5+x-x^{2}}}\).
\end{enumerate}

\[
\text { 捔 } \begin{aligned}
& \int \frac{x d x}{\sqrt{5+x-x^{2}}}=\int \frac{\left(x-\frac{1}{2}\right)+\frac{1}{2}}{\sqrt{\frac{21}{4}-\left(x-\frac{1}{2}\right)^{2}}} d x \\
= & -\frac{1}{2} \int \frac{d\left(\frac{21}{4}-\left(x-\frac{1}{2}\right)^{2}\right)}{\sqrt{\frac{21}{4}-\left(x-\frac{1}{2}\right)^{2}}}
\end{aligned}
\]

\[
\begin{aligned}
& +\frac{1}{2} \int \frac{d\left(x-\frac{1}{2}\right)}{\sqrt{\frac{21}{4}-\left(x-\frac{1}{2}\right)^{2}}} \\
& =-\sqrt{5+x-x^{2}}+\frac{1}{2} \arcsin \left(\frac{2 x-1}{\sqrt{21}}\right)+C \text {. } \\
& \text { 1852. } \int \frac{x+1}{\sqrt{x^{2}+x+1}} d x \text {. } \\
& \text { \{ } \int \frac{x+1}{\sqrt{x^{2}+x+1}} d x=\int \frac{\left(x+\frac{1}{2}\right)+\frac{1}{2}}{\sqrt{\left(x+\frac{1}{2}\right)^{2}+\frac{3}{4}}} d x \\
& =\frac{1}{2} \int \frac{d\left(\left(x+\frac{1}{2}\right)^{2}+\frac{3}{4}\right)}{\sqrt{\left(x+\frac{1}{2}\right)^{2}+\frac{3}{4}}}+\frac{1}{2} \int \frac{d\left(x+\frac{1}{2}\right)}{\sqrt{\left(x+\frac{1}{2}\right)^{2}+\frac{3}{4}}} \\
& =\sqrt{x^{2}+x+1}+\frac{1}{2} \ln \left(x+\frac{1}{2}+\sqrt{x^{2}+x+1}\right) \\
& +C \text {. } \\
& \text { 1853. } \int \frac{x d x}{\sqrt{1-3 x^{2}-2 x^{4}}} \text {. } \\
& \text { A } \int \frac{x d x}{\sqrt{1-3 x^{2}-2 x^{4}}} \\
& =\frac{1}{2 \sqrt{2}} \int \frac{d\left(x^{2}+\frac{3}{4}\right)}{\sqrt{\frac{17}{16}-\left(x^{2}+\frac{3}{4}\right)^{2}}} \\
& =\frac{1}{2 \sqrt{2}} \arcsin \left(\frac{4 x^{2}+3}{\sqrt{17}}\right)+C \text {. } 
\end{aligned}
\]

\[
\text { 1854. } \begin{aligned}
\int & \frac{x^{3} d x}{\sqrt{x^{4}-2 x^{2}-1}} . \\
\text { 解 } & \int \frac{x^{3} d x}{\sqrt{x^{4}-2 x^{2}-1}}=\frac{1}{2} \int \frac{x^{2} d\left(x^{2}\right)}{\sqrt{\left(x^{2}-1\right)^{2}-2}} \\
= & \frac{1}{2} \int \frac{\left(x^{2}-1\right) d\left(x^{2}-1\right)}{\sqrt{\left(x^{2}-1\right)^{2}-2}}+\frac{1}{2} \int \frac{d\left(x^{2}-1\right)}{\sqrt{\left(x^{2}-1\right)^{2}-2}} \\
= & \frac{1}{2} \sqrt{x^{4}-2 x^{2}-1} \\
& +\frac{1}{2} \ln \left|x^{2}-1+\sqrt{x^{4}-2 x^{2}-1}\right|+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1854}
  \item \(\int \frac{x+x^{3}}{\sqrt{1+x^{2}-x^{4}}} d x\).
\end{enumerate}

\[
\text { 解 } \begin{aligned}
& \int \frac{x+x^{3}}{\sqrt{1+x^{2}-x^{4}}} d x=\frac{1}{2} \int \frac{\left(1+x^{2}\right) d\left(x^{2}\right)}{\sqrt{\frac{5}{4}-\left(x^{2}-\frac{1}{2}\right)^{2}}} \\
= & \frac{1}{2} \int \frac{\left(x^{2}-\frac{1}{2}\right) d\left(x^{2}-\frac{1}{2}\right)}{\sqrt{\frac{5}{4}-\left(x^{2}-\frac{1}{2}\right)^{2}}} \\
& +\frac{3}{4} \int \frac{d\left(x^{2}-\frac{1}{2}\right)}{\sqrt{\frac{5}{4}-\left(x^{2}-\frac{1}{2}\right)^{2}}} \\
= & -\frac{1}{2} \sqrt{1+x^{2}-x^{4}}+\frac{3}{4} \arcsin \left(\frac{2 x^{2}-1}{\sqrt{5}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1855}
  \item \(\int \frac{d x}{x \sqrt{x^{2}+x+1}}\).
\end{enumerate}

m \begin{CJK}{UTF8}{mj}作代换\end{CJK} \(\ell=\frac{1}{x}\), \begin{CJK}{UTF8}{mj}则\end{CJK}

\[
\begin{aligned}
& x \sqrt{x^{2}+x+1}=\frac{\operatorname{sgn} t}{t^{2}} \sqrt{t^{2}+t+1}, d x=-\frac{d t}{t^{2}} \text {. 于是 } \\
& \int \frac{d x}{x \sqrt{x^{2}+x+1}}=-(\operatorname{sgn} t) \int \frac{d t}{\sqrt{t^{2}+t+1}} \\
& =-(\operatorname{sgn} t) \ln \left|t+\frac{1}{2}+\sqrt{t^{2}+t+1}\right|^{\cdot \prime}+C_{1} \\
& =-(\operatorname{sgn} x) \ln \left|\frac{x+2+2(\operatorname{sgn} x) \sqrt{x^{2}+x+1}}{2 x}\right| \\
& +C_{1} \cdot
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}故当\end{CJK} \(x>0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{d x}{x \sqrt{x^{2}+x+1}} \\
= & -\ln \left|\frac{x+2+2 \sqrt{x^{2}+x+1}}{x}\right|+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}当\end{CJK} \(x<0\) \begin{CJK}{UTF8}{mj}时\end{CJK},

\[
\begin{aligned}
& \int \frac{d x}{x \sqrt{x^{2}+x+1}} \\
= & -\ln \left|\frac{2 x}{x+2-2 \sqrt{x^{2}+x+1}}\right|+C_{1} \\
= & -\ln \left|\frac{2 x\left(x+2+2 \sqrt{x^{2}+x+1}\right)}{(x+2)^{2}-4\left(x^{2}+x+1\right)}\right|+C_{1} \\
= & -\ln \left|\frac{x+2+2 \sqrt{x^{2}+x+1}}{x}\right|+C .
\end{aligned}
\]

\[
\begin{aligned}
& \text { 总之,不论 } x \text { 为正或为梨,均有 } \\
& \int \frac{d x}{x \sqrt{x^{2}+x+1}} \\
& =-\ln \left|\frac{x+2+2 \sqrt{x^{2}+x+1}}{x}\right|+C .
\end{aligned}
\]

*)\begin{CJK}{UTF8}{mj}利用\end{CJK} 1850 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}. 1857. \(\int \frac{d x}{x^{2} \sqrt{x^{3}+x-1}}\).

\begin{CJK}{UTF8}{mj}解\end{CJK} \begin{CJK}{UTF8}{mj}作代换\end{CJK} \(t=\frac{1}{x}\), \begin{CJK}{UTF8}{mj}则\end{CJK} \(x^{2} \sqrt{x^{2}+x-1}\)

\[
=\operatorname{sgn} t: \frac{\sqrt{-t^{2}+t+1}}{t^{3}}, d x=-\frac{d t}{t^{2}} \text {. 于是 }
\]

\[
\begin{aligned}
& \int \frac{d x}{x^{2} \sqrt{x^{2}+x-1}}=-(\operatorname{sgn} t) \int \frac{t}{\sqrt{-t^{2}+t+1}} d t \\
& =-(\operatorname{sgn} t) \cdot\left(-\frac{1}{2} \int \frac{d\left(-t^{2}+t+1\right)}{\sqrt{-t^{2}+t+1}}\right. \\
& \left.+\frac{1}{2} \int \frac{d t}{\sqrt{-t^{2}+t+1}}\right) \\
& =-(\operatorname{sgn} t) \cdot\left(-\sqrt{-t^{2}+t+1}\right. \\
& \left.+\frac{1}{2} \arcsin \frac{2 t-1}{\sqrt{5}}\right)^{\circ \prime}+C \\
& =(\operatorname{sgn} x) \cdot\left(\frac{\sqrt{x^{2}+x-1}}{|x|}\right.
\end{aligned}
\]

\(\left.+\frac{1}{2} \arcsin \left(\frac{x-2}{x \sqrt{5}}\right)\right]+C\)

\(=\frac{\sqrt{x^{2}+x-1}}{x}+\frac{1}{2} \arcsin \left(\frac{x-2}{|x| \sqrt{5}}\right)+C\).

\begin{CJK}{UTF8}{mj}其存在域为\end{CJK} \(\left|x+\frac{1}{2}\right|>\frac{\sqrt{5}}{2}\).

*) \begin{CJK}{UTF8}{mj}利用\end{CJK} 1850 \begin{CJK}{UTF8}{mj}题的结果\end{CJK}.

\begin{enumerate}
  \setcounter{enumi}{1857}
  \item \(\int \frac{d x}{(x+1) \sqrt{x^{2}+1}}\).
\end{enumerate}

\begin{CJK}{UTF8}{mj}鿉\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(y=x+1\), \begin{CJK}{UTF8}{mj}本题即转化为\end{CJK} 1856 \begin{CJK}{UTF8}{mj}题的类型\end{CJK}. \begin{CJK}{UTF8}{mj}由\end{CJK} \begin{CJK}{UTF8}{mj}于解法类似\end{CJK}, \begin{CJK}{UTF8}{mj}且\end{CJK} \(x+1\) \begin{CJK}{UTF8}{mj}的符号对结果没有影响\end{CJK}, \begin{CJK}{UTF8}{mj}故仅就\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{(x+1) \sqrt{x^{2}+1}}=\int \frac{d y}{y \sqrt{y^{2}-2 y+2}} \\
& =-\int \frac{d\left(\frac{1}{y}\right)}{\sqrt{\frac{2}{y^{2}}-\frac{2}{y}+1}} \\
& =-\frac{1}{\sqrt{2}} \ln \left|\frac{1}{y}-\frac{1}{2}+\frac{\sqrt{y^{2}-2 y+2}}{y \sqrt{2}}\right|+C_{1} \\
& =-\frac{1}{\sqrt{2}} \ln \left|\frac{1-x+\sqrt{2\left(x^{z}+1\right)}}{x+1}\right|+C \text {. }
\end{aligned}
\]

\[
\text { 1859. } \int \frac{d x}{(x-1) \sqrt{x^{2}-2}} \text {. }
\]

\begin{CJK}{UTF8}{mj}解\end{CJK} \begin{CJK}{UTF8}{mj}设\end{CJK} \(x-1=\frac{1}{t}\), \begin{CJK}{UTF8}{mj}则\end{CJK}

\[
(x-1) \sqrt{x^{2}-2}=\frac{\sqrt{1+2 t-t^{2}}}{t|t|}, d x=-\frac{1}{t^{2}} d t \text {, }
\]

\begin{CJK}{UTF8}{mj}代入得\end{CJK}

\[
\begin{aligned}
& \int \frac{d x}{(x-1) \sqrt{x^{2}-2}}=-\int \frac{\operatorname{sgn} t d t}{\sqrt{1+2 t-t^{2}}} \\
&=-\operatorname{sgn} t \cdot \arcsin \left(\frac{t-1}{\sqrt{2}}\right)+C \\
&= \operatorname{arc} \sin \left(\frac{x-2}{|x-1| \sqrt{2}}\right)+C \quad(|x|>\sqrt{2}) . \\
& 1860^{+} \cdot \int \frac{d x}{(x+2)^{2} \sqrt{x^{2}+2 x}-\overline{5}} . \\
& \quad \text { 设 } x+2=\frac{1}{t}, \text { 则 } \\
&(x+2)^{2} \sqrt{x^{2}+2 x-5}=\frac{\sqrt{1-2 t-5 t^{2}}}{\left.t^{2} \mid t\right]},
\end{aligned}
\]

\begin{center}
\includegraphics[max width=\textwidth]{2022_12_26_c19bf7cf4ca87c30c547g-075}
\end{center}

\[
\begin{aligned}
& \text { 解 } \int \sqrt{2+x+x^{2}} d x \\
& =\int \sqrt{\frac{7}{4}+\left(x+\frac{1}{2}\right)^{2}} d\left(x+\frac{1}{2}\right) \\
& =\frac{2 x+1}{4} \sqrt{2+x+x^{2}} \\
& +\frac{7}{8} \ln \left(x+\frac{1}{2}+\sqrt{2+x+x^{2}}\right)+C .
\end{aligned}
\]

\begin{enumerate}
  \setcounter{enumi}{1862}
  \item \(\int \sqrt{x^{4}+2 x^{2}-1} x d x\).
\end{enumerate}

\[
\begin{aligned}
& \text { 霁 } \int \sqrt{x^{4}+2 x^{2}-1} x d x \\
& =\frac{1}{2} \int \sqrt{\left(x^{2}+1\right)^{2}-\overline{2}} d\left(x^{2}+1\right) \\
& =\frac{x^{2}+1}{4} \sqrt{x^{4}+2 x^{2}-1} \\
& -\frac{1}{2} \ln \left(x^{2}+1+\sqrt{x^{4}+2 x^{2}-1}\right)+C \text {. }
\end{aligned}
\]

\[
\text { 1864. } \begin{aligned}
& \int \frac{1-x+x^{2}}{x \sqrt{1+x-x^{2}}} d x . \\
& \text { 由干 } \\
& \int \frac{d x}{x \sqrt{1+x-x^{2}}} \\
&=-\ln \left|\frac{\left.2+x+2 \sqrt{1+2 x^{2}-1}\right)+C \cdot}{x}\right|+x^{2} \\
& \text { (可仿照 } 1856 \text { 题求得), }
\end{aligned}
\]

(\begin{CJK}{UTF8}{mj}可仿照\end{CJK} 1856 \begin{CJK}{UTF8}{mj}题求得\end{CJK}),

\[
\begin{aligned}
& \int \frac{d x}{\sqrt{1+x-x^{2}}}=\int \frac{d\left(x-\frac{1}{2}\right)}{\sqrt{\frac{5}{4}-\left(x-\frac{1}{2}\right)^{2}}} \\
= & \operatorname{arc} \sin \left(\frac{2 x-1}{\sqrt{5}}\right)+C_{2},
\end{aligned}
\]

\[
\begin{aligned}
& \int \frac{x d x}{\sqrt{1+x-x^{2}}}=\int \frac{\left(x-\frac{1}{2}\right)+\frac{1}{2}}{\sqrt{\frac{5}{4}-\left(x-\frac{1}{2}\right)^{2}}} d\left(x-\frac{1}{2}\right) \\
& =-\sqrt{1+x-x^{2}}+\frac{1}{2} \arcsin \left(\frac{2 x-1}{\sqrt{5}}\right)+C_{3},
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}所以\end{CJK}

\[
\begin{aligned}
& \int \frac{1-x+x^{2}}{x \sqrt{1+x-x^{2}}} d x=\int \frac{d x}{x \sqrt{1+x-x^{2}}} \\
& -\int \frac{d x}{\sqrt{1+x-x^{2}}}+\int \frac{x d x}{\sqrt{1+x-x^{2}}} \\
= & -\ln \left|\frac{2+x+2 \sqrt{1+x-x^{2}}}{x}\right| \\
& +\frac{1}{2} \arcsin \left(\frac{1-2 x}{\sqrt{5}}\right)-\sqrt{1+x-x^{2}}+C .
\end{aligned}
\]

\begin{CJK}{UTF8}{mj}其中存在域为满足不等式\end{CJK} \(1+x-x^{2}>0\) \begin{CJK}{UTF8}{mj}且\end{CJK} \(x \neq 0\) \begin{CJK}{UTF8}{mj}的\end{CJK}

\[
\text { 一切 } x \text { 值, 即 }\left|x-\frac{1}{2}\right|<\frac{\sqrt{5}}{2} \text { 及 } x \neq 0 \text {. }
\]

\begin{enumerate}
  \setcounter{enumi}{1864}
  \item \(\int \frac{x^{2}+1}{x \sqrt{x^{4}+1}} d x\).
\end{enumerate}

\[
\begin{aligned}
& \int \frac{x^{2}+1}{x \sqrt{x^{4}+1}} d x . \\
= & \int \frac{\operatorname{sgn} x \cdot\left(1+\frac{1}{x^{2}}\right)}{\sqrt{x^{2}+\frac{1}{x^{2}}}} d x=\int \frac{\operatorname{sgn} x d\left(x-\frac{1}{x}\right)}{\sqrt{\left(x-\frac{1}{x}\right)^{2}+2}} \\
= & \operatorname{sgn} x \cdot \ln \left(x-\frac{1}{x}+\sqrt{\left(x-\frac{1}{x}\right)^{2}+2}\right)+C_{1} \\
= & \ln \left|\frac{x^{2}-1+\sqrt{x^{4}+1}}{x}\right|+C .
\end{aligned}
\]
-->
