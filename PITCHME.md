# EFFECT OF INTERACTION-RULES VARIATION ON COLLECTIVE MOTION SYSTEMS

---

# INTRODUCTION

---
## Collective motion

@ul[brighten]
- Similar individual units that **interact** by adjusting their speed, direction of motion and distance to each other, to achieve a coherent group displacement.

- No central control: self-organization.

- The interactions are central in order for different “phases” to emerge: disorder vs. order.

- Observed in a wide range of biological systems.
@ulend

Note:
- Collective motion is a type of behavior that consists of similar agents interacting in such a way that they achieve a coherent group displacement. By coherent i mean they adjust their speed, direction of motion and distance to each other to achieve cohesion and synchronization.

- This is done without any central control, i.e. the system self-organizes.

- From the way agents interact, different phases can emerge: from disorganized aggregations to coordinated and polarized groups.

- Moving collectively endows with adaptive properties to individuals, specially on foraging (like finding food more rapidly), and in anti-predation strategies (like, the dilution effect, that decreases individuals probability of being taken by a predator as group size increases, or the many-eyes effect that increases the probability of detecting a predator more rapidly). And due to this adaptive advantage collective motion is observed in a wide range of biological systems; including bacterial colonies, social insects, fish schools, bird flocks and human crowds.

---
## The study of collective motion
@ul[brighten]
- Universality of the phenomenon.
@div[left-70]
- Theoretical approaches
  - Models of self-proppelled particles (SPP).
  - Variation of the rules of interaction.

- Experimental approaches
  - High precision data of animals on the move.

@divend

@div[right-30]
![Video](https://www.youtube.com/embed/Y-5ffl5_7AI)
@divend

@ulend
Note:
- The underlying fundamental principles of collective motion are usually generalized, and therefore nearly independent of the specific details relative to the behavior of individual components, so they are transferable between systems of different nature. This characteristic is known as universality, and coupled with the many technological applications inspired by collective models, has attracted the attention of statistical physicists and theoretical biologists, as well as experimental scientists.

- In theoretical approximations, the mechanisms by which local interactions between agents generate emergent global patterns is investigated with models of self-propelled particles with interaction rules that can be varied.

- In experimental approaches, the advances in tracking and image technologies have enabled to obtain high precision data of animals on the move and make and accurate analysis of individual behavior.

- With this data, it is possible to compare the observations with simulated data results, and infer the underlying mechanisms of communication in collective motion events.


---
## Rules of interaction

- Flexibility in collective decision-making and information transfer processes.

- Source of diversity of structures and dynamics observed in nature.

- Individual and global variations.

Note:
- The different ways in which individuals interact give flexibility to a group in decision-making and information transfer processes. They seem to be the source of the diversity of structures and dynamics of collective motion observed in nature. In recent theoretical and experimental works, these differences have been explored, and it has been shown that animals can be subject to both behavioral group and individual variations.

+++
@div[left-50]
- GROUP VARIATION:
  - Changes in the frequency and force of interactions.
  - External perturbations or internal states.  
  - Group's capacity to exhibit multiple stable collective states.
@divend

@div[right-50]

- INDIVIDUAL VARIATION:
  - Difference in the rules of interaction within a group.
  - Internal states, body-size, information or experience disparities.
  - Emergence of leader-follower dynamics.

@divend


Note:
Global variations

- Group variation refers to changes in the frequency and the force by which individuals interact (By force i mean individuals' probability of responding to the movements of their neighbors), without changing the rules of interaction *per se*.

- Group variation can occur as a response to an external perturbation, to internal states, or to different stages of development.

- This variation expresses in groups' capacity to exhibit mutiple stable collective states: swarming to schooling to milling.

Individual variations

- Individual variation expresses in the difference in the rules of interaction within a group.

- This can be a consequence of factors that affect the preferred individual's speed and direction (different body sizes, specific internal states) or to intrinsic differences in their behavior (more experiences individuals, familiarity, socially dominant) that change attention an individual puts on their neighbors in decision making processes.

- Individual variation often causes the emergence of leader-follower dynamics (i.e. variations in individuals' probability to follow others).

These variations are relevant to understand which strategies groups can adopt to transfer information and endow some members with greater weight in the collective decision-making.

---

## GOALS
@ul[brighten]
- Study the impact of the variation in group and individual interaction-rules:

    - Ordering
    - Information transfer
    - Decision-making

- Compare emergent behaviors with those observed in animal collectives with flocking behavior.
@ulend

+++


---

# PRELIMINARY RESULTS

---?image=Vicsek_dynamics.png&position=right&size=35%

## @color[#324851](Vicsek model)

- Model of self-propelled particles (SPP).  

- Vicsek et al. (1995).  

- Integrates natural perturbations in   
the direction of motion.  


Note:
The model describes the dynamics of a collection of SPPs moving at a constant velocity, and at each time unit, each particle $i$ changes its orientation depending on both the average orientation of its neighbors (defined by a neighborhood of radius $R_{0}$ centered on $i$) and a noise term representing perturbations.

---

### Parameters:

- **Density $\rho$**: Number of particles $N$ in a volume $R^d$.

- **Velocity $v_{0}$**

- **Noise amplitude $\eta$**: white noise uniformely distributed in $[-\pi , \pi]$

- **Order parameter** $\phi$: Average normalized velocity,

`$$ \phi = \frac{1}{N v_{0}} \left| \sum_{i=1}^{N} \vec{v_{i}} \right| $$`

---

## Phase transitions in the Vicsek model

First order vs. Second order as a function of $\eta$

@div[left-50]
<span style="font-size:0.6em; color:grey">Vicsek et al. 1995</span>
![Vicsek1995](phi_vs_eta_Nvariable.png)

@divend

@div[right-50]
![Chate2008](FirstTransitionEvidence.png)
<span style="font-size:0.6em; color:grey">Gregoire and Chaté, 2008</span>
@divend

Note:
Estudiar transiciones de fase y la diferencia entre los dos estudios.

---

### Phase transition as a function of particles' velocity

- **Fish collectives**: Higher average polarization at higher swimming speeds.

@color[blue]((Gautrais2012; Tunstrom2013, Rieucau2014))

@div[left-50]
![Video](https://www.youtube.com/embed/xYl4m0xFcCU)  
@divend

@div[right-50]
![Video](https://www.youtube.com/embed/SIg5d_mi92k)
@divend

Note:
Buscar rangos de velocidades en peces.

---?image=PONERIMAGEN&position=right&size=35%

## @color[purple](¿Is it possible to reproduce the velocity-dependent disorder-to-order phase transition in a model as simple as the Vicsek model?)

---?image=BOXES_IMAGE.PNG&position=right

### Our simulations

#### Computational optimization of the Vicsek model

- System $L^2$ divided in boxes of size $R_{0} = 1$, and each particle is assigned to a given box. <span style="font-size:0.6em; color:grey">(Ginelli et al. 2016)</span>


- First the sum of particles' orientation for each box, and update their positions aftewards.  

+++

#### Simulations

Changes in the time-average order parameter $\phi$ as particles' velocity is increased.

  - N = 10,000
  - $\rho$ from 0.1 to 2
  - Fixed $\eta$ value

---?image=eta_vs_phi_v00.05a10.png&position=right&size=48%

### To fix $\eta$

- Values of $\eta$ where disorder   
and order states are observed:

  - $\eta$ = 0.3, 0.4, 0.5 and 0.6

---?image=Phi_vs_v0a5_vs_rhoa2_eta03a06_surface_plot_big.png&position=right&size=35%
### Changes in $\phi$ by changing $v_{0}$ and $\rho$

- **Disorder-to-order phase transition**

- As $\eta$ is increased, the transition
ocurrs at higher $v_{0}$ and $\rho$ values.


Note:
Hacer análisis de por qué ocurre esto!
Anotar los valores de eta en cada una.

For each $\eta$, a value of $\rho$ was chosen where a transition was observed.

---?image=Phi_vs_v0_rho01a1_eta03a06_big.png&position=right&size=50%

### Nature of velocity-induced phase transition

@div[left-50]
@ul[brighten]
- For each $\eta$, a value of $\rho$ was chosen where a transition was observed.

- After a $v_{0}$ threshold value, a phase transition compatible with a **first-order transition** is observed.
@ulend
@divend

Note:
Which means that with little increase in velocity, theres an increase of factor 10 in the average polar order?

+++

A rapid increase in polarization when a critical velocity is reached would be an advantaje for fish groups, specially for predation risk avoidance.


Note:
The relation between ordering and velocity in fish has been thought of as an adaptive trait to collectively respond to changing environmental conditions.

Being able to rapidly increase group polarization by reaching a critical velocity value would be an advantaje for the group, specially in predation risk avoidance.

Even in the simplest model, order is achieved by increasing the system velocity.

---
#### FUTURE WORK

- Study the velocity induced phase transition in fish



@div[left-50]
@ul[brighten]
- Study the velocity induced phase transition in fish
  - Experimental data of zebrafish (*Danio rerio*): swarming and schooling behaviors.
@ulend
@divend

@div[right-50]
![igb_logo](igb_logo.png)
@divend

+++

- Explore the effect of increasing the velocity of only a fraction of particles on the disorder-order phase-transition.

  - ¿Adaptive strategy in natural systems?
DIBUJO BONITO

Note:
FOTO DE ZEBRAFISH
Poner logo de Research Group in Recreational Fisheries, Fish Ecology and Human Dimensions at the Leibniz-Institute of Freshwater Ecology and Inland Fisheries, or as a collaboration with the Research Group on Adaptive Behaviour and Interaction of the University of Barcelona.
* As a way of saving energy but still respond efficienty
to perturbations.
---

## Kilobots
- Simple low-cost swarm robot by the Self-organizing Systems Research Group at Harvard University.

CARACTERÍSTICAS Y FOTO

+++

Setup del overhead controller, kilobots y KiloGUI

---

- Kilobots have been used to study:

1. Collective decision-making
2. Space exploratin and eficiency in information transfer
3. Collective transport of objects.

FOTOS Y VIDEOS DE LOS ESTUDIOS: Valentini2016, Dimidov2016 Rubenstein2013

---

### GOAL

- Implement and vary collective motion interaction-rules on kilobots to study leader-follower dynamics, and their impact on information transfer and collective decision-making processes.

- Relate their behavior with those of animal collectives, and on the other

- Contribute with collective algorithms with which robots swarms can efficiently fulfill complex tasks.


---
#### LOCALIZATION BY DISTANCE SENSING

- Kilobots rely only on distance measuring to obtain relative positions and orientations of nearby robots.
- They need information to collectively move.

---

### REACH ALGORITHM

Purpose: For kilobots to follow each other, no matter their initial configuration.

#### TRILATERATION
-

FIGURA 5: mejorarla para enseñar como se resuelve la ambiguedad, y luego como se acerca a el.
![](reach_algorithm.png)
Kilobot B localization of reference kilobot A by trilateration using $d_{t-1}$, $d_{t}$ and the distance kilobot B moved from t-1 to t. $\beta$ angle is also shown.

---

#### RANDOM-WALK-BASED SEARCH

- First stage of implementation:
- Choosing among six possible turning angles:
  - poner los ángulos
  - Hacer dibujo de esto.

---

### KILOMBO

- C-based kilobots simulator.
- Efficient hypothesis testing.

---

VIDEOS DE ROBOTS CON ALGORITMOS, Y DIBUJO DE LO QUE FALTA.

---

### FUTURE WORK

- Mantain minimum distances among neighoring kilobots while moving collectively.

- Implement leader-follower dynamics and compare information transfer and decision-making effiency on the direction of motion for different dynamics.

---
### REFERENCES

bla bla bla
