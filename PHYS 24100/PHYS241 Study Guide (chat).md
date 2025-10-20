---
Class: "[[PHYS 24100]]"
Type: Study guide
Date: 2025-09-26
tags:
  - exam
  - s1
  - phys241
---
# Study Guide for PHYS 241 (Lectures 1–7)

## Overview of Electric Charge and Coulomb’s Law

### Fundamental concepts

* **Electric charge** – Matter contains positive and negative charges.  Experiments show that charge is **quantised** (the smallest unit is the elementary charge $e$) and is **conserved**; total charge in an isolated system remains constant.  Charge on macroscopic objects results from an imbalance between electrons and protons.
* **Conductors and insulators** – In **conductors**, electrons are free to move, whereas in **insulators** the charges remain bound.  Semiconductors and superconductors fall between these extremes.  When excess charge is placed on an isolated conductor it migrates to the surface; the electric field inside becomes zero.
* **Coulomb’s law** – The electrostatic force between two point charges is 
  $$\mathbf F = \frac{1}{4\pi\epsilon_0}\,\frac{q_1 q_2}{r^2}\,\hat{\mathbf r},$$
  where $r$ is the separation and $\hat{\mathbf r}$ is the unit vector from the source to the test charge.  The force obeys Newton’s third law: charges exert equal and opposite forces.  Coulomb’s law has the same inverse‑square form as Newton’s gravitational law but may be attractive or repulsive.  **Superposition** applies: the net force on a charge is the vector sum of the individual forces from all other charges.

### Electric field as a vector field

* The **electric field** $\mathbf E$ describes the force per unit test charge: $\mathbf E = \mathbf F/q_0$.  It is a **vector field** defined at every point in space.  Multiple source charges create a field that is the **vector sum** of individual fields.  Field lines emanate from positive charges and terminate on negative charges, and the density of lines indicates the field’s magnitude.
* For a point charge $q$, $\mathbf E = (1/4\pi\epsilon_0)\,q\,\mathbf{\hat r}/r^2$.  For an **electric dipole** separated by distance $d$ the far‑field scales as $1/r^3$; the dipole moment $\mathbf p = q\,d\,\hat{\mathbf p}$ points from negative to positive and the torque in a uniform field is $\boldsymbol{\tau} = \mathbf p \times \mathbf E$.

### Problem‑solving strategy for discrete charges

1. Draw a diagram with coordinate axes.  Label known charges, distances and the point where the field/force is sought.
2. Apply Coulomb’s law to each pair of charges.
3. Break vectors into components; sum the components to get the net force or field.
4. Use symmetry whenever possible to simplify directions and magnitudes.
5. Check units and consider limiting cases.

## Continuous Charge Distributions

### Charge densities

For extended objects the total charge $Q$ is represented by small elements $dq$.  Different kinds of densities are defined:

| Density | Symbol | Definition | Example element |
|---|---|---|---|
| **Linear** | $\lambda$ | charge per unit length \([\rm C/m]\) | $dq = \lambda \, dx$ on a rod |
| **Surface** | $\sigma$ | charge per unit area \([\rm C/m^2]\) | $dq = \sigma \, dA$ on a sheet |
| **Volume** | $\rho$ | charge per unit volume \([\rm C/m^3]\) | $dq = \rho \, dV$ in 3‑D region |

### General method for calculating $\mathbf E$

Electric fields from continuous distributions are found by slicing the charge into infinitesimal pieces and summing their contributions via integration.  Slides outline the systematic steps:

1. **Understand the geometry** – Identify symmetry and coordinate axes.
2. **Choose** $dq$ – Express the infinitesimal charge in terms of density and differential length/area/volume.
3. **Calculate** $d\mathbf E$ – Use Coulomb’s law for the element.
4. **Exploit symmetry** – Determine which components cancel; often only one component survives.
5. **Set up the integral** – Integrate over the entire distribution.
6. **Solve the integral** analytically or numerically.
7. **Check limiting cases** – Ensure the result reduces to familiar forms (e.g., point charge) as appropriate.

### Examples

* **Ring of charge** – Along the axis of a uniformly charged ring of radius $R$ and total charge $Q$, the field points along the axis.  After integration the axial component is
  $$E_z = \frac{1}{4\pi\epsilon_0}\frac{Q z}{(z^2+R^2)^{3/2}}.$$
* **Disk of charge** – For a uniformly charged disk of radius $R$ with surface density $\sigma$, the field along the axis at distance $z$ is
  $$E_z = \frac{\sigma}{2\epsilon_0}\Bigl(1 - \frac{z}{\sqrt{z^2+R^2}}\Bigr).$$
  In the limit $z \gg R$ the disk behaves like a point charge (field $\sim 1/z^2$).  As $R\to\infty$ the field approaches $\sigma/2\epsilon_0$, the field of an infinite sheet.
* **Infinite line and plane** – By choosing cylindrical or planar Gaussian surfaces (see Gauss’s law section), one finds that a line of density $\lambda$ produces $E=\lambda/(2\pi\epsilon_0 r)$ radially outward, and an infinite sheet of density $\sigma$ produces a constant field $\sigma/(2\epsilon_0)$ on either side.

## Gauss’s Law and Electric Flux

### Electric flux

The **flux** through a surface is $\Phi_E = \int \mathbf E \cdot d\mathbf A$.  For a closed surface, the outward normal is used.  Slides describe flux qualitatively and with examples.

### Gauss’s law

Gauss’s law states that the net electric flux through a closed surface equals the enclosed charge divided by $\epsilon_0$:
$$\oint_S \mathbf E \cdot d\mathbf A = \frac{Q_{\mathrm{enclosed}}}{\epsilon_0}.$$
It relates the electric field on a closed surface to the total enclosed charge.  Gauss’s law and Coulomb’s law are equivalent.  When combined with symmetry, Gauss’s law can simplify calculations of $\mathbf E$ for highly symmetric charge distributions:

* **Spherical symmetry** – For a point charge or uniformly charged sphere, the field outside behaves like a point charge, and inside a uniformly charged sphere $E \propto r$ until the surface is reached.  Shell theorems follow: (1) a shell of uniform charge attracts/repels an external charge as if all its charge were at the centre; (2) a shell exerts no force on a charge inside.
* **Cylindrical symmetry** – For a long charged line, choose a cylindrical Gaussian surface coaxial with the line.  Only the curved side contributes, leading to $E=\lambda/(2\pi\epsilon_0 r)$.
* **Planar symmetry** – For an infinite sheet of charge, choose a pill‑box Gaussian surface straddling the sheet.  The field is constant and perpendicular, yielding $E=\sigma/(2\epsilon_0)$.  If two conducting plates carry equal and opposite charge, all charge resides on the inner surfaces; the field is $E=\sigma/\epsilon_0$ between plates and zero outside.

### Conductors and Gauss’s law

* Because charges in a conductor move freely, any net excess charge resides on the surface.  Just inside a conductor $\mathbf E=0$; otherwise free electrons would accelerate until equilibrium is restored.  Therefore, the entire conductor (bulk and surface) is at a constant potential.
* When a cavity exists in a conductor, charges on the cavity wall rearrange so that the field inside the material remains zero.  No net charge resides on the cavity walls unless a charge is placed inside.
* At the surface, the field is perpendicular and its magnitude is related to the surface charge density: $E_{\text{surface}} = \sigma/\epsilon_0$.  Areas of high curvature have a higher surface charge density, leading to stronger local fields (useful for lightning rods and electrostatic spraying).

### Shielding and Faraday cages

Because $\mathbf E = 0$ inside conductors, conductive enclosures protect their interiors from external fields.  The lecture demonstrated that a radio stops receiving signals when placed inside a Faraday cage and that a person inside a cage is unaffected by sparks.  The same principle underlies shielded cables and microwave oven walls.

## Electric Potential Energy and Potential

### Work, potential energy and conservative forces

* Work is $W = \int \mathbf F \cdot d\mathbf x$.  For conservative forces (e.g., gravity and electrostatic), work depends only on initial and final positions.  The **work–energy theorem** states that the work done on a particle changes its kinetic energy.
* In electrostatics, the **electrostatic force** is conservative.  The **electric potential energy** of a system is the work required by an external agent to assemble the charges from infinity.
* For two point charges $q_1$ and $q_2$ separated by $r$, the potential energy is
  $$U = \frac{1}{4\pi\epsilon_0}\frac{q_1 q_2}{r}.$$
  If the charges have the **same sign**, $U>0$ because positive work must be done against repulsion; if they have **opposite signs**, $U<0$ because work is done against attraction.  For systems of more than two charges, sum the pairwise contributions.

* To assemble multiple charges, bring them in from infinity one at a time.  No work is done to place the first charge.  Bringing the second charge into the field of the first requires work $k q_1 q_2/r_{12}$.  Bringing the third charge requires work against the fields of both charges, and so on; summing all contributions yields the total potential energy.

### Electric potential and potential difference

* The **electric potential** $V$ at a point is the potential energy per unit charge: $V = U/q$.  Potential is a scalar field; it depends only on the sources, not on the test charge used to probe it.  Only differences in potential have physical meaning.
* By convention, the potential at infinity is set to zero.  For a point charge, $V(r) = (1/4\pi\epsilon_0)\,q/r$; it decreases as one moves away from a positive charge.
* The **potential difference** between two points is the negative of the work done by the electric field per unit charge to move between them.  Because the electrostatic force is conservative, this difference is **path independent**.  The line‑integral form is
  $$V(b) - V(a) = -\int_a^b \mathbf E \cdot d\mathbf l.$$
  This is the basis for relating $\mathbf E$ and $V$.
* Slides emphasise that the electric field points in the direction of steepest decrease of potential and its magnitude equals the slope.

### Relationship between $\mathbf E$ and $V$

Taking the gradient of the potential recovers the field:
$$\mathbf E = -\nabla V = -\left(\frac{\partial V}{\partial x}\hat{\mathbf i} + \frac{\partial V}{\partial y}\hat{\mathbf j} + \frac{\partial V}{\partial z}\hat{\mathbf k}\right).$$
Slides list these relations explicitly.  When given a potential function, differentiate to find $\mathbf E$.  Conversely, integrating $\mathbf E$ along a path yields potential differences.

### Equipotential surfaces

An **equipotential** is a locus of points where $V$ has the same value.  Because moving along an equipotential requires no work, the electric field is always **perpendicular** to equipotential surfaces.  For example, concentric spheres around a point charge are equipotentials; planes perpendicular to the field of a uniform sheet are equipotentials.  Inside a conductor, the entire volume is at a constant potential.

## Potentials from Continuous Charge Distributions

The potential at a point due to continuous charge can be obtained by integrating contributions from small elements:
$$V = \frac{1}{4\pi\epsilon_0}\int \frac{dq}{r}.$$
Examples:

* **Ring** – At a point on the axis, $V = (1/4\pi\epsilon_0) Q / \sqrt{z^2 + R^2}$.  Differentiating this expression with respect to $z$ recovers the axial field derived earlier.
* **Disk** – For a disk of radius $R$ and surface density $\sigma$, the potential on the axis is
  $$V(z) = \frac{\sigma}{2\epsilon_0}\left(\sqrt{z^2 + R^2} - z\right).$$
  Differentiating yields $E_z = \sigma/(2\epsilon_0)\bigl(1 - z/\sqrt{z^2+R^2}\bigr)$.  Slides show that both the “integrate $dq$” method and the “integrate $E$” method produce the same result.
* **Infinite sheet** – For a uniformly charged infinite sheet, the potential varies linearly with distance: $V(x) = V_0 - \sigma x/(2\epsilon_0)$ for $x>0$ and $V(x) = V_0 + \sigma x/(2\epsilon_0)$ for $x<0$.  The linear drop enables potential differences to be used to accelerate charges; the lecture demonstrated lighting a fluorescent bulb by holding it near a Van de Graaff generator and aligning it across the potential gradient.

## Homework Concepts and Typical Problem Types

The first homework focused on applying these ideas.  Common themes included:

* **Vector addition of forces** – Determining the net force on a charge due to multiple other charges by decomposing vectors and summing components.  Superposition was emphasised; exchanging the positions of charges changes the direction of the net force but may not change its magnitude.
* **Net zero force or field** – Identifying points where the electric field (or force on a test charge) is zero.  This occurs when contributions from multiple charges cancel; symmetry often helps locate such points.
* **Charge calculations** – Converting masses of substances to total charge using Avogadro’s number and the number of protons/electrons per atom.  For example, determining the total positive charge in 1.9 kg of carbon requires calculating the number of carbon atoms and multiplying by the charge of the protons.
* **Locating charges** – Solving for the location or magnitude of a charge such that the net force on another charge is zero, using vector relations from Coulomb’s law.
* **Charges on a semicircle** – Calculating the force on a central charge due to charges uniformly spaced around a semicircle.  By symmetry, components perpendicular to the diameter cancel; the remaining components add.
* **Energy and electric fields** – Relating electric field strength to changes in kinetic energy: a uniform field does work on a charged particle, changing its speed over a given distance.  In one homework problem, finding the field needed to stop a beam of protons in 2 m uses the work–energy theorem.  Increasing the initial speed requires a larger field; replacing protons with electrons (lighter mass and opposite charge) alters the field direction and magnitude.
* **Linking force, field and potential** – Recognising that $\mathbf F=q\mathbf E$ and $V=U/q$, so problems asking for force or potential may be solved by finding the appropriate field or energy.

## Study Tips

1. **Master vector basics.**  Many problems involve decomposing vectors, drawing components and applying trigonometry.
2. **Use symmetry.**  Look for geometrical symmetry (circular, cylindrical, planar) to simplify integrals or recognise that certain components cancel.
3. **Check limiting cases.**  After obtaining a field or potential, consider extreme limits (very far away, or at the centre) to ensure the expression behaves as expected.
4. **Keep track of signs.**  Positive and negative charges produce fields in opposite directions; potential energy can be positive or negative depending on whether charges attract or repel.
5. **Draw equipotential surfaces and field lines.**  Visualising how field lines intersect equipotentials helps predict the direction of motion of charges.
6. **Understand the physical meaning.**  Potential energy reflects stored ability to do work; potential difference drives charge motion; the electric field is the mediator of forces.
