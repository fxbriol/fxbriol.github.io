---
title: "Transfer Learning for Numerical Integration"
permalink: /research/multiple-integrals/
author_profile: true
---

## About

Whether for computing an integral, solving an optimisation problem, or solving differential equations, numerical methods are one of the core tools of statistics and machine learning. Most of the numerical methods available come from the field of numerical analysis, where one of the common assumption is that a high level of accuracy can be obtain by for example obtaining more function values or using a finer mesh or step-size. In this setting, strong theoretical guarantees can usually be provided in the form of worst-case errors.

Unfortunately, due to the increasing complexity and computational cost of modern statistical machine learning models, there are many application areas where obtaining more function values is simply not feasible. The worst-case theoretical guarantees are therefore not particularly useful since they are designed with an alternative setting in mind, and as a result can be overly pessimistic.

*Bayesian numerical methods* (sometimes also called [*probabilistic numerics*](http://www.probabilistic-numerics.org)) provide an alternative way forward through the lense of Bayesian inference. The idea is to consider the solution of the numerical problem as a quantity of interest, then use Bayesian inference to obtain an estimate of this quantity. This allows for the use of prior information to be incorporated in the numerical method (very often using Gaussian processes), and for a detailed description of our uncertainty through the resulting posterior distribution. In fact, these algorithms are particularly useful for statistical applications since they allow for both the inference and the numerics to speak the same language, and as such uncertainty can be propagated throughout the entire procedure.

The most well-know algorithm from this field is *Bayesian optimisation*, which has been used in academia and industry to tune large scale models. However, there is an increasingly active research field exploring other uses of Bayesian inference for integration, linear algebra or differential equations.


## Contributions to this field

My own work has focused on *Bayesian quadrature*, a family of Bayesian inference schemes for tackling the computation of intractable integrals. Although the first Bayesian quadrature algorithm appeared in the 1980s (and certain aspects even in the 1960s), initial developments were slowed down because computers were not yet able to handle such models. However, the field has recently received renewed interest due to the many advantages provided by Bayesian numerical methods and the rapid improvements in our computing abilities. My own contributions have been on the methodology side, where I have shown how to improve the algorithms for improved computational accuracy, and the theoretical side, where I have provided very general convergence guarantees under a wide range of scenarios including when the Bayesian model is misspecified. 

* Xi, X., ***Briol, F-X.*** & Girolami, M. (2018). *Bayesian quadrature for multiple related integrals*. International Conference on Machine Learning, PMLR 80:5369-5378. [(***Conference***)](http://proceedings.mlr.press/v80/xi18a.html) [(***Preprint***)](https://arxiv.org/abs/1801.04153)





* Sun, Z., Barp, A. & ***Briol, F-X.*** (2021). *Vector-valued control variates*.  



<p align="center">
  <img src="/images/BQ-illumination.png" alt="Application of Bayesian Quadrature to Global Illumination" width="100%">
</p>

<br>



## Funding

Funding for this work was generously provided by Amazon through an **Amazon Research Award** for a project entitled *"Transfer Learning for Numerical Integration in Expensive Machine Learning Systems"*. See the following [Amazon announcement](https://www.amazon.science/blog/recipients-of-the-2019-amazon-research-awards-announced) and [UCL press release](https://www.ucl.ac.uk/mathematical-physical-sciences/news/2020/jul/ucl-statistical-science-lecturer-receives-2019-amazon-research-award) for more details.
