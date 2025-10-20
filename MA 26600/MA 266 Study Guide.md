---
Class: "[[MA 26600.base|MA 26600]]"
Type: Study guide
Date: 2025-10-06
tags:
  - exam
  - s1
  - ma266
---
# To Study
- [ ] **Integrating factor**
- [ ] Euler's Method
- [ ] Population
- [ ] Salt tank application
# Equations
- Euler's Method: $y_{n+1}=y_{n}+hf(x_{n},y_{n})$
- First-order linear differential equation: $y'+p(t)y=g(t)$ ^3fbd18
- Integrating factor - can be used with any first-order linear ODE: $\rho=\pm e^{\int P(x)~ d{x}}$
- Given $\frac{dy}{dx}+P(x,y)=Q(x)$, use formula $y(x)=\frac{\int \rho(x)Q(x)~ d{x}+C}{\rho(x)}$
- If roots from a characteristic equation are not in $\mathbb{R}$, use substitution $r=e^{ax}\cos bx,e^{ax}\sin bx$ where $r=a\pm ib$
- Given $\int \frac{1}{A(Q-B)}$, use partial fraction decomposition: $\frac{1}{QA}+\frac{1}{Q(Q-B)}$
- Mixing tank mass flow rate: $\frac{dQ}{dt}=r_{in}c_{in}-r_{out} \frac{Q(t)}{V(t)}$
# Reduction of order
1. Set $y_{2}=v(x)y_{1}(x)$ 
2. Differentiate: $y'_{2}=v'y_{1}+vy_{1}',y_{2}''=v''y_{1}+vy_{1}''$
3. Substitute $y_{2},y_{2},y_{2}''$ and Use that $y_1$ satisfies the ODE to cancel the $v$ terms.  You obtain a first–order linear ODE for $w=v'$:
$$w' + \Big(2\,\frac{y_1'}{y_1} + P(x)\Big) w = 0.$$
4. Solve for $w=v'$ (integrating factor):
$$
w = C\,\exp\!\left(-\int\!\Big(2\,\frac{y_1'}{y_1}+P\Big)\,dx\right)
    = C\,\frac{e^{-\int P\,dx}}{y_1^{2}}.
$$
5. Integrate once more to get $v$:
$$v(x) = C \int \frac{e^{-\int P\,dx}}{y_1(x)^2}\,dx + K$$
6. Second solution (drop the multiple of $y_1$):
$$
\boxed{\,y_2(x)=y_1(x)\int \frac{e^{-\int P(x)\,dx}}{y_1(x)^{2}}\,dx\, }.
$$

>[!exm|*] Given that $y_{1}=t$ is a solution to the differential equation $t^3y''-ty'+y=0$, find another solution
> $$y_{2}=v(t)y_{1}=v(t)t=vt$$
> $$y'=v't+v$$
> $$y''=v''t+v'+v'=v''t+2v'$$
> $$t^3(v''t+2v')-t(v't+v)+vt=0$$
> $$t^4v''+2t^3v'-t^2v-\cancel{ tv }+\cancel{ tv }=0$$
> $$t^4v''+2t^3v'-t^2v'=0$$
> $$t^4v''+(2t^3-t^2)v'=0$$
> $$v''+\left( \frac{2t^3-t^2}{t^4} \right)v'=0$$
> $$\text{Let }u=v' \text{ to get equation } u'+ \left( \frac{2t^3-t^2}{t^4} \right)u=0\text{ then solve for u(t) and integrate it}$$

---
# Bernoulli Equation
1. Rearrange equation to get the form $\frac{dy}{dx}+P(x)y=Q(x)y^n$
2. Let $v=y^{1-n}$, solve for $\frac{dv}{dx}=\frac{dy}{dx}\cdot \frac{dv}{dy}$
3. Multiply by $\frac{dy}{dx}$ (found from $\frac{dv}{dx}$) and substitute $v$ and $\frac{dv}{dx}$ *[sort of, this step is hard to explain]*
4. Once you get form $\frac{dv}{dx}+P(x)v=Q(x)v^n$, find integrating factor $e^{\int P(x)~ d{x}}$ and multiply the equation by it 
5. Integrate then subsitute $v=y^{1-n}$ back into to the solution

> [!exm|*] Find the general solution of the Bernoulli equation $y'-y=4y^3$
> $$v=y^{1-n}=y^{-2}, \frac{dv}{dx}=-\frac{2}{y^3} \frac{dy}{dx}$$
> $$-\frac{2}{y^3} \frac{dy}{dx}+ \frac{2}{y^2}=-8=\frac{dv}{dx}+2v=-8\to\text{integrating factor: }\rho=e^{\int  2~ d{x}}=e^{2x}$$
> $$e^{2x} \frac{dv}{dx}+2ve^{2x}=-8e^{2x}= \frac{d}{dx}(e^{2x}v)=-8e^{2x}$$
> $$\int   \frac{d}{dx}e^{2x}v ~dx=\int  -8e^{2x}~ d{x}$$
> $$e^{2x}v=-4e^{2x}+C\to y^{-2}=Ce^{-2x}-4\to y(x)=\frac{1}{\sqrt{ Ce^{-2x}-4 }}$$
# Existence & Uniqueness Theorem
1. Rearrange equation to get it in [[#^3fbd18|standard form]]
2. Isolate $y'$ and evaluate discontinuities
3. Create number range with discontinuities and check which one fits the initial condition, this is the answer
# Mixing-tank Problems
Typically given volume $v_{0}$, initial mass $Q_{0}$, concentration flowing in/out of tank $c_{in/out}$, volume rate flowing in/out of tank $r_{in/out}$
- Volume balance: $V(t)=V_{0}+(r_{in}-r_{out})t$
- Rate in: $r_{in}c_{in}$
- Rate out: $r_{out}\frac{Q}{V(t)}$
- ODE: $\frac{dQ}{dt}=r_{in}c_{in}(t)-r_{out} \frac{Q}{V(t)}$