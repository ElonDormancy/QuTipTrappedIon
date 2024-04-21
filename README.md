# Trapped Ion with QuTip
Repository to store the basic code of trapped ion via qutip(https://github.com/qutip)

# Homework 2024

## Part I
### Two level system, Rabi flopping and Ramsey experiment

Deduce the final probability of excited state after a Ramsey sequence as followed slides from zihan's JC
### Decoherence, Spin echo, composite pulse

- What kind of noise can be eliminated by spin echo?
- In the addressing error model, compare the error correction effect of composite pulse
sequences SK1, N2, B2 for different values of base errors
- In the amplitude error model, compare the error correction effect of composite pulse
sequences SK1, N2, B2 for different values of base errors

### Adiabatic theorem, Landau-Zener transition, Counter-diabatic drive
Based on AE scheme，calculate the waveform of adiabatic passage with CD-drive Hamiltonian


## Part II 

### Raman Transition Simulation

Derive the effective results to drive two-photon Raman transitions and use the Qutip to calculate the time-evolution of the raman transition with/without deca

### Spin-Motion Coupling

We will now investigate the generation and characterizing of nonclassical motional states in a trapped ion system as described by [Meekhof et al. in PhysRevLett. 76.1796 (1996).]
The authors generate the thermal, Fock, coherent, and squeezed state of motional of a single Be+ ion. Then they detect the state of atomic motion by observing the evolution of the atom’s internal levels under the influence of a JCM-type interaction.
 
Reproduce the four population plots of four different motional states in this reference as closely as possible and learn how they generate these states.
 
Hint: https://iontrap.umd.edu/wp-content/uploads/2012/12/Experimental-Preparation-and-Measurement-of-the-State-of-Motion-of-a-Trapped-Atom.pdf


We can also just apply a multi-frequency laser field, with each frequency component resonant with one of the transitions to generate the coherent state and squeezing
state.[ Kienzler D, Lo H Y, Keitch B, et al. Science, 2015, 347(6217): 53-56.]
 
Reproduce the Figure 2 to learn the technology of how to generate the coherent state and squeezing state by simultaneously apply the multi-frequency laser field.

# Homework 2023

## Problem 1
Rabi oscillation
- Use Qutip to calculate the Rabi oscillation under a perfect drive, plot the
following graphs (with the correct labels): 1. population evolution with time; 2.
Fixed time, population vs. scanning frequency; 3. Evolution on the Bloch sphere.
- Suppose we have 20% and 50% amplitude error, respectively, re-plot the
evolution on the Bloch sphere

## Problem 2
- Plot the spin evolution under a perfect Ramsey experiment
- Suppose during the free evolution, we have random phase shifts that varies from
shot to shot, but is fixed in a single experiment (for example caused by slowly
changing magnetic field for a Zeeman sensitive qubit). Take a uniform
distribution between [0, π/6] and average over 100 shots, how much does the
Ramsey contrast decay?
- Numerically simulate how spin echo can remove this (although very ideal)
perturbation. Show it on the Bloch sphere.

## Problem 3
Composite pulse sequence vs. Counter diabetic driving
- Take an SK1 pulse sequence for example, and we want to flip the qubit from up
to down. Calculate the qubit evolution with SK1 sequence and CD drive (e.g.
Alberly-Elden scheme mentioned in our journal club), plot them on the bloch
sphere.
- Suppose we have 20% and 50% amplitude error, respectively, re-plot the
evolution on the Bloch sphere.

## Problem 4
We will now investigate EIT cooling as described by Morigi et. al. in Phys. Rev. Lett.
85, 4458 (2000). This paper is also available at arxiv.org/abs/quant-ph/0005009.

Reproduce the plot in Fig. 3 of this reference as closely as possible. You do not have to
reproduce the inset. Reproduce both their Monte-Carlo result (instead using our master
equation approach) as well as the rate equation result described in the paper. You may
assume that the spontaneous emission is equally likely to cause decay into either ground
state. This simulation will also take some time to run, this time due to the relatively large
Hilbert space necessary to describe the problem. If it takes too long, feel free to reduce the
initial number of motional quanta in order to reduce the size of the Hilbert space.

Hint 1: Make sure to start with a thermal state as the initial motional state.

Hint 2: Pay specific attention to the Lamb-Dicke parameters!

## Problem 5
- Derive the effective results to drive two-photon Raman transitions.

- Write code to verify that the adiabatic elimination procedure is valid, assuming we start in the
|0⟩ state

## Problem 6
We will now investigate the generation and characterizing of nonclassical motional states in
a trapped ion system as described by Meekhof et al. in PhysRevLett. 76.1796 (1996). The
authors generate the thermal, Fock, coherent, and squeezed state of motional of a single Be+
ion. Then they detect the state of atomic motion by observing the evolution of the atom’s
internal levels under the influence of a JCM-type interaction.

Reproduce the four population plots of four different motional states in this reference as
closely as possible.