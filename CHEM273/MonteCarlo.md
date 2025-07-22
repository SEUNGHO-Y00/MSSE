# Simulation and Monte Carlo Method

1. The Problem

* many dynamic problems don’t have an analytical solution
  - degradation of a chemical compound A with rate k

* some quantities have singularities → standard simulations are not possible
  - moving particles in a potential U

2. Finding PI

* generating a set of values randomly i.e. repeated random sampling

3. Gillespie Algorithm

* based on 𝑁(𝑡) and 𝝉, calculate the time Δt that elapses until one atom decays

1) draw a random number 𝜌 from a uniform distribution in the interval (𝟎, 𝟏)
2) calculate the time Δt that elapses until the next decay
Δt = −1 /(𝜏*𝑁(𝑡)) * ln 𝜌
3) set 𝑡 ⇾ 𝑡 + Δt and 𝑁(𝑡 + Δt) = 𝑁(𝑡) − 1
4) repeat

4. Metropolis Algorithm

* We can combine the MC method with different ways how to run a simulation

* calculating if a particle changes its state (here locations, velocities and acceleration)
  - If 𝑑𝑈𝑡𝑜𝑡(𝑥, 𝑦)𝐿𝐽 is negative: → always move (a ball always rolls down the hill)
  - If 𝑑𝑈𝑡𝑜𝑡(𝑥, 𝑦)𝐿𝐽 is positive: → calculate the probability to move
