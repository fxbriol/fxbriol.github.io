---
title: "Bayesian Numerical Methods"
permalink: /PN/
author_profile: true
---

## About

Whether for computing an integral, solving an optimisation problem, or solving differential equations, numerical methods are one of the core tools of statistics and machine learning.

* We usually want to obtain certain quantities of interest, but these take the form of some intractable integral/expectations.

* We often only know the probability density functions we are working with up to some unknown normalisation constant. For example, we usually do not know the normalisation constant of Bayesian posterior distributions (called the model evidence), and sometimes the likelihood itself has an unknown constant.

The most common solution to these problems is to use elaborate Monte Carlo methods or variational inference, but this can often lead to significant further computational challenges. Thankfully, Stein's method offers us an alternative approach. Using so-called *Stein operators*, it is straightforward to construct functions which integrate to a known value, and can be evaluated even without knowing normalisation constants of the densities of interest. This can also be used to construct notions of distance between probability distributions with these same properties called *Stein discrepancies*.

I have developed novel methodology in a range of fields thanks to this computational trick. In particular, I have focused on developing novel tools for Monte Carlo, and novel statistical estimators in frequentist and Bayesian settings. Further details can be found below.
