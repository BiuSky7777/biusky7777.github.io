---
layout: archive
title: "Projects"
permalink: /projects/
author_profile: true
---

Here are some project write-ups, completed either in collaboration with amazing peers. While the results may not be novel enough for publication, I hope they can still offer a bit of inspiration by:
* Highlighting directions that didn't work out.
* Verifying and confirming established results numerically.
* Demonstrating how elegant theorems/algorithms can be casually applied to similar problems and senarios.

***

[**Differentially Private SGD with Curriculum Learning**](https://github.com/BiuSky7777/biusky7777.github.io/blob/master/_projects/dp_sgd.pdf)
* We incorporated curriculum learning into stochastic gradient descent with differential privacy to better balance data privacy and model performance.
* We experimented different noise injection schedules (noise curriculum) and re-arranged sample ordering (sample curriculum) when training a deep learning model.
* Results show promising accuracy improvements with noise curriculum, but little evidence of performance gains from sample curriculum.

[**Differentiable Pulse-Based Variational Quantum Eigensolver**](https://github.com/BiuSky7777/biusky7777.github.io/blob/master/_projects/pb_vqe.pdf) [(PPT)](https://github.com/BiuSky7777/biusky7777.github.io/blob/master/_projects/quantum_diff_pre.pdf)
* We proposed a polynomial parameterization method for pulse-based VQE, reducing parameters from $M \times Q$ to $n \times Q$ (where $M$ is the number of time segments and $Q$ is the number of qubits), along with an efficient analytic gradient formula that lowers computational cost to $O(1)$ compared to $O(M)$ in finite difference methods, though it applies to a limited set of pulse sequences.
* Implementations confirm the proposed pulse-based VQE is fast, but we cannot reach the theoretical
minimum due to pulse sequence ansatz choices, which is limited by our gradient calculation method.

[**Quantum Dynamic Programming**](https://github.com/BiuSky7777/biusky7777.github.io/blob/master/_projects/quantum_dynamic_programming.pdf)
* We applied the divide-and-conquer dynamic programming approach [ABIKPV18](https://arxiv.org/abs/1807.05209) to NP-hard problems like graph coloring, minimum clique cover, and minimum dominating set, achieving time complexity improvements from $O(2.4423^n)$ classically to $O(1.9140^n)$ quantumly on certain instances.
* We highlighted that for problems like the dominating set and minimum vertex cover, dynamic programming underperforms compared to direct application of Grover's algorithm on classical brute-force methods, suggesting the need for new approaches to utilize dynamic programming effectively.

[**Towards Physically-Consistent, Chaotic Spatiotemporal Dynamics with Echo State Networks**](http://ceur-ws.org/Vol-2964/article_199.pdf)
* This study investigates the use of echo state networks (ESNs) for time-series forecasting in chaotic physics.
* We compare a basic ESN with two physics-informed variants on the Lorenz attractor and then test the ESN on a large-scale atmospheric model and a real-world weather dataset. 
* Results show that a well-tuned traditional ESN can outperform physics-informed methods. While the ESN accurately predicts the global evolution of atmospheric primitive equations over short periods (~67 hours), it struggles with real-world data.
* Accepted to AAAI Spring Symposium Series 2021 

[**Investigation of Area Law for Local Hamiltonians**](https://github.com/BiuSky7777/Reed2020-Thesis/blob/master/Paper/My_Final_College_Paper.pdf)
* We implemented generic and RRG algorithms to find ground states of local Hamiltonians, including Heisenberg and AKLT models.
* We verified an area law for von Neumann entanglement entropy in the XXZ model for up to $14$ qubits.
* We confirmed exponential Schmidt coefficient distribution up to 13 qubits and predicted the slope for $14$ qubits, with discrepancies within $0.1$.
