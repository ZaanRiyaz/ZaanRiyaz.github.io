---
title: "White Dwarves: The Chandrsekhar Limit"
modified:
categories: Notes
excerpt: "A brief look at the Chandrasekhar Limit, which tells us whether or not a star will turn out to be a White Dwarf."
tags: []
date: 2020-10-13
toc: true
---
A star at the end of it's lifecycle will become a 'White Dwarf', if it's mass is 1.44 $M_{\odot}$. That is, 1.44 times the mass of the Sun. This is called the Chandrasekhar limit, named after Subrahmanyan Chandrasekhar who calculated it in the 1930s. 

Having done the exercise of re-deriving this limit in an undergrad statistical physics module I took, I thought it would be nice to approach it in the spirit of coming back to some astrophysics after much time with the Composite Higgs.

# Fermions
Elementary particles can be divided into two categories: bosons and fermions. The difference between them is that bosons have integer 'spin' and fermions have half-integer 'spin', where 'spin' is an intrinsic quantum number (examples: electrons are fermions with a spin of 1/2. The Higgs is a Boson with a spin of 0). Fermions follow a very important rule called the Pauli exclusion principle which can be stated as follows,

> "No two fermions share the same quantum numbers".

For instance, if particle A has a quantum number of 1 then another particle B can't share this quantum number because it violates Pauli exclusion.

## Fermi - Dirac Distribution

The Fermi - Dirac distribution tells us about the average number of particles in a particular quantum state labelled as $\vec{k}$:

$$\langle N_{\vec{k}}\rangle = \frac{1}{e^{\beta(E_{\vec{k}} - \mu) + 1}} \tag{1} $$

Here, $E_{\vec{k}}$ tells us the energy of the state $\vec{k}$, $\mu$ is called the energy potential and $\beta = 1/K_{B}T$ where $T$ is the temperature and $K_{B}$ is Boltzmann's constant.

The behaviour of the Fermi - Dirac distribution is quite simple 