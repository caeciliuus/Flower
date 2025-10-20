---
Class: "[[ME 20000]]"
Type: Lecture notes
Date: 2025-10-15
tags:
  - 25-26
  - s1
  - lecture
  - me200
---
- Spontaneous heat flow from hold -> hot is unphysical, but satisfies conservation of mass and the first law
	- 2nd Law provides a way to rule out unphysical processes and ways to identify and quantify inefficiencies
- A **reservoir** is a system whose $\Delta T=0$, even if $Q\neq0$ - e.g SLVM
![[Pasted image 20251015163928.png|right|400]]
- **Clausius Statement:** no cycle can have the sole effect of heat transfer from a colder -> warmer reservoir
- **Kelvin-Planck Statement:** no cycle can receive energy via heat transfer from a single reservoir and produce net work
	- "power cycles must produce 'waste heat'"
- While the statements sound different, C and KP are equivalent (see right)
- **Reversible process:** after its run, system and surroundings can be returned to their initial states
	- All real processes have irreversibilities like friction, electric resistance, unresistricted expansion of fluid to lower pressure, substances of of different states/compositions mixing
- Heat transfer $\delta Q$ into system and work $\delta W$ done by system can cause change in internal energy: $dU=\delta Q-\delta W$
- **Entropy** ($kJ/K$): heat transfer $\delta Q$ into system at system temperature $T$ and entropy generation $\delta\sigma$ ($\geq0$) within ysstem cause change in system entropy: $dS=\frac{\delta Q}{T}+\delta\sigma$
	- for any isolated system, $dS=0$ is reversible, $dS>0$ is irreversible
	- Systems at $T_{a}$ and $T_{b}$ exchange heat ~reversibly if $T_{a}\approx T_{b}$
- Clausius Inequality $\frac{Q_{in}}{T_{in}}\leq \frac{Q_{out}}{T_{out}}$ only holds true if process is reversible, considering cycle where system absorbs $Q_{in}>0$ from reservoir with $T_{in}$ and emits $Q_{out}>0$ to reservoir with $T_{out}$
	- $W>0$ if $\frac{Q_{h}}{Q_{c}}>1$