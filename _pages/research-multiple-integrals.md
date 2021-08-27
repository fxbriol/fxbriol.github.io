---
title: "Transfer Learning for Numerical Integration"
permalink: /research/multiple-integrals/
author_profile: true
---

## The problem

Estimating integrals or expectations through simulation is one of the key challenges in computational statistics and machine learning. Indeed, many quantities of interest including posterior moments, model evidences, tail probabilities and marginal likelihoods take the form of intractable integrals, and we hence need algorithms to obtain accurate estimates. One of the key challenges is the cost (either computational or financial) of obtaining integrand evaluations. When working with complex models, this cost can be very large, which limits the number of integrand evaluations and can lead to poor accuracy of the resulting algorithms. In order to obtain highly accurate estimates of these integrals, it is therefore necessary to make use of any mathematical structure or side-information available.

There are of course many different types of side-information could you attempt to encode in your algorithms, but one key element which is often neglected is that you rarely have to compute a single isolated integral. Indeed, many practical problems will require you to compute several integrals which are somewhat related either simultaneously or sequentially. For example, in Bayesian statistics you usually have to compute some posterior expectation of interest, but you will also often want to calculate similar integrals when you collect more data or change your prior. Similarly, when working with mathematical models of physical or biological phenomenon, you will often have access to models of varying accuracy and may want to calculate integrals for each of these. 

## Contributions to this field



* Xi, X., ***Briol, F-X.*** & Girolami, M. (2018). *Bayesian quadrature for multiple related integrals*. International Conference on Machine Learning, PMLR 80:5369-5378. [(***Conference***)](http://proceedings.mlr.press/v80/xi18a.html) [(***Preprint***)](https://arxiv.org/abs/1801.04153)





* Sun, Z., Barp, A. & ***Briol, F-X.*** (2021). *Vector-valued control variates*.  



<p align="center">
  <img src="/images/BQ-illumination.png" alt="Application of Bayesian Quadrature to Global Illumination" width="100%">
</p>

<br>



## Funding

Funding for this work was generously provided by Amazon through an **Amazon Research Award** for a project entitled *"Transfer Learning for Numerical Integration in Expensive Machine Learning Systems"*. See the following [Amazon announcement](https://www.amazon.science/blog/recipients-of-the-2019-amazon-research-awards-announced) and [UCL press release](https://www.ucl.ac.uk/mathematical-physical-sciences/news/2020/jul/ucl-statistical-science-lecturer-receives-2019-amazon-research-award) for more details.




## More

*Bayesian numerical methods* (sometimes also called [*probabilistic numerics*](http://www.probabilistic-numerics.org)) provide an alternative way forward through the lense of Bayesian inference. The idea is to consider the solution of the numerical problem as a quantity of interest, then use Bayesian inference to obtain an estimate of this quantity. This allows for the use of prior information to be incorporated in the numerical method (very often using Gaussian processes), and for a detailed description of our uncertainty through the resulting posterior distribution. In fact, these algorithms are particularly useful for statistical applications since they allow for both the inference and the numerics to speak the same language, and as such uncertainty can be propagated throughout the entire procedure.


