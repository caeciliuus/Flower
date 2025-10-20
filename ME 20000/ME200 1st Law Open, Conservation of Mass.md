---
Class: "[[ME 20000]]"
Type: Lecture notes
Date: 2025-10-15
tags:
  - lecture
  - 25-26
  - s1
  - me200
---
# Conservation of Mass
- Closed system is fixed qty. of matter (control mass)
- Open system is region of space (control volume)
	- Boundary called control surface
- Use $\dot{r}$ for velocity
	- $\dot{r}_{n}$ is magnitude of component of $\dot{r}$ along normal vector to system boundary
- In **1-dimensional flow model,** mass flow $\perp$ to boundary
	- Intensive properties uniform along entrance/exit surfaces
- In time $\Delta t,$ mass $\Delta \rho A \dot{r}\Delta t$ crosses surface and as $\lim_{ \Delta t \to 0 }$, we get $\dot{m}=\rho A \dot{r}$
- Single in/output conservation of mass: $\frac{dm}{dt}=\dot{m}_{in}-\dot{m}_{out}$
- Multiple in/output conservation of mass: $\frac{dm}{dt}=\sum_{i}\dot{m}_{i}^{in}-\sum_{j}\dot{m}_{j}^{out}$
- In steady state, properties are constant w.r.t time, so $\frac{dm}{dt}=0$
# 1st Law Open
- $\frac{dE}{dt}=\dot{Q}-\dot{W}$
- Mass that enters a system brings energy with it: mass inflow $\dot{m}$ carries $\dot{E}^{in}=\frac{1}{2}\dot{m}^{in}(\dot{r}^{in})^2+\dot{m}^{in}gz^{in}+\dot{U}^{in}=\dot{m}^{in}e^{in}$ where $e^{in}=\frac{1}{2}(\dot{r}^{in})^2+gz^{in}+u^{in}$
- If $\dot{m}^{out}$ is in 1d- flow, pressure is $p^{out}$ and as mass leaves, system pushes on it with force $F=p^{out}A^{out}$
$$\frac{dE}{dt}=\dot{Q}-\dot{W}+\sum^{N_{in}}_{i=1}\dot{m}^{in}_{i}\left[ \frac{1}{2}(\dot{r}^{in}_{i})^2+gz^{in}_{i}+h^{in}_{i} \right]-\sum ^{N_{out}}_{j=1}\dot{m}^{out}_{j}\left[ \frac{1}{2}(\dot{r}^{in}_{j})^2+gz^{out}_{j}+h_{j}^{out} \right]$$
- Enthalpy $H=U+pV$