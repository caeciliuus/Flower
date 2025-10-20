---
Class: "[[PHYS 24100]]"
Type: Cheatsheet
Date: 2025-09-28
tags:
  - cheatsheet
  - s1
  - exam
  - phys241
---
# Discrete Charge Distributions
 $$\vec{F}= \frac{kq_{1}q_{2}}{r^2}\hat{r}$$
 $$\vec{E}=\frac{\vec{F}}{q}= \frac{kq}{r^2}\hat{r}$$
$$\vec{E}_{P}=\sum_{i} \vec{E}_{iP}$$
$$\vec{p}=q\vec{L}$$
$$\vec{\tau}=\vec{p}\times \vec{E}$$
$$U=-\vec{p}\cdot \vec{E}+U_{0}$$
# Continuous Charge Distributions
$$\vec{E}=\int  d\vec{E}=\int  \frac{kdq}{r^2}\text{ where }dq =\rho dV \text{ or }\sigma dA\text{ or }\lambda dL$$
$$\Phi=\int  _{S}\vec{E}\cdot \hat{n}~ d{A}$$
$$\Phi=\oint_{S}\vec{E}\cdot \hat{n}~dA=\oint_{S}E_{n}~dA=\frac{Q_{\text{inside}}}{\varepsilon_{0}}$$
$$E_{n}=\frac{\sigma}{\varepsilon_{0}}\text{ where }\sigma \text{ is local surface charge density just outside conductor surface}$$
$$E_{R}=2k \frac{\lambda}{R}=\frac{1}{2\pi\varepsilon_{0}} \frac{\lambda}{R}\text{ for line charge of infinite length}$$
$$E_{z}= \frac{kQz}{(z^2+a^2)^{3/2}}\text{ on the axis of a charged ring}$$
$$E_{r}= \begin{cases}
\frac{kQ}{r^2} &\text{if }r>R\\ \\
0&\text{if }r<R
\end{cases}$$
# Electric Potential
$$\Delta V=V_{b}-V_{a}=\frac{\Delta U}{q_{0}}=-\int  _{a}^b \vec{E}\cdot d\vec{\ell}$$
$$dV=-\vec{E}\cdot d\vec{\ell}$$
$$V= \frac{kq}{r}- \frac{kq}{r_{ref}}~(V=0 \text{ if }r=\infty) \text{ for point charge}$$
$$V=\sum_{i} \frac{kq_{i}}{r_{i}}~(v=0\text{ if }r_{i}=\infty,i=1,2)$$
$$V=\int   \frac{kdq}{r}~(V=0\text{ if }r=\infty)\text{ for continuous charge distribution}$$
$$U=-\nabla V=-\left(  \frac{\partial V}{\partial x}\hat{i}+\frac{\partial V}{\partial y}\hat{j}+\frac{\partial V}{\partial z}\hat{k} \right)$$
$$1V = 1J/C$$
$$U=q_{0}V= \frac{kq_{0}q}{r}~(U=0\text{ if }r=\infty)\text{ for two point charges}$$
$$V=\frac{kQ}{\sqrt{ z^2+a^2 }}~(V=0\text{ if }|z|=\infty)\text{ for axis of uniformly charged ring}$$
$$V=2\pi k\sigma|z|\left( \sqrt{ 1+ \frac{R^2}{a^2} }-1 \right)~(V=0\text{ if }|z|=\infty)\text{ for axis of uniformly charged disk}$$
$$V=V_{0}-2\pi k\sigma|x|~(V=V_{0}\text{ if }x=0)\text{ for infinite plane of charge}$$
$$V= \begin{cases}
\frac{kQ}{r} &\text{if }r\geq R\\
\frac{kQ}{r}&\text{if }r\leq R
\end{cases}~(V=0\text{ if }r=\infty)\text{ for spherical shell of charge}$$
$$V=2k\lambda \ln\left( \frac{R_{ref}}{R} \right)~(V=0\text{ if }r=R_{ref}) \text{ for infinite line charge}$$
$$U=\frac{1}{2}\sum^n _{i=1}q_{i}V_{i}\text{ for system of point charges}$$
$$U=\frac{1}{2}QV\text{ for conductor with charge }Q\text{ at potential V}$$
$$U=\frac{1}{2}\sum_{i=1}^nQ_{i}V_{i}\text{ for system of conductors}$$