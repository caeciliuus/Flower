---
Class: PHYS 24100
Type: Lecture notes
Date: 2025-09-08
tags:
  - lecture
  - s1
  - phys241
---
- Gauss' Law relates $\vec{E}$ fields at points on a closed Gaussian surface and the netcharge enclosed by that surface. Given by $\oint _SE_{n}~ d{A}=\frac{1}{\varepsilon_{0}}Q_{inside}=\Phi$
- How to set up flux equation
	1. Define $\vec{A}$, $\perp$ to the loop -> $|\vec{A}|=$ area
	2. Scalar $\Phi=\vec{v}\cdot \vec{A}\to|\Phi|=vA\cos\theta$
- In a closed surface, $\vec{A}$ point outward
- To calculate flux of a non-uniform arbitrary shape, $\Phi=\sum \vec{E}\cdot d\vec{A}$
	- Taking $\lim_{ \Delta A \to 0 }$, we get $\oint \vec{E}\cdot \Delta \vec{A}=\Phi$
- Gauss' Law states $\varepsilon_{0}\Phi=\varepsilon_{0}\oint \vec{E}\cdot d\vec{A}=q_{enc}$
	1. If $\vec{E}\parallel \vec{A}\text{ }[\theta=0]\text{ }\vec{E}\cdot d\vec{A}=\vec{E}d\vec{A}$
	2. If $\vec{E}\perp \vec{A}\text{ }[\theta=90]~\vec{E}\cdot d\vec{A}=0$
	3. $\vec{E}$ has the same value at all points
	4. Holds in a vacuum -> additional factor in non-vacuum
- Gauss' Law and Coulomb's Law are equivalent, can be derived from eachother
- Shell of uniform charge attracts/repels a charged particle that's outside the shell as if all the shell's charge were concentrated at the shell center
- Shell of uniform charge exerts no electrostatic force on a charged particle located inside the shell
- Spherically symmetric charge distribution
	- Outside: $\vec{E}=\frac{\rho R_{sp}^3}{3\varepsilon_{0}R_{GS}^2}$
		- $E\propto R$
	- Inside: $\vec{E}= \frac{q_{enc}R_{GS}}{4\pi\varepsilon_{0}R_{sp}^3}$
		- $E\propto \frac{1}{r^2}$