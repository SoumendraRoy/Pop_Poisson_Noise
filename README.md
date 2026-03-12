# Is Gravitational-Wave Population Analysis Overthinking or Reality?

Because the number of events observed by the LIGO–Virgo–KAGRA detectors is small compared to the true number of binary black hole (BBH), binary neutron star (BNS), and neutron star–black hole (NSBH) mergers occurring in the Universe, a natural question arises:

**Can we reliably infer the merger rate and population properties of compact binaries from such a limited number of detections?**

This repository explores this question in hierarchical Bayesian inference. We show that even with a relatively small number of observations, population inference remains **unbiased**. In other words, the true population parameters are correctly recovered, but with larger uncertainties when the number of observations is small.

This naturally leads to another question: why do some population trends reported in successive gravitational-wave transient catalogs sometimes change or weaken? For example:

- unequal-mass binaries favor higher effective spin, or  
- the merger rate drops on the left side of the 35 Msun  

appears less significant in later catalogs.

The reason is that the **true population model of compact binary mergers is unknown**. As new data become available, we modify the population model and the hyperpriors to better capture features suggested by the data. This happens in both **strongly parameterized models** and **weakly parameterized models**. Explictly:

- in parametric model, the functional form of the population of mass, spin and redshift may change or the prior on the hyperparameters are updated,
- in 'non-parametric' approaches, choices such as bin sizes, Gaussian process kernels, or hyperpriors (or hyperhyperprior) are updated.

However, if the population model and priors were kept exactly the same between the *n*-th and *(n+1)*-th gravitational-wave catalogs, the allowed region of the hyperparameter space (remember the integrate merger rate is also a hyperparameter) in the *(n+1)* analysis would simply be a **subset of the region allowed by the n-th analysis**.
