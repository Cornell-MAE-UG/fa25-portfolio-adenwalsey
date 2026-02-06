---
layout: project
title: Aero Pack
description: Personal aero saddle bag project
technologies: [Autodesk Fusion, 3D Printing]
image: /assets/images/aero 2.png
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
-	Design and fabricate a lightweight, aerodynamic saddle bag that integrates cleanly with a Canyon Ultimate seatpost, minimizes drag, and securely carries essential ride items using a custom CAD model and 3D-printed prototype.
<br>

### Design Requirements
- Minimize frontal and side projected area behind the seatpost.
- Maintain secure mounting under dynamic road vibration.
- Achieve low mass while preserving sufficient stiffness.
- Allow one-handed access to contents.
- Fit common cycling tools.
- Be fully manufacturable via desktop FDM 3D printing.

<div style="display: flex; justify-content: center; gap: 20px;">
  <img src="{{ '/assets/images/aero cad 1.png' | relative_url }}" style="width: 20%;">
  <img src="{{ '/assets/images/aero cad 2.png' | relative_url }}" style="width: 20%;">
  <img src="{{ '/assets/images/aero cad 3.png' | relative_url }}" style="width: 20%;">
</div>

### Key Design Features
- Streamlined and tapered housing to reduce flow separation behind the saddle.
- Integrated rear light mount aligned within wake region.
- Custom saddle-rail clamp geometry for rigid attachment without straps.
- Smooth exterior surfaces with controlled fillets to reduce stress concentrations and drag.
- Modular interface allowing light removal independent of the bag.



### Outcomes:
-	Successfully produced a functional, lightweight saddle bag prototype.
- Achieved a compact, aero-conscious form factor compared to traditional fabric bags.
- Demonstrated secure mounting with no sway during riding.
- Integrated rear lighting without additional mounts or straps.
<br>

### Next Steps
- Conduct CFD analysis to confirm drag reduction, evaluate flow separation, and identify downstream wake region.
- Consider alternative slicing configuration to reduce stress concentrations and mitigate printing failures.








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
