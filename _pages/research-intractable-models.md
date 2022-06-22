---
title: "Inference for Intractable Models"
permalink: /research/intractable-models/
author_profile: true
---

## About

Researchers in Statistics and Machine Learning are having to work with ever-larger models developed by scientists or engineers. One particular challenge is that these models become so complex that standard tools for parameter estimation are not fit for purpose anymore. For example, most standard methods such as maximum likelihood estimation or Bayesian inference rely on the availability of a likelihood function that represents our model. But when the underlying phenomena being modelled is highly complex, it is often not possible to specify the likelihood associated to our model. 

The term *intractable model* is a general term encompassing all models for which the corresponding likelihood function is not available. However, there are many different types of intractability. A first example includes *intractable generative models* or *simulator-based models*, which are models for which nothing is known about the likelihood function, but it is possible to simulate new data given a fixed value of the parameters. A second example are  *unnormalised models*, in which case the likelihood function can be evaluated, but only up to some unknown normalisation constant. For each class of intractable model, alternative approaches need to be developed for parameter estimation.


## Contributions to this field

My work in this area focuses on developing novel methodology for inference with intractable models which have several desirable properties. First, our algorithms should be robust in the sense that mild model misspecification or a few outliers should not have a disproportionate impact. This is particularly important when modelling complex phenomena because our models will ever be at best some reasonable idealisation of the underlying process. Second, the algorithm should be efficient in the sense that we obtain estimates which are as accurate as possible given the finite amount of data available. This is particularly important because collecting new data can be a costly process. Finally, the algorithms should be scalable and computationally efficient in the sense that they should be easy to implement and able to deal with large datasets or high-dimensional problems.

For generative models, I have proposed and analysed novel estimators based on a family of distances called *maximum mean discrepancy* where specific instances can be chosen to balance the three desirable properties mentioned above:

* ***Briol, F-X.***, Barp, A., Duncan, A. B., Girolami, M. (2019). *Statistical inference for generative models with maximum mean discrepancy*. arXiv:1906.05944. [(***Preprint***)](https://arxiv.org/abs/1906.05944) [(***Talk/Video***)](https://youtu.be/mm7bHjEzhow)

* Dellaporta, C., Knoblauch, J., Damoulas, T. ***Briol. F-X.*** (2022). *Robust Bayesian inference for simulator-based models via the MMD posterior bootstrap*. Proceedings of The 25th International Conference on Artificial Intelligence and Statistics (AISTATS), PMLR 151:943-970. [(***Conference***)](https://proceedings.mlr.press/v151/dellaporta22a.html) [(***Preprint***)](https://arxiv.org/abs/2202.04744) [(***Code***)](https://github.com/haritadell/npl_mmd_project.git) [(***Video***)](https://youtu.be/h4yWC-01oqQ)

<p align="center">
  <img src="/images/intractable-naturalgradient.png" alt="Natural Gradient Descent for Maximum Mean Discrepancy Estimators" width="60%">
</p>

<br>

I have also worked on developing methods which can significantly reduce the number of simulations required for these generative models, which can significantly impact the computational cost of the procedure:

* Niu, Z., Meier, J. & ***Briol, F-X.*** (2021). *Discrepancy-based inference for intractable generative models using quasi-Monte Carlo*. arXiv:2106.11561. [(***Preprint***)](https://arxiv.org/abs/2106.11561)

<p align="center">
  <img src="/images/mvgandk_d2_scatter.png" alt="QMC Sampling from a g-and-k Model" width="50%">
</p>

<br>



For unnormalised models, a convenient choice of distance are the so-called [Stein discrepancies](https://fxbriol.github.io/research/Stein/), which I have used to obtain flexible families of frequentist statistical estimators or generalised Bayesian inference approaches.

* Barp, A., ***Briol, F-X.***, Duncan, A. B., Girolami, M., Mackey, L. (2019). *Minimum Stein discrepancy estimators*. Neural Information Processing Systems, 12964-12976. [(***Conference***)](https://papers.nips.cc/paper/9457-minimum-stein-discrepancy-estimators) [(***Preprint***)](https://arxiv.org/abs/1906.08283) [(***Talk/Video***)](https://slideslive.com/38917866/minimun-stein-discrepancy-estimators)

* Mastubara, T., Knoblauch, J., ***Briol, F-X.*** & Oates, C. J. (2022). *Robust generalised Bayesian inference for intractable likelihoods*. To appear in the Journal of the Royal Statistical Society: Series B. arXiv:2104.07359. [(***Journal***)](https://rss.onlinelibrary.wiley.com/doi/10.1111/rssb.12500) [(***Preprint***)](https://arxiv.org/abs/2104.07359) [(***Code***)](https://github.com/takuomatsubara/KSD-Bayes) [(***Video***)](https://drive.google.com/file/d/1gs016iDfvDbO07GBglI5xtOB8bFmjbAH/view)

* Matsubara, T., Knoblauch, J., ***Briol, F-X.*** & Oates, C. J. (2022). *Generalised Bayesian inference for discrete intractable likelihood*. arXiv:2206.08420. [(***Preprint***)](https://arxiv.org/abs/2206.08420) [(***Code***)](https://github.com/takuomatsubara/Discrete-Fisher-Bayes)

<p align="center">
  <img src="/images/protein-signalling-network.png" alt="Robust Bayesian Estimation of Protein Signalling Networks" width="60%">
</p>

<br>

As part of my work in the Data-Centric Engineering programme of The Alan Turing Institute, I have also worked in specialising some of the methods above to solve important engineering problems, in particular in the field of telecommunications:

* Bharti, A., ***Briol, F-X.***, Pedersen, T. (2021). *A general method for calibrating stochastic radio channel models with kernels*. IEEE Transactions on Antennas and Propagation. [(***Journal***)](https://ieeexplore.ieee.org/document/9445690) [(***Preprint***)](https://arxiv.org/abs/2012.09612) [(***Code***)](https://github.com/bharti-ayush/Kernel-based-ABC)

* ***Briol, F-X.***, Bharti, A. (2021). *Using machine learning to improve the reliability of wireless communication systems*.  [(***Turing Institute Blog Post***)](https://www.turing.ac.uk/blog/using-machine-learning-improve-reliability-wireless-communication-systems)

<p align="center">
  <img src="/images/stochastic-radio-channels.png" alt="Intractable Models in Telecommunications" width="70%">
</p>

<br>
