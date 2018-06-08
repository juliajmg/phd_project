# EFFECT OF INTERACTION-RULES VARIATION ON COLLECTIVE MOTION SYSTEMS

---

# INTRODUCTION

---

## Collective motion
- Qué es
- Cómo se estudia


### INTRODUCTION
---
## Rules of interaction
- Qué son
- Ventajas adaptativas

### INTRODUCTION
---

# GOALS
- Study the impact of the variation in group and individual interaction-rules:
    - Ordering,
    - Information transfer
    - Decision-making

- Compare emergent behaviors with those observed in animal collectives with flocking behavior.


---

# PRELIMINARY RESULTS

---

## Vicsek model

- Model of self-propelled particles (SPP)
- Vicsek et al. (1995)
- Imitates flocking behavior:
  - Integrates natural perturbations in particles' direction of motion.  

- Parámeters:
Density $\rho$: Number of particles $N$ in a volume "$R^d$" ($d$ is the dimension).
Velocity $v_{0}$
Noise amplitude $\eta$
(FUNCIÓN DE RUIDO)
Order parameter: Average normalized velocity $\phi$,

$$ \phi = \frac{1}{N v_{0}} \left| \sum_{i=1}^{N} \vec{v_{i}} \right| $$

#### PRELIMINARY RESULTS

Note:
Agregar un esquema con partículas.
Describes particles moving at constant velocity.
At each time unit, each particle i changes its orientation depending on the average orientation of its neighbors (neighborhood of radius R_0 centered in i) and a noise term that represents perturbations.
