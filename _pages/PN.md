---
title: "Bayesian Numerical Methods"
permalink: /research/PN/
author_profile: true
---

## About

Whether for computing an integral, solving an optimisation problem, or solving differential equations, numerical methods are one of the core tools of statistics and machine learning. Most of the numerical methods available come from the field of numerical analysis, where one of the common assumption is that a high level of accuracy can be obtain by for example obtaining more function values or using a finer mesh or step-size. In this settings, strong theoretical guarantees can usually be provided in the form of worst-case errors.

Unfortunately, due to the increasing complexity and computational cost of modern statistical machine learning models, there are many application areas where obtaining more function values is simply not feasible. The worst-case theoretical guarantees are therefore not particularly useful since they are designed with an alternative setting in mind, and as a result can be overly pessimistic.

*Bayesian numerical methods* (sometimes also called [*probabilistic numerics*](http://www.probabilistic-numerics.org)) provide an alternative way forward through the lense of Bayesian inference. The idea is to consider the solution of the numerical problem as a quantity of interest, then use Bayesian inference to obtain an estimate of this quantity. This allows for the use of prior information to be incorporated in the numerical method, and for a detailed description of our uncertainty through the resulting posterior distribution. In fact, these algorithms are particularly useful for statistical applications since they allow for both the inference and the numerics to speak the same language, and as such uncertainty can be propagated throughout the entire procedure.

The most well-know algorithm from this field is *Bayesian optimisation*, which has been used in academia and industry to tune large scale models. However, there is an increasingly active research field exploring other uses of Bayesian inference for integration, linear algebra or differential equations.


## Contributions to this field

My own work has focused on *Bayesian quadrature*, a family of Bayesian inference schemes for tackling the computation of intractable integrals. Although the first version of this algorithm appeared in the 1980s (and certain aspects even in the 1960s), 

Following review paper, which was published with discussion and rejoinder in Statistical Science, is a good starting point:

* ***Briol, F-X.***, Oates, C. J., Girolami, M., Osborne, M. A. & Sejdinovic, D. (2019). *Probabilistic integration: a role in statistical computation?* Statistical Science, Vol 34, Number 1, 1-22. [(***Journal***)](https://projecteuclid.org/euclid.ss/1555056025) [(***Preprint***)](https://fxbriol.github.io/pdfs/STS660.pdf) [(***Supplement***)](https://fxbriol.github.io/pdfs/STS660_supplement.pdf)


<p align="center">
  <img src="/images/BQ-sketch.png" alt="Sketch of the Bayesian Quadrature Algorithm" width="65%">
</p>

<br>

I have also contributed a number of novel methodologies to improve the scalability and accuracy of the method. See for example:

* ***Briol, F-X.***, Oates, C. J., Cockayne, J., Chen, W. Y. & Girolami, M. (2017). *On the sampling problem for kernel quadrature*. Proceedings of the 34th International Conference on Machine Learning, PMLR 70:586-595. [(***Conference***)](http://proceedings.mlr.press/v70/briol17a.html) [(***Preprint***)](https://arxiv.org/abs/1706.03369) 

* ***Briol, F-X.***, Oates, C. J., Girolami, M. & Osborne, M. A. (2015). *Frank-Wolfe Bayesian Quadrature: probabilistic integration with theoretical guarantees*. Advances In Neural Information Processing Systems (NIPS), 1162-1170. [(***Preprint***)](https://arxiv.org/abs/1506.02681) [(***Conference***)](https://papers.nips.cc/paper/5749-frank-wolfe-bayesian-quadrature-probabilistic-integration-with-theoretical-guarantees)

On the modelling side, I have also extended the approach to use alternatives to standard Gaussian process regression, including through the use of tree-based models and multi-output Gaussian processes:

* Xi, X., ***Briol, F-X.*** & Girolami, M. (2018). *Bayesian quadrature for multiple related integrals*. International Conference on Machine Learning, PMLR 80:5369-5378. [(***Conference***)](http://proceedings.mlr.press/v80/xi18a.html) [(***Preprint***)](https://arxiv.org/abs/1801.04153)

* Zhu, H., Liu, X., Kang, R., Shen, Z., Flaxman, S., ***Briol, F-X.*** (2020). *Bayesian probabilistic numerical integration with tree-based models*. Neural Information Processing Systems, 5837-5849. [(***Conference***)](https://proceedings.neurips.cc/paper/2020/hash/3fe94a002317b5f9259f82690aeea4cd-Abstract.html) [(***Preprint***)](https://arxiv.org/abs/2006.05371)


Finally, an interesting by-product of my interest in Bayesian numerical methods has been the following paper, which provides some of the most general theoretical results for Gaussian process regression (including implications for Bayesian optimisation and Bayesian quadrature):	

* Wynne, G., ***Briol, F-X.***, Girolami, M. (2020). *Convergence guarantees for Gaussian process means with misspecified likelihoods and smoothness*. arXiv:2001.10818. Accepted for publication in the Journal of Machine Learning Research (subject to minor revisions). [(***Preprint***)](https://arxiv.org/abs/2001.10818)


<p align="center">
  <img src="/images/BQ-illumination.png" alt="Application of Bayesian Quadrature to Global Illumination" width="100%">
</p>

<br>

