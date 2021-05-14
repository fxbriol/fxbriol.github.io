---
title: "Stein's Method as a Computational Tool"
permalink: /research/Stein/
author_profile: true
---

## About

My main research interests consist in developing novel statistical or machine learning methodology which can deal with computational expensive or intractable models. From a computational viewpoint, two of the main challenges in this context are: 

* We usually want to obtain certain quantities of interest, but these take the form of some intractable integral/expectations. Examples include Bayesian posterior moments, marginal likelihoods or expected losses.

* We often only know the probability density functions we are working with up to some unknown normalisation constant. For example, we usually do not know the normalisation constant of Bayesian posterior distributions (called the model evidence), and sometimes the likelihood itself has an unknown constant (this includes so-called unnormalised models, or doubly-intractable problems in a Bayesian setting).

The most common solution to these problems is to use elaborate Monte Carlo methods or variational inference, but this can often lead to significant further computational challenges. Thankfully, Stein's method offers us an alternative approach. Using so-called *Stein operators*, it is straightforward to construct functions which integrate to a known value, and can be evaluated even without knowing normalisation constants of the densities of interest. This can also be used to construct notions of distance between probability distributions with these same properties called *Stein discrepancies*.

## Contributions to this field

I have developed novel methodology in a range of fields thanks to the tools from Stein's method. In particular, I have focused on developing novel tools for Monte Carlo, and novel statistical estimators in frequentist and Bayesian settings. 

If you would like to get an in-depth introduction to this topic, see the following review paper:

   * Anastasiou, A., Barp, A., ***Briol, F-X.***, Ebner, B., Gaunt, R. E., Ghaderinezhad, F., Gorham, J., Gretton, A., Ley, C., Liu, Q., Mackey, L., Oates, C. J., Reinert, G. & Swan, Y. (2021). *Stein's method meets statistics: A review of some recent developments*. arXiv:2105.03481. [(***Preprint***)](https://arxiv.org/abs/2105.03481)


If you already know about Stein's method, you might instead be interested in my work in a range of areas including:

* Control variates to reduce the variance of Monte Carlo/MCMC estimators:

  * Oates, C. J., Cockayne, J., ***Briol, F-X.*** & Girolami, M. (2019). *Convergence rates for a class of estimators based on Stein's identity*. Bernoulli, Vol. 25, No. 2, 1141-1159. [(***Journal***)](https://projecteuclid.org/euclid.bj/1551862846) [(***Preprint***)](https://fxbriol.github.io/pdfs/Bernoulli_1551862846.pdf)

  * Si, S., Oates, C. J., Duncan, A. B., Carin, L., ***Briol. F-X.*** (2020). *Scalable control variates for Monte Carlo methods via stochastic optimization*. arXiv:2006.07487. [(***Preprint***)](https://arxiv.org/abs/2006.07487) [(***Video***)](https://www.youtube.com/watch?v=6MheW58gyKA)


<p align="center">
  <img src="/images/Stein-CV.png" alt="Control Variates from Stein's Method" width="75%">
</p>

<br>

* Statistical estimation methods for models with unnormalised likelihoods:

  * Barp, A., ***Briol, F-X.***, Duncan, A. B., Girolami, M., Mackey, L. (2019). *Minimum Stein discrepancy estimators*. Neural Information Processing Systems, 12964-12976. [(***Conference***)](https://papers.nips.cc/paper/9457-minimum-stein-discrepancy-estimators) [(***Preprint***)](https://arxiv.org/abs/1906.08283) [(***Talk/Video***)](https://slideslive.com/38917866/minimun-stein-discrepancy-estimators)

  * Mastubara, T., Knoblauch, J., ***Briol, F-X.***, Oates, C. J. (2021). *Robust generalised Bayesian inference for intractable likelihoods*. arXiv:2104.07359. [(***Preprint***)](https://arxiv.org/abs/2104.07359) [(***Code***)](https://github.com/takuomatsubara/KSD-Bayes)

<p align="center">
  <img src="/images/KSD-Bayes.png" alt="Robust inference with KSD-Bayes" width="100%">
</p>

<br>


* Novel samplers for approximating complicated probability distributions such as Bayesian posterior distributions:

  * Chen, W. Y., Mackey, L., Gorham, J. ***Briol, F-X.*** & Oates, C. J. (2018). *Stein points*. International Conference on Machine Learning, PMLR 80:843-852. 
[(***Conference***)](http://proceedings.mlr.press/v80/chen18f.html) [(***Preprint***)](https://arxiv.org/abs/1803.10161) [(***Code***)](https://github.com/wilson-ye-chen/stein_points)

  * Chen, W. Y., Barp, A., ***Briol, F-X.***, Gorham, J., Girolami, M., Mackey, L., Oates, C. J. (2019). *Stein point Markov chain Monte Carlo*. International Conference on Machine Learning, PMLR 97:1011-1021. [(***Conference***)](http://proceedings.mlr.press/v97/chen19b.html) [(***Preprint***)](https://arxiv.org/abs/1905.03673) [(***Code***)](https://github.com/wilson-ye-chen/sp-mcmc)


<p align="center">
  <img src="/images/SP.png" alt="Stein Points" width="75%">
</p>


