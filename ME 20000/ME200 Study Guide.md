---
Class: "[[ME 20000]]"
Type: Study guide
Date: 2025-09-30
tags:
  - studyguide
  - exam
  - s1
  - me200
---
# Definitions ![[Pasted image 20251001142852.png|right|294x257]]
## System Types 
- **System**: Portion of space or matter selected for analysis.
- **Surroundings**: Everything outside the system.
- **Boundary**: Real/imaginary surface separating system from surroundings.
- **Open System (Control Volume)**: Mass and energy can cross boundary.
- **Closed System (Control Mass)**: Fixed mass; only energy crosses boundary.
- **Isolated System**: No mass or energy crosses boundary.
## Properties ![[Pasted image 20250930220103.png|right|295]]
- **Intensive**: Independent of system size ($T, p, v, u, h, s$). 
- **Extensive**: Scale with system size ($V, U, H, S$).
- **Specific Property**: Extensive property per unit mass (e.g., $v = V/m$).
## State & State Principle
- **State**: Condition of a system described by its properties.
- **State Principle**: For a pure, simple compressible substance, any **two independent intensive properties** define the state.
## Energy Forms ![[Pasted image 20251001143225.png|right|300]]
- **Kinetic Energy (KE)** =$\frac{1}{2}mv^2$
- **Potential Energy (PE)** = $mgh$
- **Internal Energy (U)** = Microscopic molecular energy (translation, vibration, rotation, chemical/nuclear interactions).
- **Enthalpy (H)** = $U + pV$
- **Specific forms**: $u = U/m, h = H/m.$
## Heat vs Work 
- **Heat (Q)**: Energy transfer due to temperature difference.
- **Work (W)**: Energy transfer due to force × displacement or other mechanical interaction.
- Both are **path functions**, not properties → inexact differentials $(\delta Q,\delta W)$.
## Phases and State Definitions 
- **Saturated Liquid (f)**: At boiling/condensation point but not vaporised; $T = T_{sat}$ at given $p$.
	- Any heat addition will start creating vapor.
- **Saturated Vapor (g)**: At boiling/condensation point but not condensed; $T = T_{sat}$ at given $p$.
	- Any cooling will start forming liquid.
- **Two-Phase Mixture (Liquid–Vapor Dome)**: Combination of liquid + vapor at saturation.
	  - **Quality (x)** = $\frac{m_{vap}}{m_{vap}+m_{liq}}$
		- $x = 0$ → saturated liquid
		- $0 < x < 1$ → mixture
		- $x = 1$ → saturated vapor
- **Compressed (Subcooled) Liquid**: $T < T_{sat}$ (for given p).
- **Superheated Vapor**: $T>T_{sat}$ (for given $p$).
## Property Tables
- **Single-phase regions**: Use compressed liquid or superheated vapor tables.
- **Two-phase regions**: Use saturation tables - apply $y = y_f + x(y_g − y_f)$   (works for $v, u, h, s$).
- **Saturated liquid approximation** (for compressed liquids):
	- $v(T, p) ≈ v_f(T)$
	- $u(T, p) ≈ u_f(T)$
	- $h(T, p) ≈ h_f(T) + v_f(T)(p − p_{sat}(T))$
## Process Types
- **Isothermal:** $T = C$.
- **Isobaric:** $p = C$.
- **Adiabatic:** $Q = 0$.
- **Polytropic:** $pV^n=C$
# Lecture Notes
## Work & Differentials
- For mechanical systems, $\Delta KE+\Delta PE=-W$
- Inexact differentials written as $\delta$ 
- Differential work done by a system over displacement $dx$ is given by $\delta W=Fdx=\int p~dV$
	- Boundary work given by area under PV curve
	- Path-dependent
	- Must assume quasi equilibrium to use $Fdx=\int pdV$. $p$ must be well-defined from process 1 -> 2 
### Polytropic: quasi-equilibrium process with $pV^n=c$
- Isobaric process is polytropic with $n=0$
- For any ideal gas, an isothermal process (1) is polytropic with $n=1$; (2) has $c=mRT$
### Shaft work
- Shaft of radius $r$ rotates at angular velocity $\omega$, exerting tangential force on surroundings
- Differential displacement is $d\theta$
- Shaft does differential work: $\delta W=F_{t}^{\theta}=\tau d\theta$
- Shaft power is $\dot{W}=F_{t}v_{t}=\left( \frac{\tau}{r} \right)(r\omega)=\tau\omega$
### Spring work
- Consider a linear spring with spring constant $k$  
- When relaxed, the spring has length $\ell$
- If the spring compresses further by differential length $dx$, then
	- Spring resists with force $kx$
	- Surroundings do differential work: $\delta W=kxdx$
### Electrical work
- suppose current i = dq/dt flows from ground to P  
- then over differential duration dt,
	- differential charge $dq = idt$ moves from ground to $P$
	- electric field does differential work  $\delta W= \varepsilon i~ dq$ on electrons
## 1st Law
- For general, closed systems, the 1st law is $\Delta KE+\Delta PE+\Delta U=Q-W$
- In steady state, $\frac{dE}{dt}=0$, so $\dot{Q}=\dot{W}$
- Differential heat is inexact - $\delta Q$
- Conduction: nearby particles jostling each other -> $\dot{Q}=T_{h}-T_{c}$
- Radiation: exchange of protons -> $\dot{Q}=T_{_{h}}^4-T_{c}^4$
- Convection: conduction and radiation between a solid and an adjacent fluid -> $\dot{Q}=T_{h}-T_{c}$
## Property charts
- Phase: qty of matter w/ homogenous structure (all solid/liquid/gas) and homogenous composition 
- Substances don't mix from multiple phases
- Pure substance has fixed, uniform composition
- Simple systems have only one type of work interaction 
	- For simple compressible systems, that's boundary work 
### State principle
- State principle: only takes 2 **independent, intensive** properties to define their equilibrium states
	- Assumes no $x_{cm}$ motion -> no $KE$ or $PE$
	- In equilibrium, all properties can be inferred from the state
### P-V-T Surface
- For pure simple compressible systems, we can treat 
	- $v$ and $T$ as independent variables and $p$ as a function of $v$ and $T$
### Drawing p-v diagrams by hand
1. Draw vapor dome
2. If needed, look up substance's critical point to calibrate axes
3. Solve ideal gas law for $p=\frac{RT}{v}$
	- Looks like $y=\frac{1}{x}$ when $T$ is constant
		- Draw isotherms sloping **down** in gas region
	- When $T_{2}>T_{1},p_{2}(v)=\frac{RT_{2}}{v}> \frac{RT_{1}}{v}=p_{1}(v)$
		- Draw $T_{2}$ isotherm above $T_{1}$ isotherm
- Isotherms: (1) are horizontal inside the vapor dome; (2) slope in the same direction in the liquid region as in the gas region
### Drawing t-v diagrams by hand
1. Draw the vapor dome
2. If needed, look up substance’s critical point to calibrate axes
3. Solve the ideal gas law for $T = pv/R$
	- This looks like $y = x$ when $p$ is constant
		- Draw isobars sloping **up** in gas region
	- When $p_{2}>p_{1}, T_{2}(v)=\frac{p_{2}v}{R}> \frac{p_{1}v}{R}$
		- Draw $p_{2}$ isobar above $p_{1}$ isobar
- Isobars: (1) are horizontal inside the vapor dome; (2) slope in the same direction as the gas region
## Property tables  ![[Pasted image 20250930221602.png|right|269x285]]
- Intensive properties don't change if we clone the system
	- $T,p,v,u,h,s$
- Two properties are independent if we can change one without changing the other
	- $T,p,v$ are all independent in single-phase regions
	- In 2 phase regions:
		- $T$ and $p$ are not independent, so can't determine system state
		- But $T$ and $v$ are independent, as are $p$ and $v$
### Quality 
- Any two-phase liquid-vapor mixture has a quality: $x=\frac{m_{vap}}{\sum m}=1- \frac{m_{liq}}{\sum m}$
- Given quality $x$, the mixture's specific volume is $v=\frac{V}{m} \frac{V_{liq}+V_{vap}}{m}= \frac{m_{liq}v_{liq}+m_{vap}v_{vap}}{m}=(1-x)v_{liq}+xv_{vap}=v_{liq}+x(v_{vap}-v_{liq})$
	- These formulas also work for $u,h,s$ ![[Attachments/Pasted image 20250930221611.png|right|358x265]] 
- In interpolation, we find a function $f$ s.t $y_{1}=f(x_{1}),\dots,y_{n}=f(x_{n})$ and approximate the unknown $y$ by $f(x)$
- For $x$ between $x_{i}$ and $x_{i+1}$, approximate $y$ by $y=y_{i}+ \frac{y_{i+1}-y_{i}}{x_{i+1}-x_{i}}$
- For any process moving a closed system from state 1 to 2, $\Delta U=U_{2}-U_{1}=m(u_{2}-u_{1})$ 
### Evaluating $\Delta U$ with property tables
- If system is a single phase in state $i$, can find $u_{i}$ in compressed liquid or superheated vapor table
- If system is a two-phase liquid-vapor mixture in state $i$:
	- $u_{i}=u_{liq}+x_{i}(u_{vap}-u_{liq})$
	- Can find $u_{liq}$ and $u_{vap}$ in saturation table
	- Quality $x_{i}$ must be given or calculated
## Modeling liquids and solids
- Usually can’t measure internal energy $U$ directly
- Consider system of mass $m$ in rigid tank
	- Assumptions
		- No bulk motion, so $\Delta KE=\Delta PE=0$
		- Constant volume, so $W=0$
		- From 1st law for closed systems, $\Delta U=Q$
	- Add small, measured energy $Q$ via heat transfer
	- Measure temperature change $\Delta T$; then
		- $\frac{Q}{m\Delta T}= \frac{\Delta U}{m\Delta T}= \frac{\Delta u}{\Delta T}\approx \frac{\partial u}{\partial T}=c_{v}(T,v)$
- Consider simple compressible system in static equilibrium - how much does its specific enthalpy $h(T,p)$ change (1) per unit change in $T$ with $p$ held constant? => $c_{p}(T,p)=\left(  \frac{\partial h}{\partial T} \right)_{p}$
### Specific heats and state transformations
- For simple compressible systems, any two independent intensive properties define the state
- Equations like $pv=RT$ allow state transformations
	- Suppose we choose state $(T,v)$ and have equation of state $p=f(T,v)$
		- Then $c_{p}(p,v)=c_{p}(T,f(T,v))$, a function of $(T,v)$ only
		- Similarly we can write $c_{v}$ as a function of $(T,p)$ only 
- Specific heats are intensive properties, only defined in single-phase regions
	- $c_{p}\geq c_{v}$ since no boundary work when $v$ is constant
	- $k=\frac{c_{p}}{c_{v}}$ is specific heat ratio
### Saturated liquid approximation 
- For a compressed liquid in state $(T,p),$
	- $v(T,p) \approx v_{\mathrm{liq}}(T)$
	- $u(T,p) \approx u_{\mathrm{liq}}(T)$
	- $h(T,p) \approx u_{\mathrm{liq}}(T) + p\,v_{\mathrm{liq}}(T)$
- But $h_{liq}(T)=u_{liq}(T)+p_{sat}(T)v_{liq}(T)$, so
	- $h(T,p)\approx h_{liq}(T)+(p-p_{sat}(T))v_{liq}(T)$
- So enthalpy can usually be approximated by $h(T,p)\approx h_{liq}(T)$
- Saturated liquid is at boiling temperature but is not boiling yet -> just begins to boil
### Incompressible substance model
- most liquids and solids are ∼incompressible:
	- $v$ is ~constant
	- $u$ ~depends on 
- for incompressible substances, specific heats are equal:
	- $c_{v}(T)=\left( \frac{\partial}{\partial T}u(T) \right)_{v}=\frac{du}{dt}$
	- $c_{p}(T)=\left( \frac{\partial}{\partial T} u(T)\right)_{v}=\frac{du}{dT}$
- $\Delta u=\int _{T_{1}} ^{T_{2}}c(T)dT$
- $\Delta h=\Delta u+v\Delta p$
## Modeling gasses
- Ideal gas: collection of point-mass particles that do not interact with each other and obey classical (not quantum) mechanics
	- Can use the ideal gas model (1) with most common gases (air, $O_{2},N_{2},CO_{2},CO,H_{2}$); (2) when pressure is low ($p\ll p_{c}$) and/or $T$ is high ($T\gg T_{c}$)
- Compressibility factor: $Z=\frac{pv}{RT}= \frac{p\bar{v}}{\bar{R}T}$
	- If $z=1$, then $pv=RT$
- Assumptions underlying ideal gas model: (1) $pv=RT$; (2) internal energy depends only on temperature: $h=u+pv=u(T)+RT=h(t)$
- Enthalpy depends only on temperature
- Equation of state can take on various forms via definitions $v=\frac{V}{m},\bar{v}=\frac{V}{n},M=\frac{m}{n},\bar{R}=MR$
- Specific heat depends only on temperature
	- Given one specific heat, we can always find the other form with $c_{p}(T)=c_{v}(T)+R$
- In terms of specific heat ratio $K(T)= \frac{c_{p}(T)}{c_{v}(T)}\to c_{p}(T)= \frac{R}{1-1/k(T)},c_{v}(T)= \frac{R}{k(T)-1}$
## Polytropic processes
- As previously stated, polytropic process is quasi-equilibrium process with $pV^n=C$
- $C=p_{1}V_{1}^n=p_{2}V_{2}^n$ so $\frac{p_{2}}{p_{1}}=\left( \frac{V_{1}}{V_{2}} \right)^n$
## Special cases of polytropic processes
- If $n=0$, pressure is constant: $pV^0=c\to p=C$
- As $n\to \infty$, volume becomes constant: $\frac{V_{1}}{V_{2}}=\left( \frac{p_{2}}{p_{1}}^{} \right)^{1/n}\to1$ as $|n|\to \infty$
	- If $n=1$ in a closed ideal gas station, temperature is constant
- Polytropic boundary work for closed ideal gas system: 
$$\int_{V_1}^{V_2} p\,\mathrm{d}V =
\begin{cases}
\dfrac{mR\left(T_2 - T_1\right)}{1-n}, & n\neq 1,\\[6pt]
mRT\,\ln\!\left(\dfrac{V_2}{V_1}\right), & n=1.
\end{cases}$$
- For any closed ideal gas system, $\left( \frac{p_{2}}{p_{1}} \right)^{1-1/n}=\frac{T_{2}}{T_{1}}=\left( \frac{V_{1}}{V_{2}} \right)^{n-1}$
# Practice Exams
