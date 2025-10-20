---
Class: "[[ME 20000]]"
Type: Lecture notes
Date: 2025-10-15
tags:
  - s1
  - 25-26
  - me200
  - lecture
---
- **Nozzles** increase flow velocity: $\dot{r}_{out}>\dot{r}_{in}$ and decrease pressure (fluids like to move from high -> low pressure)
	- Typical assumptions: steady state, 1D flow, $\Delta PE=0$, no boundary/shaft/electrical/etc work
- **Turbines** change the state of a working fluid to produce power
	- Typical assumptions: steady state, 1D flow, $\Delta PE=\Delta KE=0$
	- If $Q=0$, $\dot{W}=\dot{m}(h_{in}-h_{out})$
- **Compressors and pumps** are 'backwards turbines', consume power to change state of working fluid -> workiong fluid is gas in compressors, liquid in pumps
	- Typical assumptions: steady state, 1D flow, $\Delta PE=\Delta KE=0$
- **Throttles** decrease $p_{fluid}$ by resitricting flow -> *often* reduces temperature
	- Typical assumptions: steady state, 1D flow, $\Delta PE=0$, no boundary/shaft/electrical/etc work, $Q=0\to \frac{1}{2}(r_{in}^2-r_{out}^2)=\Delta h$
	- Often velocities are ~equal up/downstream, so $h_{in}=h_{out}$, called **isenthalpic**
- Real machines combine multiple pieces of equipment -> we can analyze these machines by breaking them into subsystems
	- Choosing appropriate system boundaries can simplify analysis 