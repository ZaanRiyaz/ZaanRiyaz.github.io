---
title: "White Dwarves: The Chandrsekhar Limit"
modified:
categories: Notes
excerpt: "A brief look at the Chandrasekhar Limit, which tells us whether or not a star will turn out to be a White Dwarf."
tags: []
date: 2020-10-13
toc: true
---
A star at the end of it's lifecycle will become a 'White Dwarf', if it's mass is less than 1.44 $M_{\odot}$. That is, 1.44 times the mass of the Sun. This is called the Chandrasekhar limit, named after Subrahmanyan Chandrasekhar who first calculated it in the 1930s. 

Having done the exercise of re-deriving this limit in an undergrad statistical physics module I took, I thought it would be nice to approach it in the spirit of coming back to some astrophysics after much time with the Composite Higgs.

# Fermions
We can begin by thinking of the two branches of elementary particles: bosons and fermions. The difference between them is that bosons have integer 'spin' and fermions have half-integer 'spin', where 'spin' is an intrinsic angular momentum quantum number (examples: electrons are fermions with a spin of 1/2. The photon is a boson with a spin of 1). Fermions follow a very important rule called the Pauli exclusion principle which can be stated as follows,

> "No two fermions can exhibit the same quantum numbers in a quantum system".

For instance, if particle A has quantum numbers (1,1,1) then another particle B can't have quantum numbers (1,1,1) because it violates Pauli exclusion. Anything else is permitted.

## Fermi - Dirac distribution

The Fermi - Dirac distribution tells us about the average number of particles in a particular quantum state. If we label these states as $\vec{k}$, the Fermi - Dirac distribution is:

$$
    \langle N_{\vec{k}}\rangle = \frac{1}{e^{\beta(E_{\vec{k}} - \mu) + 1}} 
\tag{1} 
$$

Here, $E_{\vec{k}}$ tells us the energy of the state $\vec{k}$, $\mu$ is called the energy potential and $\beta = 1/K_{B}T$ where $T$ is the temperature and $K_{B}$ is Boltzmann's constant.

The behaviour of the Fermi - Dirac distribution is quite simple at low temperatures. Lucky for us, this is the regime that we're interested in.

$$
    \langle N_{\vec{k}}\rangle \longrightarrow 
    \begin{cases}
        1 \quad ; \quad E_{\vec{k}} \quad > \quad \mu\\
        0 \quad ; \quad E_{\vec{k}} \quad < \quad \mu
    \end{cases}
\tag{2}
$$

What this means is that a quantum state is either occupied, or not. That is, the states above an energy of $\mu$ is *unoccupied* although states below this energy are *occupied*. At $T = 0$, we will have $\mu(T) = E_{\vec{k}}$. This constant energy is called the 'Fermi energy' $E_{F}$ and it allows us to define the Fermi momentum $p_{F}$:

$$
    E_{F} = \frac{p^{2}_{F}}{2m}
\tag{3}
$$

What all of this means is that at low energies, the particles will have low momenta. However, recall that Pauli exclusion prevents the particles from all crowding the lowest momentum state. If the next lowest energy state is available, it gets occupied by particle and so on until we reach an energy of $E_{F}$. This is a degenerate fermion gas and it serves as a good model for a White Dwarf which we can think of as being a degenerate electron gas.

## Energy of a degenerate fermion gas

For this, we're going to have to use some machinery from statistical physics.

First, we can calculate the total number of fermions using the 'density of states':

$$
    \tilde{E}(E) = g\frac{4\pi\sqrt{2}V}{(2\pi\hbar)^{3}}m^{3/2}E^{1/2}
\tag{4}
$$

The number of fermions $\langle N \rangle$ is then:

$$  \begin{align}
    \langle N \rangle &= \int_{0}^{\infty} \tilde{E}(E) \langle N_{\vec{k}} \rangle dE \\
    &= g \frac{V}{(2\pi\hbar)^{3}}\bigg(\frac{4}{3}\pi p^{3}_{F}\bigg)
    \end{align}
\tag{5}
$$

Similarly, the total energy $\langle E \rangle$ can be found using the density of states (again):

$$
\begin{align}
\langle E \rangle &= \int_{0}^{\infty}\tilde{E}(E)E dE \\
&= \frac{3}{5}\langle N \rangle E_{F}
\tag{6}
\end{align}
$$
