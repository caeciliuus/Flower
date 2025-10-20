---
Class: PHYS 24100
Type: Lecture notes
Date: 2025-09-08
tags:
  - s1
  - phys241
  - lecture
---
- Calculate E-field due to charge distribution
	1. Extension of point charge approach: $\vec{E}=\frac{kq}{r^2}\hat{r}\to d\vec{E}=\frac{kdq}{r^2}\hat{r}$
	2. Gauss' Law: $\oint \vec{E}_{n}~ d{A}=\frac{1}{\varepsilon}Q_{inside}$
- Charge distribution steps
	1. Understand symmetry
	2. Choose $dq$
	3. Evaluate $d\vec{E}$ contribution from infinitesimal charge element
	4. Exploit symmetry
	5. Set up and solve integral
	6. Check limiting cases
- $\lambda=$ charge/unit length
- $\sigma=$ charge/unit area
- $\rho=$ charge/unit volume

> [!exm] Calculate $\vec{E}$ along the z-axis due to a circular ring of uniform (+) charge
> $$dq=\lambda ds\to d\vec{E}=\frac{1}{4\pi\varepsilon_{0}} \frac{\lambda ds}{r^2},r^2=z^2+R^2\text{ (right triangle)}$$
> $$d\vec{E}=\frac{1}{4\pi\varepsilon_{0}} \frac{\lambda ds}{z^2+R^2}, \text{ break }dE \text{ into compmonents:}$$
> $$\sum dE_{\perp}=0\to \text{ only solve for }z \text{: } \cos\theta=\frac{z}{r}=\frac{z}{\sqrt{ z^2+R^2 }}$$
> $$\text{Setup integral: }\vec{E}=E_{z}=\int  dE_{z}= \frac{z\lambda}{4\pi\varepsilon_{0}(z^2+R^2)^{3/2}}\int  _{0}^{2\pi r}~ d{s}$$
> $$\text{Solving yields }\vec{E}= \frac{z\lambda2\pi R}{4\pi\varepsilon_{0}(z^2+R^2)^{3/2}}$$

>[!exm] Calculate $\vec{E}$ along z=axis due to a non-conducting disk or uniform (+) charge
> $$dq=rdA=\sigma2\pi rdr\to \vec{E}\text{ due to ring element: }d\vec{E}= \frac{z\sigma2r dr}{4\varepsilon_{0}(z^2+r^2)^{3/2}}$$
> $$E=\int  dE=\int  _{0}^R \left[ \frac{\sigma_{z}}{4\pi\varepsilon_{0}} \right] \frac{2rdr}{(z^2+r^2)^{3/2}},\text{ let }x=z^2+r^2,dx=2rdr$$
> $$E=\int  _{z^2} ^{z^2+r^2}Cx^{-3/2}=\frac{\sigma}{2\varepsilon_{0}}\left[ 1-\frac{z}{\sqrt{ z^2+R^2 }} \right]$$
