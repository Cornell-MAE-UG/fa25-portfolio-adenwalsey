---
layout: project
title: Bike Trainer Dissection
description: Class project with Graphs
technologies: [CFD concepts, kinematics/dynamics, approximation methods, data collection.]
image: /assets/images/trainer.png
---
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>
<br>

### Objective: 
-	Dissect a system with a fluid mechanical component and understand how it works based on concepts learned from Fluid Mechanics course at Cornell University.
<br>
<br>
<br>
<br>

### Outcomes:
-	Dissected and analyzed fluid mechanics of the impeller in a stationary bicycle trainer housed in silicone-based oil.
-	Calculated drag force, Reynolds number, and mechanical advantage of impeller to evaluate system behavior.
-	Created a video presenting the system’s operations and our findings, including modeling the flow using Navier-Stokes equations and how
-	 the system would change with variations in fluid
properties.
<br>

### Contributions:
- Took system measurements such as impeller length and wheel diameter.
- Used approximations for impeller such as thin-walled, flat plate area, and incompressible/mean averaged/Reynold’s averaged flow to simplify calculations (see calculations below).
- Compared viscosity of oil to other liquids such as 
water and honey to understand why the 
silicone-based oil is the most efficient.




<div style="display: flex; justify-content: center; gap: 20px;">
  <img src="{{ '/assets/images/cracking.png' | relative_url }}" style="width: 40%;">
  <img src="{{ '/assets/images/impeller.png' | relative_url }}" style="width: 40%;">
</div>
<br>

---

<br>

### Calculations:
<br>

##### Engineering Models
- Incompressible flow  
- Mean averaged flow  
- Reynold's averaged flow  


##### Shaft Speed and Reynolds Number Estimation
Ratio of wheel diameter to shaft diameter: $R_D$

$$
R_D = \frac{D_B}{D_S} = \frac{25.5''}{0.353''}
$$

$$
\omega_s = R_D(\omega_w)
$$

$$
\omega_s \approx 1210~\text{rad/s}
$$

$$
Re = \frac{\rho \, \omega_s \, D^2}{\mu}
$$

$$
Re = 47{,}342 \rightarrow \text{Turbulent}
$$


##### Drag Force Estimation

$$
C_D = \frac{F_D}{\tfrac{1}{2}\rho u^2 A}
$$

$$
F_D = \tfrac{1}{2}\rho (\omega R)^2 A C_D
$$

CD for flat plate $\perp$ to flow = 1.98

$$
F_D = 203~\text{N}
$$

$$
F_{D\text{total}} = 203 \times 6
$$

$$
F_{D\text{total}} \approx 1220~\text{N} = 274~\text{lbf}
$$
