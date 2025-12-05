# PHYS 338 – Homework 3  
## Overall Idea

This project studies a **classical interacting gas** and connects the microscopic interaction
between particles to the **macroscopic equation of state** and the **liquid–gas critical point**.   

In practice, we:

1. **Model the interaction**  
   Replace the realistic Lennard–Jones potential by a **square-well potential** (hard core + finite-range attraction). This keeps the essential physics (repulsion + attraction) but is easier to treat.

2. **Use cluster / virial expansion**  
   Expand the thermodynamics of the gas in powers of density using **Mayer clusters** and obtain the **virial coefficients** \(a_2(T)\), \(a_3(T)\), which encode how interactions modify the ideal-gas behavior.

3. **Compute coefficients**  
   - \(a_2(T)\) (second virial coefficient) is computed **analytically** from the square-well potential.  
   - \(a_3(T)\) (third virial coefficient) is computed **numerically**, via a Monte Carlo “Mayer sampling” of three-particle configurations.

4. **Locate the liquid–gas critical point**  
   Insert \(a_2(T)\) and \(a_3(T)\) into the **truncated virial equation of state**.  
   From this approximate EOS we extract the **critical temperature, density, and pressure** of the liquid–gas transition and study qualitatively how they depend on the strength/range of the attraction.

In short:  
**Microscopic potential → virial coefficients → approximate EOS → liquid–gas critical point.**
