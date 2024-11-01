# Path Integration
Authors: Nosratullah Mohammadi^1, Maylis Müller^2

^1: University of Geneva

^2: EPFL

The project titled ”Path Integration using Coupled Bump Attractors” is a mini-project undertaken during the
Spring semester of 2024 for the Computational Neuroscience : Neuronal Dynamics class. It involves the implemen-
tation of a circuit capable of integrating the movement of an ant in two dimensions, in order to estimate its current
position at every time step. The project draws inspiration from the navigational behavior of insects, particularly ants,
and aims to simulate the recurrent neural networks involved in path integration.

## Methods
Using the following model for simulating the neurons. The potential hi (in mV) of every neuron i evolves according to the differential equation:
$$
\tau \dot h_i(t) = -h_i + R I_i(t)
$$
where in the remaining we will take R = 1MΩ. Every neuron has an instantaneous mean firing rate ri(t) given by the transfer function g, for which we will use the sigmoid function.

$$
r_{i}(t)=r_{0} g\left(h_{i}(t)\right)=r_{0} \frac{1}{1+e^{-2 \alpha\left(h_{i}(t)-\beta\right)}}
$$
![sigmoid](/figures/0.1.png)
