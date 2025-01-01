---
layout: research
title: 'Quantum Inspired Super-resolution'
# author: peteryang
tags: [researches]
img: quantum-metrology-quest.png
display-order: 1
description: >
---

Advisor: Dr.David Arvidsson (Hitachi, University of Cambridge)

Please see the repository for the work [here](https://github.com/AprilSweettooth/Bayesian/tree/main) and the [manuscript](https://www.overleaf.com/read/qxbjvpfmxjbx#620593).

# Summary of the work

Rayleigh’s curse arises when the distance between closely spaced photon sources decreases beyond Rayleigh’s
limit, causing a loss of information regarding their separation. Recent advancements in mode decomposi-
tion methods, such as SPADE (Tsang et al. (2016)) and SLIVER (ham et al. (2017)), have demonstrated
both theoretically and experimentally their superiority over direct imaging, nearing the true quantum lim-
its for resolving two sub-Rayleigh sources. However, the quantum advantage of these methods diminishes
in the presence of a weak secondary source, and the measurement crosstalk between different spatial modes
raises questions about the experimental feasibility.

## Incoherent Estimation

The first part of this study addresses these challenges using Quantum State
Discrimination. I tackle the problem of estimating the separation between bright and dim photon sources
using Adaptive Hypothesis Testing. Initially, I propose a spatial parameter smaller than the actual trans-
verse separation. Based on this estimator, I developed a measurement strategy. Using the measurement
outcome, I perform Maximum Likelihood Estimation to construct the intensity profile of the two sources
and extract the updated separation estimate. Next, I conduct a hypothesis test: if the separation esti-
mate is smaller than the underlying transverse distance, the null hypothesis is accepted, and I update the
separation parameter, iterating the process with a new measurement strategy. I restart the iteration if
the alternative hypothesis is accepted and the estimate exceeds the actual separation. I refine my estima-
tor through the Bayesian adaptive scheme, achieving an optimal measurement strategy at the end of the
process. My study demonstrates the superiority of this approach over current methods:
- Reduction in type-II error —Considering the asymmetric setting, the error in this probabilistic updating
process is minimized if the type-II error is decreased. Using Quantum Stein’s Lemma, I lower bound
the probability of false negatives with relative entropy, highlighting the quantum advantage.
- Lower variance in estimators—Numerical simulations indicate that the Adaptive Hypothesis Testing
estimator has lower variance than conventional imaging methods.
- Experimental practicality—The proposed strategy only requires conventional imaging techniques such
as position basis measurement.

## Coherent Estimation

The second part of the study relates to the work of Jordan and Howell (2023),
which uses the interference pattern of photons reflected from two closely spaced objects to explore their
”sub-Rayleigh” features. I generalize this model for multi-parameter estimation, where the inverse of the
Quantum Fisher Information matrix provides a lower bound on the covariance of an unbiased estimator.
My approach offers partial immunity against Rayleigh’s curse, resulting in a quadratic enhancement in
estimation precision akin to Grover’s algorithm:
- Improved precision scaling—For separation estimation in the sub-Rayleigh regime, the precision of the
estimator ˆl scales as 1/Varquantum(ˆl) ∼ (q2 − 2q3 + q4) l2 and 1/Varclassical(ˆl) ∼ (q2 − 2q3 + q4) l4,
where q is the intensity difference between the reflected pulses and l is the spatial separation between
the two objects of interest.
